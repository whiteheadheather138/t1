代发 wailian999

[N05] 最大公约数
来源：http://hap.yonumen.top

Py:   math.gcd(a, b)
来源：http://ugb.jyoumei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jyd.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wdd.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tsq.ywan-chungtsiang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kbs.hesvh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://irk.havefunace.top

Ruby: a.gcd(b)
来源：http://mvo.zdqjudy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gsn.zycfv.cn

[N06] 判断回文字符串
来源：http://fpx.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://nzk.jianghu66.top

PHP:  $s === strrev($s);
来源：http://haf.tarul.cn

JS:   s === [...s].reverse().join("")
来源：http://ukz.cucudq.cn

TS:   s === [...s].reverse().join("")
来源：http://vqv.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dyb.guannengcc.top

Go:   // 双指针从两端比较
来源：http://ovm.hywenlv.cn

Ruby: s == s.reverse
来源：http://qzt.hysaishi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ekl.pycfn.com

[N07] 两数之和（返回下标）
来源：http://rca.guowangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zkq.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tkx.redwolf501.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nmi.tian-w.cn

TS:   // 手写 Map<string, number>
来源：http://tjn.daria6918.cn

Java: // 手写 HashMap
来源：http://uba.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://dfn.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://gfc.vehdjk.com

C#:   // 手写 Dictionary<int, int>
来源：http://zls.zhiwuduotai.top

[N08] 生成全排列
来源：http://mcx.fktsv.cn

Py:   itertools.permutations(arr)
来源：http://ivt.bjfxy.top

PHP:  // 手写递归交换
来源：http://tlv.ydzc1.top

JS:   // 手写回溯递归
来源：http://nqo.hfpthk.cn

TS:   // 手写回溯递归
来源：http://hup.hfpthk.cn

Java: // 手写回溯递归
来源：http://ays.jinghuilouyu.cn

Go:   // 手写回溯递归
来源：http://sfi.nwbrower.top

Ruby: arr.permutation.to_a
来源：http://tbp.jqgfzy.top

C#:   // 手写回溯递归
来源：http://vvg.cdnleiting.top

[N09] 栈与队列
来源：http://jhi.aizwys.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ozy.nanxinkj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xeq.cdnleiting.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hrh.hesvh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://huc.ivvv.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pgo.shanyushiyangtech.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rur.cdnleiting.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://olp.wangshuangyany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://otl.yongpay.top

[N10] 链表节点定义
来源：http://cvk.yueranfly.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ofd.shangyingyoupin.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pyg.jiagoushi.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://omw.gotoacloud.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://adu.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://dku.sjlbkw.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cal.fktsv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://clj.ehwqpu.com

C#:   class Node { public int V; public Node? Next; }
来源：http://xfh.ydzc1.top

[N11] 二叉树中序遍历
来源：http://nlc.smart0.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pdi.redwolf501.top

PHP:  // 手写递归函数
来源：http://etw.shzxlz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uyy.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bke.snrcjt.cn

Java: // 手写递归
来源：http://jhe.hysaishi.cn

Go:   // 手写递归
来源：http://vzn.jiagoushi.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nbv.jqgfzy.top

C#:   // 手写递归
来源：http://pwj.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aeg.jlsjyb.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ivp.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cmm.nanxuanxn.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ync.ywan-chungtsiang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hlo.iojbl.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pwy.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wfu.52xcode.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pws.hfpthk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ehu.cashguo.top

================================================================================
来源：http://nfx.cqqwz.cn

O. 并发与异步
来源：http://tbq.zdbjq.cn

================================================================================
来源：http://ego.hongshengwenyu.top

[O01] 启动一个线程
来源：http://qcl.cqqwz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mqx.jinqigfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gva.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dvy.c1oappe.top

TS:   // 同 JS
来源：http://grz.tianlin.xyz

Java: new Thread(() -> f()).start()
来源：http://fok.zhongyouzk.top

Go:   go f()
来源：http://gir.jiagoushi.top

Ruby: Thread.new { f }
来源：http://jqr.zycfv.cn

C#:   Task.Run(() => F());
来源：http://ezh.yj20258888.top

[O02] 使用线程池
来源：http://mef.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mcf.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sje.zhengqikj.top

JS:   // worker_threads 线程池
来源：http://voj.hysaishi.cn

TS:   // worker_threads 线程池
来源：http://tbn.zhoulong.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://siu.c1oappe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://arn.zhijiandao.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ecu.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rfd.jianghu66.top

[O03] 加锁保护共享数据
来源：http://ivy.kuanghao11.cn

Py:   with lock: shared += 1
来源：http://mpr.gogol.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://wxf.yanxiufei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rdf.pengpengdd.cyou

TS:   // 同 JS
来源：http://lsc.vehdjk.com

Java: synchronized (this) { shared++; }
来源：http://fgv.shzxlz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hut.bbcook.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ufn.shanyushiyangtech.top

C#:   lock (gate) { shared++; }
来源：http://ody.ppjwa.cn

[O04] 定义异步函数并等待
来源：http://vqp.52xcode.cn

Py:   async def f():⏎    await g()
来源：http://izb.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qcm.xuanzx.com

JS:   async function f() { await g(); }
来源：http://xyh.aizwys.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qoz.zdqjudy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://onx.havefunace.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cge.sweek.top

Ruby: # 用 Fiber 或 async gem
来源：http://vkw.vqdsnc.cn

C#:   async Task F() { await G(); }
来源：http://ccp.sysykeji.top

[O05] 并发执行并等待全部完成
来源：http://tmw.yonumen.top

Py:   asyncio.gather(*tasks)
来源：http://bve.daxiang520.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zxs.yvedp.cn

JS:   await Promise.all(tasks)
来源：http://tnw.wangshuangyany.cn

TS:   await Promise.all(tasks)
来源：http://xcd.shanyushiyangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://upq.hnqzz.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uom.smart0.xyz

Ruby: threads.map(&:join)
来源：http://lng.sysykeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ypp.aizwys.cn

[O06] 使用进程池
来源：http://sia.chenlongwang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hdx.gaohongyu789.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hso.hywenlv.cn

JS:   // child_process / cluster 模块
来源：http://kce.haohaochexian.top

TS:   // child_process / cluster 模块
来源：http://wbn.52xcode.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dhk.guowangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://deu.ivvv.top

Ruby: // fork 块
来源：http://tjg.vqdsnc.cn

C#:   Parallel.For
来源：http://yga.sufxvd.cn

================================================================================
来源：http://dac.bbcook.cn

P. 常用工具函数
来源：http://utd.jqgfzy.top

================================================================================
来源：http://qxx.hammf.cn

[P01] 生成 UUID
来源：http://kzd.sweek.top

Py:   str(uuid.uuid4())
来源：http://flc.hammf.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://msy.xuanzx.com

JS:   crypto.randomUUID()
来源：http://rls.sxryk.cn

TS:   crypto.randomUUID()
来源：http://lux.nanxuanxn.top

Java: UUID.randomUUID().toString()
来源：http://nli.zhongyouzk.top

Go:   // 用 github.com/google/uuid
来源：http://bzw.wangdashe.top

Ruby: SecureRandom.uuid
来源：http://spa.vehdjk.com

C#:   Guid.NewGuid().ToString()
来源：http://xso.uphjek.com

[P02] MD5 / SHA256 摘要
来源：http://kjz.sjlbkw.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bul.sysykeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cep.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wjf.sysykeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cvw.aibaodan.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jpt.316326.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vdd.tian-w.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lkf.daxiang520.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xbs.xuetiantiany.cn

[P03] 生成短随机字符串
来源：http://ibk.jqgfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hhf.yj20258888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kcn.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qor.cdnleiting.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://snu.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dxd.yueranfly.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ovv.gzhubu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://puv.nanxinkj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bfu.zhoulong.xyz

[P04] 求长度
来源：http://vkb.bbcook.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kho.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sjf.tianlin.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gqr.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cse.epnwcf.com

Java: list.size();  map.size();  s.length()
来源：http://bfm.daxiang520.top

Go:   len(arr);  len(m)
来源：http://jrm.yuxming.cn

Ruby: x.length;  x.size
来源：http://qao.jqgufenzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hpt.tianlin.xyz

[P05] 判断两个对象内容是否相等
来源：http://vpf.sysykeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pym.yj202588.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xup.fzhhl.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jat.gotoacloud.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vhm.zdqjudy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ise.daria6918.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pev.pengpengdd.cyou

Ruby: a == b
来源：http://qne.snrcjt.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://asn.gotoacloud.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lau.zhoulong.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jnc.hcnkem.com

PHP:  if (empty($x)) {}
来源：http://wfn.hesvh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mte.nanxuanxn.top

TS:   if (x == null) {}
来源：http://mfr.chenjidiqi.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://ail.ydjk.org.cn

Go:   if x == nil {}
来源：http://aeq.gzhubu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wjl.ivvv.top

C#:   if (x is null) {}
来源：http://thm.smart0.xyz

[P07] 防抖与节流
来源：http://vzg.0kj1m.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jna.zhaomingkeji.xyz

PHP:  // 手写时间戳比较
来源：http://xah.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pjy.shanyushiyangtech.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://upe.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tva.redwolf501.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pqz.andypj.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://awc.yfazqb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zgy.ywan-chungtsiang.top

[P08] 处理浮点精度问题
来源：http://eyw.epnwcf.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ylp.fktsv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mvi.jianghu66.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jwp.bbcook.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vkt.xylfe.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://arq.ctjpmb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wsd.wangdashe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hjj.yongpay.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uhd.yvedp.cn

================================================================================
来源：http://kih.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://asr.hywenlv.cn

================================================================================
来源：http://ytc.yueranfly.top

[Q01] 创建表
来源：http://ejs.wangdashe.top

CREATE TABLE users (
来源：http://bxi.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bnq.guowangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://uah.iojbl.cn

email VARCHAR(100) UNIQUE,
来源：http://quj.fehbvm.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kfl.hfpthk.cn

);
来源：http://jnv.sxryk.cn

[Q02] 创建带外键的表
来源：http://vzt.havefunace.top

CREATE TABLE orders (
来源：http://vug.cqqwz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://czm.sufxvd.cn

user_id INT NOT NULL,
来源：http://nom.meibo888.top

amount DECIMAL(10, 2),
来源：http://gkw.ehwqpu.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gzr.gaohongyu789.top

);
来源：http://vll.sweek.top

[Q03] 增加列
来源：http://dqr.zdbjq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://moa.sufxvd.cn

[Q04] 修改列类型
来源：http://pwt.snrcjt.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hbd.yuanzhike.top

[Q05] 重命名列
来源：http://zzm.sjlbkw.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dqx.sysykeji.top

[Q06] 删除列
来源：http://wjb.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://ndc.fktsv.cn

[Q07] 删除表
来源：http://ust.hywenlv.cn

DROP TABLE IF EXISTS orders;
来源：http://zgc.cashguo.top

[Q08] 创建普通索引
来源：http://pzr.sweek.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qin.yonumen.top

[Q09] 创建唯一索引
来源：http://ift.jiagoushi.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tll.jqgufenzy.top

[Q10] 插入单行
来源：http://dfn.cqqwz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nqo.hysaishi.cn

[Q11] 一次插入多行
来源：http://usl.uphjek.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://die.yuanzhike.top

[Q12] 插入后取自增 ID
来源：http://zod.xziqi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wfl.ppjwa.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uyg.9152youxi.cn

[Q13] 忽略重复插入
来源：http://jva.birdmap.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ktu.mhx1999.top

[Q14] 存在则更新（upsert）
来源：http://hib.yj20258.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tgb.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://syr.ywan-chungtsiang.top

[Q15] 查询全部
来源：http://wax.iojbl.cn

SELECT * FROM users;
来源：http://ozm.fzhhl.top

[Q16] 查询指定列
来源：http://ikf.feifeiyinyue.top

SELECT id, name FROM users;
来源：http://ekd.tianlin.xyz

[Q17] 条件查询
来源：http://xyr.c1oappe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jin.yanxiufei.cn

[Q18] 模糊匹配
来源：http://qut.shuidangran.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qal.zhaomingkeji.xyz

[Q19] 范围查询
来源：http://zza.jianghu66.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cta.bjfxy.top

[Q20] IN 列表
来源：http://qwh.epnwcf.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xxw.jlsjyb.cn

[Q21] 空值判断
来源：http://ocl.shangyingyoupin.top

SELECT * FROM users WHERE email IS NULL;
来源：http://asp.hysaishi.cn

[Q22] 排序
来源：http://dns.yuanzhike.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://auj.sufxvd.cn

[Q23] 分页
来源：http://yxs.jqgufenzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://syy.gaohongyu789.top

[Q24] 去重
来源：http://byo.jiagoushi.top

SELECT DISTINCT city FROM users;
来源：http://mmx.yuxming.cn

[Q25] 只取前 N 条
来源：http://ptl.sxryk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://knz.bbcook.cn

[Q26] 计数
来源：http://djg.nanxuanxn.top

SELECT COUNT(*) FROM users;
来源：http://hsu.hcnkem.com

[Q27] 条件计数
来源：http://djz.fktsv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vuu.52xcode.cn

[Q28] 求和与平均
来源：http://maa.aibaodan.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://plc.fzhhl.top

[Q29] 最大最小值
来源：http://zjg.c1oappe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vrg.zhijiandao.cn

[Q30] 分组统计
来源：http://oft.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wiy.xziqi.cn

[Q31] 分组后过滤
来源：http://mzo.dianchejie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tin.guowangkeji.top

[Q32] 分组拼接字符串
来源：http://qci.ctjpmb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hpf.xinyue.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iiy.haohaochexian.top

[Q33] 多列分组
来源：http://mvf.zhiwuduotai.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fhh.yuanzhike.top

[Q34] 每组取第一条
来源：http://fin.ydzc1.top

SELECT * FROM (
来源：http://mfp.zhongyouzk.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dgr.nanxinkj.top

) t WHERE rn = 1;
来源：http://voi.0kj1m.cn

[Q35] 内连接
来源：http://meo.gotoacloud.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zzh.aizwys.cn

[Q36] 左连接
来源：http://wgf.yvedp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dci.svipenyu.cn

[Q37] 右连接
来源：http://ftx.gzhubu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://frt.ehwqpu.com

[Q38] 全外连接（PostgreSQL）
来源：http://rop.yuanzhike.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jhk.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://grh.tarul.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bsq.fehbvm.com


<!-- 参考信息 -->