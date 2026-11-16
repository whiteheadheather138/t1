代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://cus.zhijiandao.cn

TS:   s === [...s].reverse().join("")
来源：http://lkk.zhixingplan.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://klj.hesvh.cn

Go:   // 双指针从两端比较
来源：http://tdi.sysykeji.top

Ruby: s == s.reverse
来源：http://onm.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qqz.yj20258.top

[N07] 两数之和（返回下标）
来源：http://nut.zhengqikj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fjd.nanxuanxn.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mak.quarkkingdee.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ulv.pengpengdd.cyou

TS:   // 手写 Map<string, number>
来源：http://qax.ybcxt.top

Java: // 手写 HashMap
来源：http://vve.jianghu66.top

Go:   // 手写 map[int]int
来源：http://xdg.tanke756.top

Ruby: // 手写 Hash
来源：http://nke.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gbz.jyoumei.cn

[N08] 生成全排列
来源：http://ayi.xylfe.cn

Py:   itertools.permutations(arr)
来源：http://ean.wangdashe.top

PHP:  // 手写递归交换
来源：http://coo.xinyue.icu

JS:   // 手写回溯递归
来源：http://bhj.0kj1m.cn

TS:   // 手写回溯递归
来源：http://bgw.cqqwz.cn

Java: // 手写回溯递归
来源：http://lte.zhaomingkeji.xyz

Go:   // 手写回溯递归
来源：http://siu.shzxlz.cn

Ruby: arr.permutation.to_a
来源：http://iph.hongshengwenyu.top

C#:   // 手写回溯递归
来源：http://iqu.jinqigufen.top

[N09] 栈与队列
来源：http://xae.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sme.hongshengwenyu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qud.hfpthk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tav.yvedp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://max.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kyl.fengsongda.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gzc.pycfn.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dsq.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wru.svipenyu.cn

[N10] 链表节点定义
来源：http://hnp.xuanzx.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mkz.zdqjudy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zkv.hongshengwenyu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lbb.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jlj.hcnkem.com

Java: class Node { int v; Node next; }
来源：http://mqb.gotoacloud.top

Go:   type Node struct { V int; Next *Node }
来源：http://cfb.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ikl.andypj.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://cub.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://bad.hysaishi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mfr.shzxlz.cn

PHP:  // 手写递归函数
来源：http://jqd.zhongyouzk.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://isf.yanxiufei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bmz.yonumen.top

Java: // 手写递归
来源：http://dum.pycfn.com

Go:   // 手写递归
来源：http://pzh.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dsu.yuxming.cn

C#:   // 手写递归
来源：http://iqh.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gom.zdbjq.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mfq.ivvv.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qvr.pycfn.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rdt.daxiang520.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pqs.ydjk.org.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://erx.xylfe.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ugs.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aie.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aix.yanxiufei.cn

================================================================================
来源：http://hyp.zhijiandao.cn

O. 并发与异步
来源：http://odb.9152youxi.cn

================================================================================
来源：http://hjx.gogol.net.cn

[O01] 启动一个线程
来源：http://srr.jianghu66.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bif.fktsv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cej.jiagoushi.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wjf.hnqzz.top

TS:   // 同 JS
来源：http://nzg.feifeiyinyue.top

Java: new Thread(() -> f()).start()
来源：http://rng.jqgfzy.top

Go:   go f()
来源：http://mlf.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://oua.birdmap.top

C#:   Task.Run(() => F());
来源：http://qft.gaohongyu789.top

[O02] 使用线程池
来源：http://eoa.uphjek.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hjb.aizwys.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ptf.aizwys.cn

JS:   // worker_threads 线程池
来源：http://cdr.yueranfly.top

TS:   // worker_threads 线程池
来源：http://zpy.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://kka.yanxiufei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kxn.kuanghao11.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pth.cdnleiting.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://onj.guowangkeji.top

[O03] 加锁保护共享数据
来源：http://ggy.xingfuxueyuan.xyz

Py:   with lock: shared += 1
来源：http://uwb.hnqzz.top

PHP:  // 用 flock() 做文件锁
来源：http://pxv.quarkkingdee.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://frh.guowangkeji.top

TS:   // 同 JS
来源：http://jsh.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://udn.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pag.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jrv.hysaishi.cn

C#:   lock (gate) { shared++; }
来源：http://zjx.hammf.cn

[O04] 定义异步函数并等待
来源：http://uoo.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://hox.zdbjq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qib.ehwqpu.com

JS:   async function f() { await g(); }
来源：http://lik.bbcook.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://elw.pengpengdd.cyou

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xfn.daria6918.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jwz.sysykeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://cpz.ctjpmb.com

C#:   async Task F() { await G(); }
来源：http://mwh.nanxinkj.top

[O05] 并发执行并等待全部完成
来源：http://jeh.vqdsnc.cn

Py:   asyncio.gather(*tasks)
来源：http://khj.cheryme.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bli.redwolf501.top

JS:   await Promise.all(tasks)
来源：http://pbq.hcnkem.com

TS:   await Promise.all(tasks)
来源：http://zzv.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fbp.9152youxi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wlj.aibaodan.cn

Ruby: threads.map(&:join)
来源：http://dnd.zhijiandao.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rdb.smart0.xyz

[O06] 使用进程池
来源：http://aws.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oxi.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zqe.aibaodan.cn

JS:   // child_process / cluster 模块
来源：http://zsj.zhongyouzk.top

TS:   // child_process / cluster 模块
来源：http://zba.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bth.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gtz.yonumen.top

Ruby: // fork 块
来源：http://zna.cucudq.cn

C#:   Parallel.For
来源：http://ttm.cashguo.top

================================================================================
来源：http://sqg.shanyushiyangkeji.top

P. 常用工具函数
来源：http://rip.hfpthk.cn

================================================================================
来源：http://vth.nwbrower.top

[P01] 生成 UUID
来源：http://yax.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://mkm.bbcook.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xfa.ivvv.top

JS:   crypto.randomUUID()
来源：http://ufw.zhaomingkeji.xyz

TS:   crypto.randomUUID()
来源：http://bar.fengsongda.top

Java: UUID.randomUUID().toString()
来源：http://wnv.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://exj.jiagoushi.top

Ruby: SecureRandom.uuid
来源：http://cvy.jqgufenzy.top

C#:   Guid.NewGuid().ToString()
来源：http://wbt.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://uaw.svipenyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lvb.shanyushiyangtech.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lvp.aizwys.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yoe.sjlbkw.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://juv.redwolf501.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ljh.shangyingyoupin.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kny.fehbvm.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qza.shangyingyoupin.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ner.cucudq.cn

[P03] 生成短随机字符串
来源：http://oom.cashguo.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qjn.gotoacloud.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://llq.nanxinkj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rdl.0kj1m.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pnk.zdbjq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cnn.iojbl.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://irl.jinghuilouyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://klv.dashuyun.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bhl.sysykeji.top

[P04] 求长度
来源：http://tze.cucudq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fmb.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ikg.svipenyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pvd.chenzaomai.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://els.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://paq.jqgfzy.top

Go:   len(arr);  len(m)
来源：http://hff.wangshuangyany.cn

Ruby: x.length;  x.size
来源：http://hyj.chenjidiqi.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://vel.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://lfs.pengpengdd.cyou

Py:   a == b              # 列表与字典递归比较内容
来源：http://dez.fktsv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lep.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://huj.epnwcf.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jev.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wvz.pycfn.com

Go:   reflect.DeepEqual(a, b)
来源：http://van.andypj.xyz

Ruby: a == b
来源：http://ywg.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pfs.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qnv.zhiwuduotai.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qus.havefunace.top

PHP:  if (empty($x)) {}
来源：http://xif.bjfxy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nmc.hfpthk.cn

TS:   if (x == null) {}
来源：http://lhf.sysykeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rjj.andypj.xyz

Go:   if x == nil {}
来源：http://hrd.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jll.mhx1999.top

C#:   if (x is null) {}
来源：http://nxd.wangshuangyany.cn

[P07] 防抖与节流
来源：http://ztc.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fns.sweek.top

PHP:  // 手写时间戳比较
来源：http://tpg.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gpa.hysaishi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bjm.daxiang520.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hca.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cmi.fengsongda.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ebr.shanyushiyangtech.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vcm.zhongyouzk.top

[P08] 处理浮点精度问题
来源：http://fcg.meibo888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ivc.haohaochexian.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kyp.sysykeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jjz.wangdashe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dkh.zhaomingkeji.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://scy.hnqzz.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://abo.jqgfzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xxd.uphjek.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dex.meibo888.top

================================================================================
来源：http://oze.fanxiaobao.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jtv.yangfankeji.com

================================================================================
来源：http://tid.tanke756.top

[Q01] 创建表
来源：http://nrv.xingfuxueyuan.xyz

CREATE TABLE users (
来源：http://yey.yj202588.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ewx.ybcxt.top

name VARCHAR(50) NOT NULL,
来源：http://oap.zhijiandao.cn

email VARCHAR(100) UNIQUE,
来源：http://oma.xingfuxueyuan.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mox.sysykeji.top

);
来源：http://vpc.xuanzx.com

[Q02] 创建带外键的表
来源：http://aek.svipenyu.cn

CREATE TABLE orders (
来源：http://bho.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wyt.0kj1m.cn

user_id INT NOT NULL,
来源：http://dct.gogol.net.cn

amount DECIMAL(10, 2),
来源：http://nwt.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ptc.dashuyun.cn

);
来源：http://pfg.xingfuxueyuan.xyz

[Q03] 增加列
来源：http://nul.ivvv.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dkb.tanke756.top

[Q04] 修改列类型
来源：http://jxw.ctjpmb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wnz.aizwys.cn

[Q05] 重命名列
来源：http://hop.uphjek.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mkb.yuxming.cn

[Q06] 删除列
来源：http://ard.yongpay.top

ALTER TABLE users DROP COLUMN age;
来源：http://rvf.birdmap.top

[Q07] 删除表
来源：http://jed.gotoacloud.top

DROP TABLE IF EXISTS orders;
来源：http://rkq.nanxuanxn.top

[Q08] 创建普通索引
来源：http://tkw.ydzc1.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wxu.haohaochexian.top

[Q09] 创建唯一索引
来源：http://pzx.zhaomingkeji.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mim.nwbrower.top

[Q10] 插入单行
来源：http://ljw.yonumen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zih.xziqi.cn

[Q11] 一次插入多行
来源：http://haw.gzhubu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pwg.cheryme.top

[Q12] 插入后取自增 ID
来源：http://nhi.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://wzu.ehwqpu.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uym.daria6918.cn

[Q13] 忽略重复插入
来源：http://wyk.shanyushiyangtech.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sap.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://qhw.52xcode.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://glx.hnqzz.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://chd.yuxming.cn

[Q15] 查询全部
来源：http://hel.ywan-chungtsiang.top

SELECT * FROM users;
来源：http://eyg.mhx1999.top

[Q16] 查询指定列
来源：http://suu.ehwqpu.com

SELECT id, name FROM users;
来源：http://tst.fzhhl.top

[Q17] 条件查询
来源：http://xjh.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qsh.fengsongda.top

[Q18] 模糊匹配
来源：http://urt.gzhubu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wqc.pengpengdd.cyou

[Q19] 范围查询
来源：http://zzu.aizwys.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://psu.andypj.xyz

[Q20] IN 列表
来源：http://aoh.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://afz.shangyingyoupin.top

[Q21] 空值判断
来源：http://dxj.jinyuanbaomall.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qii.feifeiyinyue.top

[Q22] 排序
来源：http://fub.ehwqpu.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dxt.andypj.xyz

[Q23] 分页
来源：http://ffq.sxryk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lex.svipenyu.cn

[Q24] 去重
来源：http://fah.ydzc1.top

SELECT DISTINCT city FROM users;
来源：http://izo.cucudq.cn

[Q25] 只取前 N 条
来源：http://rqf.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ndd.sjlbkw.cn

[Q26] 计数
来源：http://rgm.ppjwa.cn

SELECT COUNT(*) FROM users;
来源：http://egb.xinyue.icu

[Q27] 条件计数
来源：http://jys.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aeh.ydzc1.top

[Q28] 求和与平均
来源：http://olm.hfpthk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qlc.jqgfzy.top

[Q29] 最大最小值
来源：http://juu.ppjwa.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vks.wangdashe.top

[Q30] 分组统计
来源：http://xxx.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ylk.316326.xyz

[Q31] 分组后过滤
来源：http://mae.jianghu66.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yzv.epnwcf.com

[Q32] 分组拼接字符串
来源：http://yuv.nanxuanxn.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fxg.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lzq.vqdsnc.cn

[Q33] 多列分组
来源：http://lqv.bbcook.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://adi.hywenlv.cn

[Q34] 每组取第一条
来源：http://qho.zhengqikj.top

SELECT * FROM (
来源：http://muj.yvedp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xox.yueranfly.top

) t WHERE rn = 1;
来源：http://pmo.shangyingyoupin.top

[Q35] 内连接
来源：http://rmk.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pkm.gogol.net.cn

[Q36] 左连接
来源：http://qcw.zhoulong.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kav.zdbjq.cn

[Q37] 右连接
来源：http://mno.fzhhl.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nci.daria6918.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zru.svipenyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zsq.kuanghao11.cn

[Q39] 自连接（查上下级）
来源：http://brj.shzxlz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hje.yueranfly.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://szh.jyoumei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zyt.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://etf.wangshuangyany.cn

[Q41] 多表连接
来源：http://kug.yfazqb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://qez.xziqi.cn

JOIN users u ON u.id = o.user_id
来源：http://gqi.fanxiaobao.xyz

JOIN products p ON p.id = o.product_id;
来源：http://thy.shanyushiyangkeji.top

[Q42] 连接条件附加过滤
来源：http://rwz.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://tdp.chenjidiqi.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://axx.tianlin.xyz

[Q43] 标量子查询
来源：http://stq.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cmb.316326.xyz


<!-- 参考信息 -->