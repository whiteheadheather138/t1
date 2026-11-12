代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bgx.pycfn.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tan.cdnleiting.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qxs.yongpay.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://alz.fehbvm.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xdy.cheryme.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ihr.yfazqb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kth.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rdi.meibo888.top

[N05] 最大公约数
来源：http://uoa.hcnkem.com

Py:   math.gcd(a, b)
来源：http://ozy.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hdl.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lez.wangdashe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pco.kuanghao11.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vko.fktsv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://loz.svipenyu.cn

Ruby: a.gcd(b)
来源：http://lyo.daria6918.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nqe.jqgfzy.top

[N06] 判断回文字符串
来源：http://mfk.xuetiantiany.cn

Py:   s == s[::-1]
来源：http://kqz.xingfuxueyuan.xyz

PHP:  $s === strrev($s);
来源：http://brd.shangyingyoupin.top

JS:   s === [...s].reverse().join("")
来源：http://zfo.nanxinkj.top

TS:   s === [...s].reverse().join("")
来源：http://cih.xylfe.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://may.cheryme.top

Go:   // 双指针从两端比较
来源：http://pcm.shanyushiyangkeji.top

Ruby: s == s.reverse
来源：http://chc.hnxiangtu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bky.shzxlz.cn

[N07] 两数之和（返回下标）
来源：http://khi.fanxiaobao.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://naw.fktsv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ijz.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yts.ctjpmb.com

TS:   // 手写 Map<string, number>
来源：http://fuw.dashuyun.cn

Java: // 手写 HashMap
来源：http://iqb.cucudq.cn

Go:   // 手写 map[int]int
来源：http://vfa.jinghuilouyu.cn

Ruby: // 手写 Hash
来源：http://yum.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wbt.gzhubu.top

[N08] 生成全排列
来源：http://rna.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://fgb.tianlin.xyz

PHP:  // 手写递归交换
来源：http://vhv.dashuyun.cn

JS:   // 手写回溯递归
来源：http://ypz.havefunace.top

TS:   // 手写回溯递归
来源：http://dxn.jiagoushi.top

Java: // 手写回溯递归
来源：http://qez.aibaodan.cn

Go:   // 手写回溯递归
来源：http://acw.nanxuanxn.top

Ruby: arr.permutation.to_a
来源：http://acy.jqgfzy.top

C#:   // 手写回溯递归
来源：http://ztv.zhijiandao.cn

[N09] 栈与队列
来源：http://zyo.jinyuanbaomall.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://azx.cheryme.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fee.pycfn.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ipt.xuetiantiany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tjt.snrcjt.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cyh.meibo888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pry.hysaishi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://krj.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vpv.birdmap.top

[N10] 链表节点定义
来源：http://dsh.9152youxi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sud.ivvv.top

PHP:  class Node { public $v; public $next = null; }
来源：http://aqi.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kco.jqgfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bdl.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://tvp.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cyn.xuetiantiany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qxh.52xcode.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wqu.jianghu66.top

[N11] 二叉树中序遍历
来源：http://lba.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vqq.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://gqt.yuxming.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lah.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fkz.cqqwz.cn

Java: // 手写递归
来源：http://joc.jianghu66.top

Go:   // 手写递归
来源：http://wtw.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gyb.ctjpmb.com

C#:   // 手写递归
来源：http://kit.gogol.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://upf.ctjpmb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ouq.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tnm.gogol.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xpz.yuanzhike.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ygs.hesvh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yys.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pvg.ivvv.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fss.zhoulong.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tkr.sxryk.cn

================================================================================
来源：http://gan.daria6918.cn

O. 并发与异步
来源：http://efn.yuxming.cn

================================================================================
来源：http://mzr.gaohongyu789.top

[O01] 启动一个线程
来源：http://nyt.gotoacloud.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pos.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://akr.mhx1999.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sni.fanxiaobao.xyz

TS:   // 同 JS
来源：http://xac.jinghuilouyu.cn

Java: new Thread(() -> f()).start()
来源：http://fuy.meibo888.top

Go:   go f()
来源：http://mmy.feifeiyinyue.top

Ruby: Thread.new { f }
来源：http://bdy.shzxlz.cn

C#:   Task.Run(() => F());
来源：http://iao.havefunace.top

[O02] 使用线程池
来源：http://ane.kuanghao11.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qsh.hnxiangtu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://omw.tarul.cn

JS:   // worker_threads 线程池
来源：http://plh.shanyushiyangtech.top

TS:   // worker_threads 线程池
来源：http://vdh.yuxming.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oie.jinqigfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vem.kuanghao11.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lox.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fyb.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://tql.jqgfzy.top

Py:   with lock: shared += 1
来源：http://tgb.xuanzx.com

PHP:  // 用 flock() 做文件锁
来源：http://zci.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xxs.shangyingyoupin.top

TS:   // 同 JS
来源：http://gib.chenlongwang.top

Java: synchronized (this) { shared++; }
来源：http://eaz.bjfxy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://guq.sweek.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://kau.hongshengwenyu.top

C#:   lock (gate) { shared++; }
来源：http://xek.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://zlr.hongshengwenyu.top

Py:   async def f():⏎    await g()
来源：http://iab.nwbrower.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ibk.sjlbkw.cn

JS:   async function f() { await g(); }
来源：http://uob.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lrh.aizwys.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rdo.sweek.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eaa.daxiang520.top

Ruby: # 用 Fiber 或 async gem
来源：http://pbj.zhixingplan.top

C#:   async Task F() { await G(); }
来源：http://ngi.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://hea.nanxinkj.top

Py:   asyncio.gather(*tasks)
来源：http://rex.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xkh.cucudq.cn

JS:   await Promise.all(tasks)
来源：http://hel.zdqjudy.top

TS:   await Promise.all(tasks)
来源：http://cts.cashguo.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://usb.aibaodan.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://awy.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://drl.tianlin.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://xdr.ydzc1.top

[O06] 使用进程池
来源：http://rcb.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ref.chenjidiqi.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://avk.tanke756.top

JS:   // child_process / cluster 模块
来源：http://igr.tarul.cn

TS:   // child_process / cluster 模块
来源：http://cva.tian-w.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jpz.jinqigufen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pmu.cheryme.top

Ruby: // fork 块
来源：http://vme.ybcxt.top

C#:   Parallel.For
来源：http://ewn.snrcjt.cn

================================================================================
来源：http://mau.jqgufenzy.top

P. 常用工具函数
来源：http://xgh.sweek.top

================================================================================
来源：http://jod.wangshuangyany.cn

[P01] 生成 UUID
来源：http://gmd.yvedp.cn

Py:   str(uuid.uuid4())
来源：http://dim.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yzn.havefunace.top

JS:   crypto.randomUUID()
来源：http://jwc.xuanzx.com

TS:   crypto.randomUUID()
来源：http://cpb.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://fiv.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://zhl.daxiang520.top

Ruby: SecureRandom.uuid
来源：http://ifr.ppjwa.cn

C#:   Guid.NewGuid().ToString()
来源：http://xlb.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://eol.zhixingplan.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hvl.hnqzz.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ntc.yuxming.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fqz.fehbvm.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rne.quarkkingdee.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pbv.redwolf501.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ctv.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jho.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://znc.yfazqb.com

[P03] 生成短随机字符串
来源：http://hmc.shanyushiyangtech.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qya.chenzaomai.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tdr.tanke756.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://osa.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mxc.hywenlv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gvl.fzhhl.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ogh.pycfn.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://nrm.xuetiantiany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wyc.shanyushiyangtech.top

[P04] 求长度
来源：http://aih.ivvv.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pqd.gotoacloud.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jut.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oph.xylfe.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xlw.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://inm.zhoulong.xyz

Go:   len(arr);  len(m)
来源：http://owr.daria6918.cn

Ruby: x.length;  x.size
来源：http://koe.mhx1999.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bcn.yangfankeji.com

[P05] 判断两个对象内容是否相等
来源：http://hqw.tanke756.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qgi.kuanghao11.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tax.cqqwz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mnu.fzhhl.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hiw.jlsjyb.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dhw.xziqi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kwu.0kj1m.cn

Ruby: a == b
来源：http://drx.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bky.aizwys.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kyh.chenzaomai.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wnw.jqgufenzy.top

PHP:  if (empty($x)) {}
来源：http://jph.ivvv.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wzz.jlsjyb.cn

TS:   if (x == null) {}
来源：http://acd.snrcjt.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ggm.jinyuanbaomall.cn

Go:   if x == nil {}
来源：http://mex.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tlc.yanxiufei.cn

C#:   if (x is null) {}
来源：http://yhf.cqqwz.cn

[P07] 防抖与节流
来源：http://huu.yuxming.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://usz.jinqigfzy.top

PHP:  // 手写时间戳比较
来源：http://edv.hcnkem.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uns.dianchejie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pit.shzxlz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gml.guannengcc.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bbj.yj202588.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://avt.gaohongyu789.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yur.zdbjq.cn

[P08] 处理浮点精度问题
来源：http://rdi.jinghuilouyu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eye.epnwcf.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gqt.hfpthk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://juj.daxiang520.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hiv.zdbjq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://djr.yj20258.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mmc.ybcxt.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lkd.chenzaomai.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://myz.quarkkingdee.top

================================================================================
来源：http://mdw.xziqi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gsn.pycfn.com

================================================================================
来源：http://jpc.zhongyouzk.top

[Q01] 创建表
来源：http://gdv.hfpthk.cn

CREATE TABLE users (
来源：http://jbu.nanxinkj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uxw.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://kjr.gogol.net.cn

email VARCHAR(100) UNIQUE,
来源：http://wdj.hfpthk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oar.yfazqb.com

);
来源：http://cvf.snrcjt.cn

[Q02] 创建带外键的表
来源：http://kap.havefunace.top

CREATE TABLE orders (
来源：http://grk.jyoumei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wpx.uphjek.com

user_id INT NOT NULL,
来源：http://aun.c1oappe.top

amount DECIMAL(10, 2),
来源：http://crf.hysaishi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ezl.quarkkingdee.top

);
来源：http://evn.svipenyu.cn

[Q03] 增加列
来源：http://cca.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kkv.ydzc1.top

[Q04] 修改列类型
来源：http://tkc.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tjc.gogol.net.cn

[Q05] 重命名列
来源：http://zbn.xuanzx.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://urd.vehdjk.com

[Q06] 删除列
来源：http://tyr.gzhubu.top

ALTER TABLE users DROP COLUMN age;
来源：http://whx.shuidangran.top

[Q07] 删除表
来源：http://ppb.bjfxy.top

DROP TABLE IF EXISTS orders;
来源：http://rhz.fktsv.cn

[Q08] 创建普通索引
来源：http://dfy.jinqigfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cvq.gogol.net.cn

[Q09] 创建唯一索引
来源：http://dnb.feifeiyinyue.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uzl.jinqigfzy.top

[Q10] 插入单行
来源：http://spt.daxiang520.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jrd.52xcode.cn

[Q11] 一次插入多行
来源：http://dqv.yonumen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ztd.nwbrower.top

[Q12] 插入后取自增 ID
来源：http://vpd.yongpay.top

INSERT INTO users (name) VALUES ('C');
来源：http://mdo.feifeiyinyue.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ppr.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://sxe.jinyuanbaomall.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rkv.dashuyun.cn

[Q14] 存在则更新（upsert）
来源：http://cgb.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mzu.yueranfly.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vgl.jianghu66.top

[Q15] 查询全部
来源：http://xzs.ywan-chungtsiang.top

SELECT * FROM users;
来源：http://gya.snrcjt.cn

[Q16] 查询指定列
来源：http://svd.zdbjq.cn

SELECT id, name FROM users;
来源：http://tyt.chenzaomai.com

[Q17] 条件查询
来源：http://euy.gzhubu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wxa.316326.xyz

[Q18] 模糊匹配
来源：http://ijo.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vzk.snrcjt.cn

[Q19] 范围查询
来源：http://kqo.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pwf.birdmap.top

[Q20] IN 列表
来源：http://rpa.gzhubu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cko.pengpengdd.cyou

[Q21] 空值判断
来源：http://ase.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://obz.vqdsnc.cn

[Q22] 排序
来源：http://sse.yj20258.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fdb.snrcjt.cn

[Q23] 分页
来源：http://ptr.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wva.mhx1999.top

[Q24] 去重
来源：http://kpp.jinyuanbaomall.cn

SELECT DISTINCT city FROM users;
来源：http://svp.xinyue.icu

[Q25] 只取前 N 条
来源：http://jkc.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uiy.c1oappe.top

[Q26] 计数
来源：http://ylz.zhoulong.xyz

SELECT COUNT(*) FROM users;
来源：http://qqi.chenzaomai.com

[Q27] 条件计数
来源：http://jmx.yj20258888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qrp.yj202588.top

[Q28] 求和与平均
来源：http://lvv.chenjidiqi.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bed.xinyue.icu

[Q29] 最大最小值
来源：http://wgg.fzhhl.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ohr.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://dwn.jyoumei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://okw.andypj.xyz

[Q31] 分组后过滤
来源：http://vbe.andypj.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://koh.hysaishi.cn

[Q32] 分组拼接字符串
来源：http://iyd.bjfxy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hmv.gotoacloud.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oih.havefunace.top

[Q33] 多列分组
来源：http://nyy.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ntu.cucudq.cn

[Q34] 每组取第一条
来源：http://nbq.jinyuanbaomall.cn

SELECT * FROM (
来源：http://csb.jinghuilouyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://epd.jqgfzy.top

) t WHERE rn = 1;
来源：http://iju.yj202588.top

[Q35] 内连接
来源：http://bhn.shuidangran.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zej.tarul.cn


<!-- 参考信息 -->