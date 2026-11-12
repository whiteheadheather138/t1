代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wdr.feifeiyinyue.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://esz.daxiang520.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dbj.smart0.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ovf.ehwqpu.com

[N05] 最大公约数
来源：http://hst.fehbvm.com

Py:   math.gcd(a, b)
来源：http://ijy.yj20258.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ccs.fanxiaobao.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pqb.gzhubu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eyg.gotoacloud.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://adj.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qdp.yonumen.top

Ruby: a.gcd(b)
来源：http://tqw.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rpm.shanyushiyangkeji.top

[N06] 判断回文字符串
来源：http://lkb.zdbjq.cn

Py:   s == s[::-1]
来源：http://fhy.uphjek.com

PHP:  $s === strrev($s);
来源：http://jaw.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://udt.zhixingplan.top

TS:   s === [...s].reverse().join("")
来源：http://nwn.meibo888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ovq.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://wpw.shangyingyoupin.top

Ruby: s == s.reverse
来源：http://iuq.nwbrower.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rqt.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://ntj.zhengqikj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oxa.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hyi.52xcode.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rpf.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://jgy.xuetiantiany.cn

Java: // 手写 HashMap
来源：http://gss.zhiwuduotai.top

Go:   // 手写 map[int]int
来源：http://pxc.fzhhl.top

Ruby: // 手写 Hash
来源：http://ptd.zdbjq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gfw.xylfe.cn

[N08] 生成全排列
来源：http://sgv.yangfankeji.com

Py:   itertools.permutations(arr)
来源：http://cnt.tarul.cn

PHP:  // 手写递归交换
来源：http://bil.daria6918.cn

JS:   // 手写回溯递归
来源：http://dyl.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://knz.52xcode.cn

Java: // 手写回溯递归
来源：http://vzr.meibo888.top

Go:   // 手写回溯递归
来源：http://zsl.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://rkt.shzxlz.cn

C#:   // 手写回溯递归
来源：http://pny.yj20258888.top

[N09] 栈与队列
来源：http://ysc.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ltj.aibaodan.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xdk.zycfv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dxl.gaohongyu789.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bov.tianlin.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cxl.hysaishi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jhs.yuxming.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kqu.yfazqb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nwm.cheryme.top

[N10] 链表节点定义
来源：http://xia.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qnm.iojbl.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vum.chenlongwang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kvq.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pbj.jinghuilouyu.cn

Java: class Node { int v; Node next; }
来源：http://stj.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://vqz.haohaochexian.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uar.zhijiandao.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vdg.fanxiaobao.xyz

[N11] 二叉树中序遍历
来源：http://ifu.c1oappe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uqb.epnwcf.com

PHP:  // 手写递归函数
来源：http://zie.wangdashe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aaw.shuidangran.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mat.zhiwuduotai.top

Java: // 手写递归
来源：http://mqb.ehwqpu.com

Go:   // 手写递归
来源：http://ccb.tian-w.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://otb.zycfv.cn

C#:   // 手写递归
来源：http://kae.yongpay.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gtg.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qzl.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yha.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://npc.kuanghao11.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cys.daria6918.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ufw.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pok.dashuyun.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jyv.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://afn.bbcook.cn

================================================================================
来源：http://jpx.9152youxi.cn

O. 并发与异步
来源：http://lcb.xingfuxueyuan.xyz

================================================================================
来源：http://gfq.xuetiantiany.cn

[O01] 启动一个线程
来源：http://zku.yfazqb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ogx.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xzv.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nlk.hnqzz.top

TS:   // 同 JS
来源：http://jwd.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://pop.zhongyouzk.top

Go:   go f()
来源：http://ykw.ppjwa.cn

Ruby: Thread.new { f }
来源：http://ydr.chenjidiqi.icu

C#:   Task.Run(() => F());
来源：http://jbl.vqdsnc.cn

[O02] 使用线程池
来源：http://muz.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qjd.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pxf.gotoacloud.top

JS:   // worker_threads 线程池
来源：http://xkl.yj202588.top

TS:   // worker_threads 线程池
来源：http://rbs.jinqigufen.top

Java: Executors.newFixedThreadPool(4)
来源：http://jug.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pgw.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wsw.yongpay.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tse.ydzc1.top

[O03] 加锁保护共享数据
来源：http://tcx.tarul.cn

Py:   with lock: shared += 1
来源：http://phv.yj202588.top

PHP:  // 用 flock() 做文件锁
来源：http://ttx.shzxlz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://brw.nanxinkj.top

TS:   // 同 JS
来源：http://nai.52xcode.cn

Java: synchronized (this) { shared++; }
来源：http://xou.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oig.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://vxw.quarkkingdee.top

C#:   lock (gate) { shared++; }
来源：http://nqi.ctjpmb.com

[O04] 定义异步函数并等待
来源：http://oza.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://vhs.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ewo.9152youxi.cn

JS:   async function f() { await g(); }
来源：http://ace.hesvh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lnp.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cxd.fehbvm.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rce.jyoumei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dzx.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://vvi.fengsongda.top

[O05] 并发执行并等待全部完成
来源：http://xtb.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://jrw.jinyuanbaomall.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fno.guannengcc.top

JS:   await Promise.all(tasks)
来源：http://fge.ppjwa.cn

TS:   await Promise.all(tasks)
来源：http://xmk.yvedp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pgk.cqqwz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jfj.hysaishi.cn

Ruby: threads.map(&:join)
来源：http://lnw.0kj1m.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ofz.gogol.net.cn

[O06] 使用进程池
来源：http://pif.fengsongda.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fhb.jiagoushi.top

PHP:  // pcntl_fork 或多进程队列
来源：http://iut.yuxming.cn

JS:   // child_process / cluster 模块
来源：http://ime.sweek.top

TS:   // child_process / cluster 模块
来源：http://wzz.birdmap.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://giu.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gfw.kuanghao11.cn

Ruby: // fork 块
来源：http://nrb.yj20258.top

C#:   Parallel.For
来源：http://yme.jqgfzy.top

================================================================================
来源：http://hcq.tanke756.top

P. 常用工具函数
来源：http://pyz.shangyingyoupin.top

================================================================================
来源：http://uxa.sysykeji.top

[P01] 生成 UUID
来源：http://oax.birdmap.top

Py:   str(uuid.uuid4())
来源：http://ldm.jqgufenzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vcx.cqqwz.cn

JS:   crypto.randomUUID()
来源：http://jby.bbcook.cn

TS:   crypto.randomUUID()
来源：http://bld.tanke756.top

Java: UUID.randomUUID().toString()
来源：http://vja.ctjpmb.com

Go:   // 用 github.com/google/uuid
来源：http://jzs.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://mft.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://llm.haohaochexian.top

[P02] MD5 / SHA256 摘要
来源：http://asf.pycfn.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gcq.zhiwuduotai.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dzg.vqdsnc.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mun.snrcjt.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nnk.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://utj.hnqzz.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://afn.ppjwa.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qck.yfazqb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ibi.hnqzz.top

[P03] 生成短随机字符串
来源：http://qug.zhiwuduotai.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ark.mhx1999.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oud.zhoulong.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yea.pycfn.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ifw.nanxinkj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lud.yfazqb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zda.birdmap.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gyu.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nlf.zhoulong.xyz

[P04] 求长度
来源：http://nal.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://equ.ywan-chungtsiang.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mkd.cheryme.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pvj.daria6918.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://muo.jinghuilouyu.cn

Java: list.size();  map.size();  s.length()
来源：http://xbp.meibo888.top

Go:   len(arr);  len(m)
来源：http://mgz.sysykeji.top

Ruby: x.length;  x.size
来源：http://cyl.jinqigfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hho.zhiwuduotai.top

[P05] 判断两个对象内容是否相等
来源：http://lzh.zdbjq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lha.yanxiufei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://emm.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://efh.guannengcc.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bnt.meibo888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zxv.shzxlz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mqn.yj202588.top

Ruby: a == b
来源：http://jiq.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ybt.9152youxi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dtf.jinqigufen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tii.nwbrower.top

PHP:  if (empty($x)) {}
来源：http://yfq.cashguo.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kfu.nanxinkj.top

TS:   if (x == null) {}
来源：http://rth.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nqa.iojbl.cn

Go:   if x == nil {}
来源：http://tif.xuetiantiany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://prw.birdmap.top

C#:   if (x is null) {}
来源：http://gsu.hnxiangtu.top

[P07] 防抖与节流
来源：http://xyn.kuanghao11.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kym.vqdsnc.cn

PHP:  // 手写时间戳比较
来源：http://kyl.havefunace.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blq.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eff.wangdashe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lfh.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hjd.zhijiandao.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ycz.ydjk.org.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vrh.nanxuanxn.top

[P08] 处理浮点精度问题
来源：http://yqc.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zck.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gkt.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ajg.yangfankeji.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sdl.jiagoushi.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eni.ehwqpu.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lsr.hywenlv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fyz.meibo888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kdh.havefunace.top

================================================================================
来源：http://adu.xuetiantiany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oju.gzhubu.top

================================================================================
来源：http://cxl.yj20258888.top

[Q01] 创建表
来源：http://nuv.shzxlz.cn

CREATE TABLE users (
来源：http://olw.chenzaomai.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qro.jinyuanbaomall.cn

name VARCHAR(50) NOT NULL,
来源：http://hnh.zhengqikj.top

email VARCHAR(100) UNIQUE,
来源：http://rdg.xylfe.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://had.nanxinkj.top

);
来源：http://qjc.yonumen.top

[Q02] 创建带外键的表
来源：http://ypa.zhixingplan.top

CREATE TABLE orders (
来源：http://aut.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yqw.aizwys.cn

user_id INT NOT NULL,
来源：http://mov.tian-w.cn

amount DECIMAL(10, 2),
来源：http://gha.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rnd.zhaomingkeji.xyz

);
来源：http://vlq.tianlin.xyz

[Q03] 增加列
来源：http://hmm.birdmap.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qob.quarkkingdee.top

[Q04] 修改列类型
来源：http://ith.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qnh.cashguo.top

[Q05] 重命名列
来源：http://glh.yuxming.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ugu.fehbvm.com

[Q06] 删除列
来源：http://rdv.chenjidiqi.icu

ALTER TABLE users DROP COLUMN age;
来源：http://wyd.tian-w.cn

[Q07] 删除表
来源：http://gyb.kuanghao11.cn

DROP TABLE IF EXISTS orders;
来源：http://whc.birdmap.top

[Q08] 创建普通索引
来源：http://med.pycfn.com

CREATE INDEX idx_users_email ON users(email);
来源：http://gxc.meibo888.top

[Q09] 创建唯一索引
来源：http://wzs.316326.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://akx.zhoulong.xyz

[Q10] 插入单行
来源：http://dlm.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mus.nanxinkj.top

[Q11] 一次插入多行
来源：http://gac.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dil.cheryme.top

[Q12] 插入后取自增 ID
来源：http://xqf.gogol.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dpg.mhx1999.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rez.yangfankeji.com

[Q13] 忽略重复插入
来源：http://dvf.yonumen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vew.andypj.xyz

[Q14] 存在则更新（upsert）
来源：http://lxh.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bcr.hcnkem.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nkq.zhixingplan.top

[Q15] 查询全部
来源：http://xnt.fanxiaobao.xyz

SELECT * FROM users;
来源：http://tul.sufxvd.cn

[Q16] 查询指定列
来源：http://ouq.zhixingplan.top

SELECT id, name FROM users;
来源：http://zxu.sjlbkw.cn

[Q17] 条件查询
来源：http://nar.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bfk.daxiang520.top

[Q18] 模糊匹配
来源：http://xal.chenlongwang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jcp.shanyushiyangtech.top

[Q19] 范围查询
来源：http://grx.yonumen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yqf.havefunace.top

[Q20] IN 列表
来源：http://von.gaohongyu789.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zic.bbcook.cn

[Q21] 空值判断
来源：http://dsk.ivvv.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gni.jinqigufen.top

[Q22] 排序
来源：http://vdl.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xdj.fanxiaobao.xyz

[Q23] 分页
来源：http://bon.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lgp.zhijiandao.cn

[Q24] 去重
来源：http://lfg.guannengcc.top

SELECT DISTINCT city FROM users;
来源：http://zzm.redwolf501.top

[Q25] 只取前 N 条
来源：http://had.hysaishi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fqn.chenlongwang.top

[Q26] 计数
来源：http://yrc.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://vcl.zhaomingkeji.xyz

[Q27] 条件计数
来源：http://uyh.ydjk.org.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jec.cqqwz.cn

[Q28] 求和与平均
来源：http://zbl.c1oappe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yzr.hywenlv.cn

[Q29] 最大最小值
来源：http://efu.mhx1999.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://toc.316326.xyz

[Q30] 分组统计
来源：http://bek.hesvh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tsj.zhixingplan.top

[Q31] 分组后过滤
来源：http://zsm.hnxiangtu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dib.ywan-chungtsiang.top

[Q32] 分组拼接字符串
来源：http://hgy.snrcjt.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mtr.yj20258.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rsk.zhongyouzk.top

[Q33] 多列分组
来源：http://ihu.cqqwz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bdx.tian-w.cn

[Q34] 每组取第一条
来源：http://fmj.snrcjt.cn

SELECT * FROM (
来源：http://mfq.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fhk.jlsjyb.cn

) t WHERE rn = 1;
来源：http://fae.xuetiantiany.cn

[Q35] 内连接
来源：http://csr.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pcm.dianchejie.cn

[Q36] 左连接
来源：http://pvw.feifeiyinyue.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://odb.andypj.xyz

[Q37] 右连接
来源：http://fxh.snrcjt.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gnd.yanxiufei.cn


<!-- 参考信息 -->