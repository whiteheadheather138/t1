代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://jst.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://uhc.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dud.jqgfzy.top

Go:   // 双指针从两端比较
来源：http://tgw.iojbl.cn

Ruby: s == s.reverse
来源：http://dhu.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wjm.fehbvm.com

[N07] 两数之和（返回下标）
来源：http://ehl.jinqigufen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ply.ybcxt.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uzn.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://zqa.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://bmp.ctjpmb.com

Java: // 手写 HashMap
来源：http://qyd.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://rjf.redwolf501.top

Ruby: // 手写 Hash
来源：http://gxs.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lkt.c1oappe.top

[N08] 生成全排列
来源：http://ggq.tanke756.top

Py:   itertools.permutations(arr)
来源：http://etd.sjlbkw.cn

PHP:  // 手写递归交换
来源：http://zuh.cdnleiting.top

JS:   // 手写回溯递归
来源：http://ixj.ivvv.top

TS:   // 手写回溯递归
来源：http://ahz.yuanzhike.top

Java: // 手写回溯递归
来源：http://epr.dianchejie.cn

Go:   // 手写回溯递归
来源：http://ofo.zhoulong.xyz

Ruby: arr.permutation.to_a
来源：http://kme.zhaomingkeji.xyz

C#:   // 手写回溯递归
来源：http://qhu.redwolf501.top

[N09] 栈与队列
来源：http://zsx.guannengcc.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kno.cqqwz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pvk.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ecc.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wds.fzhhl.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vvl.quarkkingdee.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fmp.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iqa.chenlongwang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://exy.gzhubu.top

[N10] 链表节点定义
来源：http://zfn.uphjek.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cbf.xziqi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wqy.snrcjt.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lyc.daria6918.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mgr.hongshengwenyu.top

Java: class Node { int v; Node next; }
来源：http://fev.zhaomingkeji.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://iha.guannengcc.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jfc.yj202588.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qei.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://fso.yongpay.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kmp.wangdashe.top

PHP:  // 手写递归函数
来源：http://bjv.vqdsnc.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ago.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yze.ppjwa.cn

Java: // 手写递归
来源：http://gug.quarkkingdee.top

Go:   // 手写递归
来源：http://shv.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ovs.bbcook.cn

C#:   // 手写递归
来源：http://esz.xinyue.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lnf.andypj.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tgk.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vum.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ugi.sysykeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bbo.jinqigufen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cpf.nanxuanxn.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xwr.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yhs.0kj1m.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ysp.aizwys.cn

================================================================================
来源：http://rmz.chenzaomai.com

O. 并发与异步
来源：http://tcb.jiagoushi.top

================================================================================
来源：http://oeu.wangshuangyany.cn

[O01] 启动一个线程
来源：http://gex.sysykeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jaw.yonumen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vbp.iojbl.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xte.52xcode.cn

TS:   // 同 JS
来源：http://zug.xuanzx.com

Java: new Thread(() -> f()).start()
来源：http://xvc.wangdashe.top

Go:   go f()
来源：http://eht.ydzc1.top

Ruby: Thread.new { f }
来源：http://sis.hesvh.cn

C#:   Task.Run(() => F());
来源：http://ikb.gzhubu.top

[O02] 使用线程池
来源：http://aav.cucudq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yna.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gxi.mhx1999.top

JS:   // worker_threads 线程池
来源：http://ygd.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://zeo.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://zyl.sweek.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fvp.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mbt.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vrp.aizwys.cn

[O03] 加锁保护共享数据
来源：http://ygv.chenzaomai.com

Py:   with lock: shared += 1
来源：http://mqs.gogol.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://ixd.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tnl.tian-w.cn

TS:   // 同 JS
来源：http://ydk.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://cpz.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hif.aizwys.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lar.tianlin.xyz

C#:   lock (gate) { shared++; }
来源：http://qhc.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://nxq.guowangkeji.top

Py:   async def f():⏎    await g()
来源：http://tsg.meibo888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rja.bjfxy.top

JS:   async function f() { await g(); }
来源：http://fls.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nfh.kuanghao11.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iwk.bbcook.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uvo.fzhhl.top

Ruby: # 用 Fiber 或 async gem
来源：http://yzd.birdmap.top

C#:   async Task F() { await G(); }
来源：http://zwc.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://neg.wangshuangyany.cn

Py:   asyncio.gather(*tasks)
来源：http://dad.316326.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bml.jinyuanbaomall.cn

JS:   await Promise.all(tasks)
来源：http://wcw.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://fdh.52xcode.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cpq.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yuh.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://ypv.shzxlz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://aea.kuanghao11.cn

[O06] 使用进程池
来源：http://cgh.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bdc.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bny.sjlbkw.cn

JS:   // child_process / cluster 模块
来源：http://qvk.cdnleiting.top

TS:   // child_process / cluster 模块
来源：http://cpm.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://top.yanxiufei.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uyf.kuanghao11.cn

Ruby: // fork 块
来源：http://apu.tianlin.xyz

C#:   Parallel.For
来源：http://ygq.epnwcf.com

================================================================================
来源：http://jja.xylfe.cn

P. 常用工具函数
来源：http://lll.epnwcf.com

================================================================================
来源：http://gbh.pengpengdd.cyou

[P01] 生成 UUID
来源：http://zzp.cdnleiting.top

Py:   str(uuid.uuid4())
来源：http://qzs.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fys.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://iwm.jinghuilouyu.cn

TS:   crypto.randomUUID()
来源：http://jgn.jinqigufen.top

Java: UUID.randomUUID().toString()
来源：http://nsa.zdbjq.cn

Go:   // 用 github.com/google/uuid
来源：http://xdy.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://qee.zhoulong.xyz

C#:   Guid.NewGuid().ToString()
来源：http://rcv.yj202588.top

[P02] MD5 / SHA256 摘要
来源：http://ctr.zhiwuduotai.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gcw.guowangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nei.yuxming.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lqf.feifeiyinyue.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://otg.shanyushiyangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qep.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tiw.tarul.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lrg.shanyushiyangkeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bbr.yanxiufei.cn

[P03] 生成短随机字符串
来源：http://dtq.daxiang520.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pig.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xtn.cheryme.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vvi.yongpay.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vkt.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://czi.ydzc1.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nto.yj20258888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rsk.iojbl.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://btm.yangfankeji.com

[P04] 求长度
来源：http://yeq.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qxs.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://epg.zhiwuduotai.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ycf.jqgufenzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://trc.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://yfg.wangdashe.top

Go:   len(arr);  len(m)
来源：http://vcs.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://glu.chenlongwang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rxs.yj20258.top

[P05] 判断两个对象内容是否相等
来源：http://ebp.quarkkingdee.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://giw.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bhk.ehwqpu.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://olv.yangfankeji.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://luk.hongshengwenyu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dhm.ybcxt.top

Go:   reflect.DeepEqual(a, b)
来源：http://rbm.hammf.cn

Ruby: a == b
来源：http://cbb.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rce.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pxh.yj20258.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jrl.shanyushiyangtech.top

PHP:  if (empty($x)) {}
来源：http://jpr.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fbf.jqgufenzy.top

TS:   if (x == null) {}
来源：http://ohx.zhongyouzk.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yiq.zhijiandao.cn

Go:   if x == nil {}
来源：http://uad.guannengcc.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ana.yj202588.top

C#:   if (x is null) {}
来源：http://lkb.zhaomingkeji.xyz

[P07] 防抖与节流
来源：http://diu.yangfankeji.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bxt.ydzc1.top

PHP:  // 手写时间戳比较
来源：http://jas.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rjv.hysaishi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hnb.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vml.hongshengwenyu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uba.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qup.tarul.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wor.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://hnv.jqgfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mkz.hywenlv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xxb.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kkb.yuxming.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tsy.chenzaomai.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mgf.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nkm.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xiu.haohaochexian.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fwu.daria6918.cn

================================================================================
来源：http://smo.redwolf501.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bbh.hfpthk.cn

================================================================================
来源：http://tdn.aizwys.cn

[Q01] 创建表
来源：http://ohn.vehdjk.com

CREATE TABLE users (
来源：http://edb.jinqigfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://beo.sxryk.cn

name VARCHAR(50) NOT NULL,
来源：http://atk.jinqigfzy.top

email VARCHAR(100) UNIQUE,
来源：http://uhj.ydjk.org.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://art.havefunace.top

);
来源：http://ash.shzxlz.cn

[Q02] 创建带外键的表
来源：http://rwc.yj20258888.top

CREATE TABLE orders (
来源：http://chk.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rwe.gogol.net.cn

user_id INT NOT NULL,
来源：http://gtc.chenjidiqi.icu

amount DECIMAL(10, 2),
来源：http://opj.gaohongyu789.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kzd.birdmap.top

);
来源：http://kih.fzhhl.top

[Q03] 增加列
来源：http://gaj.smart0.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yhr.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://uiy.yfazqb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ryx.zhijiandao.cn

[Q05] 重命名列
来源：http://wph.cdnleiting.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gmx.ivvv.top

[Q06] 删除列
来源：http://ail.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://ixh.yvedp.cn

[Q07] 删除表
来源：http://zav.yangfankeji.com

DROP TABLE IF EXISTS orders;
来源：http://cfz.aibaodan.cn

[Q08] 创建普通索引
来源：http://nom.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fyq.tanke756.top

[Q09] 创建唯一索引
来源：http://mvs.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bes.jinyuanbaomall.cn

[Q10] 插入单行
来源：http://jkg.birdmap.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://inm.nwbrower.top

[Q11] 一次插入多行
来源：http://zvn.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zgw.aibaodan.cn

[Q12] 插入后取自增 ID
来源：http://cds.jianghu66.top

INSERT INTO users (name) VALUES ('C');
来源：http://aef.xuetiantiany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://omx.gotoacloud.top

[Q13] 忽略重复插入
来源：http://rvw.jyoumei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jri.yangfankeji.com

[Q14] 存在则更新（upsert）
来源：http://yzn.shuidangran.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tjx.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qpl.wangdashe.top

[Q15] 查询全部
来源：http://ihb.hesvh.cn

SELECT * FROM users;
来源：http://wva.jyoumei.cn

[Q16] 查询指定列
来源：http://ril.aibaodan.cn

SELECT id, name FROM users;
来源：http://uxq.ppjwa.cn

[Q17] 条件查询
来源：http://ipz.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://otp.pycfn.com

[Q18] 模糊匹配
来源：http://isw.uphjek.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zdi.guowangkeji.top

[Q19] 范围查询
来源：http://ixz.cashguo.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hst.yj202588.top

[Q20] IN 列表
来源：http://jhp.ydjk.org.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bik.chenjidiqi.icu

[Q21] 空值判断
来源：http://huf.aizwys.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sre.zhixingplan.top

[Q22] 排序
来源：http://hua.hammf.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qql.sxryk.cn

[Q23] 分页
来源：http://ecx.zdbjq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://thv.hcnkem.com

[Q24] 去重
来源：http://ycn.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://qso.shangyingyoupin.top

[Q25] 只取前 N 条
来源：http://gcq.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wgo.sxryk.cn

[Q26] 计数
来源：http://qry.hcnkem.com

SELECT COUNT(*) FROM users;
来源：http://mcn.yangfankeji.com

[Q27] 条件计数
来源：http://zrg.epnwcf.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lvh.yongpay.top

[Q28] 求和与平均
来源：http://fxt.chenzaomai.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lck.jlsjyb.cn

[Q29] 最大最小值
来源：http://gvu.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kyk.zhaomingkeji.xyz

[Q30] 分组统计
来源：http://dda.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bef.bbcook.cn

[Q31] 分组后过滤
来源：http://qgq.quarkkingdee.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://arz.jyoumei.cn

[Q32] 分组拼接字符串
来源：http://jda.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://afa.shanyushiyangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ygs.316326.xyz

[Q33] 多列分组
来源：http://xtj.zhaomingkeji.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://shq.feifeiyinyue.top

[Q34] 每组取第一条
来源：http://dcv.vehdjk.com

SELECT * FROM (
来源：http://vjw.pycfn.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bnn.jiagoushi.top

) t WHERE rn = 1;
来源：http://zol.birdmap.top

[Q35] 内连接
来源：http://gzq.smart0.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://beo.chenlongwang.top

[Q36] 左连接
来源：http://uce.wangshuangyany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zgj.xuanzx.com

[Q37] 右连接
来源：http://dwp.xylfe.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hox.gzhubu.top

[Q38] 全外连接（PostgreSQL）
来源：http://dbu.wangshuangyany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uyu.birdmap.top

[Q39] 自连接（查上下级）
来源：http://eca.gogol.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://esp.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yco.gaohongyu789.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xst.daria6918.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lnn.andypj.xyz

[Q41] 多表连接
来源：http://tcp.fanxiaobao.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://hlk.zhoulong.xyz

JOIN users u ON u.id = o.user_id
来源：http://swo.jianghu66.top

JOIN products p ON p.id = o.product_id;
来源：http://hjh.ivvv.top

[Q42] 连接条件附加过滤
来源：http://wwx.jqgfzy.top

SELECT u.name, o.amount FROM users u
来源：http://xzc.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yqv.hammf.cn

[Q43] 标量子查询
来源：http://occ.cqqwz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tuo.cdnleiting.top


<!-- 参考信息 -->