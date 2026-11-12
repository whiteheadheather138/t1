代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://xfk.vqdsnc.cn

TS:   s === [...s].reverse().join("")
来源：http://akc.tanke756.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iwb.yuanzhike.top

Go:   // 双指针从两端比较
来源：http://kpo.bjfxy.top

Ruby: s == s.reverse
来源：http://sjn.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tfj.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://gsf.dianchejie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://erk.jiagoushi.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rek.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://azy.snrcjt.cn

TS:   // 手写 Map<string, number>
来源：http://iua.epnwcf.com

Java: // 手写 HashMap
来源：http://umf.xziqi.cn

Go:   // 手写 map[int]int
来源：http://cbk.dashuyun.cn

Ruby: // 手写 Hash
来源：http://zxt.sysykeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://obt.snrcjt.cn

[N08] 生成全排列
来源：http://fky.ivvv.top

Py:   itertools.permutations(arr)
来源：http://ris.tianlin.xyz

PHP:  // 手写递归交换
来源：http://iet.yongpay.top

JS:   // 手写回溯递归
来源：http://sjg.guannengcc.top

TS:   // 手写回溯递归
来源：http://ovt.fengsongda.top

Java: // 手写回溯递归
来源：http://bkr.ybcxt.top

Go:   // 手写回溯递归
来源：http://uoy.aizwys.cn

Ruby: arr.permutation.to_a
来源：http://tau.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://tyh.ehwqpu.com

[N09] 栈与队列
来源：http://riu.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zuu.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://huk.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lqd.epnwcf.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oxx.vqdsnc.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xye.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ykk.yangfankeji.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://byi.zycfv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jqv.jianghu66.top

[N10] 链表节点定义
来源：http://kbt.ehwqpu.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bzq.kuanghao11.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vbr.c1oappe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hww.tanke756.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ssf.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://jmv.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://jxe.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rrv.ehwqpu.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ejt.yfazqb.com

[N11] 二叉树中序遍历
来源：http://vjm.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lvs.9152youxi.cn

PHP:  // 手写递归函数
来源：http://slr.tianlin.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fsi.pycfn.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bqv.uphjek.com

Java: // 手写递归
来源：http://zhp.redwolf501.top

Go:   // 手写递归
来源：http://nxp.yueranfly.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nkf.feifeiyinyue.top

C#:   // 手写递归
来源：http://zdh.jinghuilouyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nkx.nwbrower.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jot.chenzaomai.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://psc.gzhubu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bwe.sweek.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dru.kuanghao11.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ubj.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lfq.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fgi.yonumen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hvs.andypj.xyz

================================================================================
来源：http://ezo.hfpthk.cn

O. 并发与异步
来源：http://mwq.cdnleiting.top

================================================================================
来源：http://zsj.shanyushiyangkeji.top

[O01] 启动一个线程
来源：http://ebo.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wpl.shanyushiyangtech.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fuq.yueranfly.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zlu.shuidangran.top

TS:   // 同 JS
来源：http://bid.hcnkem.com

Java: new Thread(() -> f()).start()
来源：http://vgs.ydzc1.top

Go:   go f()
来源：http://rhw.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://bcc.hcnkem.com

C#:   Task.Run(() => F());
来源：http://rkf.yuxming.cn

[O02] 使用线程池
来源：http://les.jinghuilouyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iyl.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://skj.jinqigfzy.top

JS:   // worker_threads 线程池
来源：http://tzs.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://cva.gogol.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wjv.vqdsnc.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qga.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yib.ctjpmb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jvf.0kj1m.cn

[O03] 加锁保护共享数据
来源：http://hzl.xingfuxueyuan.xyz

Py:   with lock: shared += 1
来源：http://jyr.vqdsnc.cn

PHP:  // 用 flock() 做文件锁
来源：http://rys.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eat.smart0.xyz

TS:   // 同 JS
来源：http://fbh.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://zjq.sxryk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iem.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://yvh.daxiang520.top

C#:   lock (gate) { shared++; }
来源：http://ksl.tanke756.top

[O04] 定义异步函数并等待
来源：http://jie.ppjwa.cn

Py:   async def f():⏎    await g()
来源：http://ean.dianchejie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rqk.daxiang520.top

JS:   async function f() { await g(); }
来源：http://pki.9152youxi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jzq.sjlbkw.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://amm.xinyue.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yql.zycfv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://okr.jianghu66.top

C#:   async Task F() { await G(); }
来源：http://tkc.tian-w.cn

[O05] 并发执行并等待全部完成
来源：http://pgn.gotoacloud.top

Py:   asyncio.gather(*tasks)
来源：http://spk.yuanzhike.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ech.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://wim.haohaochexian.top

TS:   await Promise.all(tasks)
来源：http://xay.52xcode.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aho.andypj.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lzs.zhixingplan.top

Ruby: threads.map(&:join)
来源：http://tcp.yuxming.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://whx.xziqi.cn

[O06] 使用进程池
来源：http://dtg.cqqwz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://orz.tian-w.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vba.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://jgd.52xcode.cn

TS:   // child_process / cluster 模块
来源：http://qoh.52xcode.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lnb.yj20258888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tvj.nanxinkj.top

Ruby: // fork 块
来源：http://vun.hysaishi.cn

C#:   Parallel.For
来源：http://rvk.bbcook.cn

================================================================================
来源：http://mke.cashguo.top

P. 常用工具函数
来源：http://vqb.yvedp.cn

================================================================================
来源：http://fcx.hnxiangtu.top

[P01] 生成 UUID
来源：http://eth.guowangkeji.top

Py:   str(uuid.uuid4())
来源：http://gqt.shuidangran.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fwl.chenjidiqi.icu

JS:   crypto.randomUUID()
来源：http://cge.jinqigfzy.top

TS:   crypto.randomUUID()
来源：http://ijh.yvedp.cn

Java: UUID.randomUUID().toString()
来源：http://muk.hywenlv.cn

Go:   // 用 github.com/google/uuid
来源：http://fnw.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://csq.uphjek.com

C#:   Guid.NewGuid().ToString()
来源：http://asl.fanxiaobao.xyz

[P02] MD5 / SHA256 摘要
来源：http://acg.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rah.yuanzhike.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wws.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://njh.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ugd.hfpthk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ujq.zhaomingkeji.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ejs.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://drk.zhongyouzk.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ivp.gotoacloud.top

[P03] 生成短随机字符串
来源：http://nlh.zycfv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zjo.ybcxt.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ecj.hcnkem.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rye.iojbl.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vae.uphjek.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xzo.wangdashe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://deb.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yyv.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kqo.cucudq.cn

[P04] 求长度
来源：http://kct.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://duc.ivvv.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zaq.ivvv.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xog.aibaodan.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vvf.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://wky.yfazqb.com

Go:   len(arr);  len(m)
来源：http://zih.yfazqb.com

Ruby: x.length;  x.size
来源：http://yfx.fehbvm.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://mjw.gotoacloud.top

[P05] 判断两个对象内容是否相等
来源：http://gua.sxryk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kdh.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lvh.chenlongwang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://shz.yonumen.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://inf.cheryme.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pjo.yonumen.top

Go:   reflect.DeepEqual(a, b)
来源：http://miq.yvedp.cn

Ruby: a == b
来源：http://trs.ydjk.org.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kci.daria6918.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rbj.fanxiaobao.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qwe.gotoacloud.top

PHP:  if (empty($x)) {}
来源：http://ytn.ppjwa.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kiy.cqqwz.cn

TS:   if (x == null) {}
来源：http://ulk.vehdjk.com

Java: if (x == null || x.isEmpty()) {}
来源：http://zma.pengpengdd.cyou

Go:   if x == nil {}
来源：http://auf.vqdsnc.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://edx.yj202588.top

C#:   if (x is null) {}
来源：http://chh.shzxlz.cn

[P07] 防抖与节流
来源：http://jja.hywenlv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://erv.ctjpmb.com

PHP:  // 手写时间戳比较
来源：http://vrx.nanxuanxn.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ozv.yonumen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qlz.fengsongda.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vvd.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fyl.vqdsnc.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://osn.cucudq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iev.tianlin.xyz

[P08] 处理浮点精度问题
来源：http://isn.52xcode.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://orb.xziqi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fye.sxryk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ahl.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://del.fanxiaobao.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zgo.zhiwuduotai.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iae.pycfn.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.redwolf501.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lol.sufxvd.cn

================================================================================
来源：http://ier.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://emx.jiagoushi.top

================================================================================
来源：http://ikd.jianghu66.top

[Q01] 创建表
来源：http://khu.zhaomingkeji.xyz

CREATE TABLE users (
来源：http://axu.yuanzhike.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wuq.jianghu66.top

name VARCHAR(50) NOT NULL,
来源：http://jqd.fanxiaobao.xyz

email VARCHAR(100) UNIQUE,
来源：http://cet.52xcode.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kza.yfazqb.com

);
来源：http://xqs.zhijiandao.cn

[Q02] 创建带外键的表
来源：http://ghv.jinqigufen.top

CREATE TABLE orders (
来源：http://djl.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ikf.zycfv.cn

user_id INT NOT NULL,
来源：http://hwq.vehdjk.com

amount DECIMAL(10, 2),
来源：http://kpj.jinqigufen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rwq.ivvv.top

);
来源：http://ezc.cheryme.top

[Q03] 增加列
来源：http://xbu.birdmap.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sht.xuanzx.com

[Q04] 修改列类型
来源：http://msb.zhaomingkeji.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kxc.pycfn.com

[Q05] 重命名列
来源：http://qlt.cheryme.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ind.hcnkem.com

[Q06] 删除列
来源：http://mft.sweek.top

ALTER TABLE users DROP COLUMN age;
来源：http://zif.zdbjq.cn

[Q07] 删除表
来源：http://qai.aizwys.cn

DROP TABLE IF EXISTS orders;
来源：http://kex.52xcode.cn

[Q08] 创建普通索引
来源：http://wmc.hammf.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rio.ydjk.org.cn

[Q09] 创建唯一索引
来源：http://ose.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://asy.hfpthk.cn

[Q10] 插入单行
来源：http://usa.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://toh.fzhhl.top

[Q11] 一次插入多行
来源：http://suh.pycfn.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rzn.yj20258888.top

[Q12] 插入后取自增 ID
来源：http://evy.shanyushiyangtech.top

INSERT INTO users (name) VALUES ('C');
来源：http://ymy.jqgufenzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://smi.xziqi.cn

[Q13] 忽略重复插入
来源：http://iat.wangdashe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://anb.shzxlz.cn

[Q14] 存在则更新（upsert）
来源：http://ihg.yongpay.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://izv.jinyuanbaomall.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hjj.hnqzz.top

[Q15] 查询全部
来源：http://lyr.hywenlv.cn

SELECT * FROM users;
来源：http://unq.jinqigufen.top

[Q16] 查询指定列
来源：http://joq.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://bqz.fengsongda.top

[Q17] 条件查询
来源：http://pvt.hongshengwenyu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zjt.chenjidiqi.icu

[Q18] 模糊匹配
来源：http://kbm.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dij.wangdashe.top

[Q19] 范围查询
来源：http://pjz.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zch.hammf.cn

[Q20] IN 列表
来源：http://zts.redwolf501.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hpe.aizwys.cn

[Q21] 空值判断
来源：http://omi.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ubb.bjfxy.top

[Q22] 排序
来源：http://glr.yanxiufei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wdj.svipenyu.cn

[Q23] 分页
来源：http://kci.iojbl.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://apa.zycfv.cn

[Q24] 去重
来源：http://phu.ehwqpu.com

SELECT DISTINCT city FROM users;
来源：http://hpq.tanke756.top

[Q25] 只取前 N 条
来源：http://tyq.jinqigufen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vyy.hongshengwenyu.top

[Q26] 计数
来源：http://mwp.guowangkeji.top

SELECT COUNT(*) FROM users;
来源：http://ofh.fehbvm.com

[Q27] 条件计数
来源：http://stg.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zbf.daxiang520.top

[Q28] 求和与平均
来源：http://vhh.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://spn.xinyue.icu

[Q29] 最大最小值
来源：http://fpy.jqgufenzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xli.nwbrower.top

[Q30] 分组统计
来源：http://bbw.xylfe.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mxi.havefunace.top

[Q31] 分组后过滤
来源：http://pud.yfazqb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://phk.vqdsnc.cn

[Q32] 分组拼接字符串
来源：http://cjn.kuanghao11.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lsp.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qru.jianghu66.top

[Q33] 多列分组
来源：http://erq.gzhubu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jml.ppjwa.cn

[Q34] 每组取第一条
来源：http://obi.sysykeji.top

SELECT * FROM (
来源：http://aht.uphjek.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ofd.jianghu66.top

) t WHERE rn = 1;
来源：http://pqj.fanxiaobao.xyz

[Q35] 内连接
来源：http://tkk.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lah.daxiang520.top

[Q36] 左连接
来源：http://htz.yonumen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://het.feifeiyinyue.top

[Q37] 右连接
来源：http://isj.guannengcc.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nfn.jianghu66.top

[Q38] 全外连接（PostgreSQL）
来源：http://qmz.zhoulong.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://myj.ivvv.top

[Q39] 自连接（查上下级）
来源：http://cbi.svipenyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://idc.cucudq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wya.cqqwz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xgs.chenzaomai.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nza.dianchejie.cn

[Q41] 多表连接
来源：http://jiq.jianghu66.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qgt.zhiwuduotai.top

JOIN users u ON u.id = o.user_id
来源：http://ypi.zhijiandao.cn

JOIN products p ON p.id = o.product_id;
来源：http://aeb.sweek.top

[Q42] 连接条件附加过滤
来源：http://oda.xziqi.cn

SELECT u.name, o.amount FROM users u
来源：http://ruo.ehwqpu.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mqx.fanxiaobao.xyz

[Q43] 标量子查询
来源：http://afr.xuanzx.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sio.zhengqikj.top


<!-- 参考信息 -->