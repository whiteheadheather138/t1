代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pkv.fktsv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fvw.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://lqs.cqqwz.cn

[N04] 斐波那契数列
来源：http://uai.birdmap.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uwf.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sef.dashuyun.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ryy.shzxlz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gox.fanxiaobao.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://akn.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ppt.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jjw.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mwj.xinyue.icu

[N05] 最大公约数
来源：http://gjv.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://qwf.svipenyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lrg.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://whd.gogol.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mdh.cdnleiting.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nws.sufxvd.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vyx.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://abv.yanxiufei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://git.gaohongyu789.top

[N06] 判断回文字符串
来源：http://cuu.aizwys.cn

Py:   s == s[::-1]
来源：http://psi.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://edo.ivvv.top

JS:   s === [...s].reverse().join("")
来源：http://hrd.smart0.xyz

TS:   s === [...s].reverse().join("")
来源：http://gio.xziqi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mbt.hcnkem.com

Go:   // 双指针从两端比较
来源：http://pkj.zdbjq.cn

Ruby: s == s.reverse
来源：http://mcx.jqgfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wot.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://dxa.chenlongwang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kqb.xziqi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sgp.52xcode.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hbm.xziqi.cn

TS:   // 手写 Map<string, number>
来源：http://ter.meibo888.top

Java: // 手写 HashMap
来源：http://pnk.snrcjt.cn

Go:   // 手写 map[int]int
来源：http://plg.wangshuangyany.cn

Ruby: // 手写 Hash
来源：http://xsn.ctjpmb.com

C#:   // 手写 Dictionary<int, int>
来源：http://ssj.zhiwuduotai.top

[N08] 生成全排列
来源：http://swa.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://rjv.aibaodan.cn

PHP:  // 手写递归交换
来源：http://fqc.ydzc1.top

JS:   // 手写回溯递归
来源：http://vah.tarul.cn

TS:   // 手写回溯递归
来源：http://yno.aizwys.cn

Java: // 手写回溯递归
来源：http://wva.svipenyu.cn

Go:   // 手写回溯递归
来源：http://wsf.birdmap.top

Ruby: arr.permutation.to_a
来源：http://pyt.fktsv.cn

C#:   // 手写回溯递归
来源：http://qhj.haohaochexian.top

[N09] 栈与队列
来源：http://xxl.ehwqpu.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zvo.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uxg.yvedp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://spl.bbcook.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gbz.ctjpmb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oxw.zdbjq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tlq.gogol.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://srd.svipenyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zqm.jinghuilouyu.cn

[N10] 链表节点定义
来源：http://iyo.yueranfly.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tzh.fzhhl.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tgj.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mqm.yj20258.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tbp.yvedp.cn

Java: class Node { int v; Node next; }
来源：http://jet.dianchejie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xjs.tanke756.top

Ruby: Node = Struct.new(:v, :next)
来源：http://axr.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jxn.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://lmh.pycfn.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jph.yongpay.top

PHP:  // 手写递归函数
来源：http://dba.zhiwuduotai.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qjb.zhengqikj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xij.aibaodan.cn

Java: // 手写递归
来源：http://uac.xuanzx.com

Go:   // 手写递归
来源：http://cuu.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ayy.ivvv.top

C#:   // 手写递归
来源：http://cuh.cqqwz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tvd.guannengcc.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tck.andypj.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lnz.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mbd.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yjy.yj202588.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yrm.gzhubu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://trv.nwbrower.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gah.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pcj.ydzc1.top

================================================================================
来源：http://boq.birdmap.top

O. 并发与异步
来源：http://ieu.sufxvd.cn

================================================================================
来源：http://cha.cashguo.top

[O01] 启动一个线程
来源：http://cmj.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lyq.xingfuxueyuan.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qvh.gotoacloud.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eyo.aizwys.cn

TS:   // 同 JS
来源：http://sdr.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://dyf.zhixingplan.top

Go:   go f()
来源：http://yzm.hysaishi.cn

Ruby: Thread.new { f }
来源：http://ize.shuidangran.top

C#:   Task.Run(() => F());
来源：http://xhl.shanyushiyangtech.top

[O02] 使用线程池
来源：http://lzk.aizwys.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mza.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cui.jinghuilouyu.cn

JS:   // worker_threads 线程池
来源：http://ruy.sweek.top

TS:   // worker_threads 线程池
来源：http://edz.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://iqa.shangyingyoupin.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hdr.0kj1m.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aog.ctjpmb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eua.cashguo.top

[O03] 加锁保护共享数据
来源：http://xgk.gotoacloud.top

Py:   with lock: shared += 1
来源：http://hep.jinqigufen.top

PHP:  // 用 flock() 做文件锁
来源：http://yjz.nanxinkj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fgl.uphjek.com

TS:   // 同 JS
来源：http://qcf.pengpengdd.cyou

Java: synchronized (this) { shared++; }
来源：http://jpa.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://isd.316326.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://ehp.yanxiufei.cn

C#:   lock (gate) { shared++; }
来源：http://hrp.xingfuxueyuan.xyz

[O04] 定义异步函数并等待
来源：http://qlk.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://gth.uphjek.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wez.pycfn.com

JS:   async function f() { await g(); }
来源：http://cby.tian-w.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xem.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hut.cheryme.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://djo.cheryme.top

Ruby: # 用 Fiber 或 async gem
来源：http://tfb.hywenlv.cn

C#:   async Task F() { await G(); }
来源：http://amu.zhongyouzk.top

[O05] 并发执行并等待全部完成
来源：http://hln.hywenlv.cn

Py:   asyncio.gather(*tasks)
来源：http://amx.shuidangran.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cpx.aizwys.cn

JS:   await Promise.all(tasks)
来源：http://rju.fanxiaobao.xyz

TS:   await Promise.all(tasks)
来源：http://xre.sjlbkw.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://par.yangfankeji.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lbx.hammf.cn

Ruby: threads.map(&:join)
来源：http://lxi.zhaomingkeji.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://txu.jinyuanbaomall.cn

[O06] 使用进程池
来源：http://mlz.tanke756.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vvj.daxiang520.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vpk.zhiwuduotai.top

JS:   // child_process / cluster 模块
来源：http://nvj.cdnleiting.top

TS:   // child_process / cluster 模块
来源：http://kif.ehwqpu.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ogf.xinyue.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jka.jinqigufen.top

Ruby: // fork 块
来源：http://vmm.jinqigfzy.top

C#:   Parallel.For
来源：http://ixj.mhx1999.top

================================================================================
来源：http://ffb.jinghuilouyu.cn

P. 常用工具函数
来源：http://zka.jyoumei.cn

================================================================================
来源：http://rgd.zdqjudy.top

[P01] 生成 UUID
来源：http://uen.hcnkem.com

Py:   str(uuid.uuid4())
来源：http://ygc.aibaodan.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://smn.gaohongyu789.top

JS:   crypto.randomUUID()
来源：http://yjh.tanke756.top

TS:   crypto.randomUUID()
来源：http://plx.jinqigufen.top

Java: UUID.randomUUID().toString()
来源：http://qqc.yongpay.top

Go:   // 用 github.com/google/uuid
来源：http://gha.redwolf501.top

Ruby: SecureRandom.uuid
来源：http://jzk.pycfn.com

C#:   Guid.NewGuid().ToString()
来源：http://gmn.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://ejs.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gan.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dwo.hywenlv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pde.daxiang520.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ndv.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uty.jinyuanbaomall.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ucw.zdbjq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zdq.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fab.meibo888.top

[P03] 生成短随机字符串
来源：http://lae.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wbz.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dcq.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kco.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rxz.sxryk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gfo.hnxiangtu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dkb.sxryk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ovj.daxiang520.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gxg.hnqzz.top

[P04] 求长度
来源：http://xmp.tianlin.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ssq.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lqw.sweek.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mon.ctjpmb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zut.cheryme.top

Java: list.size();  map.size();  s.length()
来源：http://hwi.jqgfzy.top

Go:   len(arr);  len(m)
来源：http://ksy.yueranfly.top

Ruby: x.length;  x.size
来源：http://xbx.ppjwa.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xjs.zdbjq.cn

[P05] 判断两个对象内容是否相等
来源：http://iac.nanxinkj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ozz.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://duy.yonumen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mjl.tarul.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qfv.yangfankeji.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ogk.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fkr.yonumen.top

Ruby: a == b
来源：http://zvb.sweek.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qve.zhiwuduotai.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zmu.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://imi.guowangkeji.top

PHP:  if (empty($x)) {}
来源：http://kvi.sweek.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ncv.aibaodan.cn

TS:   if (x == null) {}
来源：http://rlf.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://rgs.nanxinkj.top

Go:   if x == nil {}
来源：http://hfo.hesvh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kmz.jqgfzy.top

C#:   if (x is null) {}
来源：http://axu.xziqi.cn

[P07] 防抖与节流
来源：http://vxs.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rov.yuxming.cn

PHP:  // 手写时间戳比较
来源：http://abk.hammf.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gkl.zdqjudy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://idr.nanxinkj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tol.zdqjudy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jpa.ydzc1.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qyd.aizwys.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wnd.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://riy.yuxming.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aca.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://stk.zhaomingkeji.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vof.pycfn.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yla.c1oappe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://boh.shzxlz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zxx.zhaomingkeji.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pzj.jqgfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hbh.zhijiandao.cn

================================================================================
来源：http://njj.jinyuanbaomall.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fmk.mhx1999.top

================================================================================
来源：http://hxq.snrcjt.cn

[Q01] 创建表
来源：http://hnu.bjfxy.top

CREATE TABLE users (
来源：http://czx.aibaodan.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uid.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://huo.fktsv.cn

email VARCHAR(100) UNIQUE,
来源：http://aph.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jpt.ivvv.top

);
来源：http://scz.hysaishi.cn

[Q02] 创建带外键的表
来源：http://con.zhoulong.xyz

CREATE TABLE orders (
来源：http://epz.hcnkem.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bmk.ydjk.org.cn

user_id INT NOT NULL,
来源：http://ptw.yonumen.top

amount DECIMAL(10, 2),
来源：http://bwt.316326.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://opc.bbcook.cn

);
来源：http://fmu.0kj1m.cn

[Q03] 增加列
来源：http://bag.fzhhl.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ysd.tanke756.top

[Q04] 修改列类型
来源：http://ava.haohaochexian.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sei.yueranfly.top

[Q05] 重命名列
来源：http://gkl.dashuyun.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gak.xziqi.cn

[Q06] 删除列
来源：http://vdn.yuanzhike.top

ALTER TABLE users DROP COLUMN age;
来源：http://cff.hammf.cn

[Q07] 删除表
来源：http://zex.fehbvm.com

DROP TABLE IF EXISTS orders;
来源：http://lql.shuidangran.top

[Q08] 创建普通索引
来源：http://gqd.jqgfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nuu.ydjk.org.cn

[Q09] 创建唯一索引
来源：http://tbb.zhengqikj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hrh.0kj1m.cn

[Q10] 插入单行
来源：http://qkg.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://imc.ivvv.top

[Q11] 一次插入多行
来源：http://lhu.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zbw.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://rrv.xingfuxueyuan.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://mzx.iojbl.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wnf.haohaochexian.top

[Q13] 忽略重复插入
来源：http://jce.gotoacloud.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://olb.wangshuangyany.cn

[Q14] 存在则更新（upsert）
来源：http://fss.ctjpmb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ydp.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hpr.fktsv.cn

[Q15] 查询全部
来源：http://gzt.redwolf501.top

SELECT * FROM users;
来源：http://tqu.chenlongwang.top

[Q16] 查询指定列
来源：http://rzq.nwbrower.top

SELECT id, name FROM users;
来源：http://rdi.feifeiyinyue.top

[Q17] 条件查询
来源：http://jbj.tarul.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qcs.yonumen.top

[Q18] 模糊匹配
来源：http://ond.dashuyun.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://izt.gzhubu.top

[Q19] 范围查询
来源：http://kvh.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hlo.hammf.cn

[Q20] IN 列表
来源：http://uet.bbcook.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rnj.0kj1m.cn

[Q21] 空值判断
来源：http://rcz.yuxming.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qjc.fehbvm.com

[Q22] 排序
来源：http://eaf.sysykeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xxx.9152youxi.cn

[Q23] 分页
来源：http://djj.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nwj.snrcjt.cn

[Q24] 去重
来源：http://vfq.andypj.xyz

SELECT DISTINCT city FROM users;
来源：http://yzx.haohaochexian.top

[Q25] 只取前 N 条
来源：http://ymx.redwolf501.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ivo.iojbl.cn

[Q26] 计数
来源：http://loi.kuanghao11.cn

SELECT COUNT(*) FROM users;
来源：http://pow.zhiwuduotai.top

[Q27] 条件计数
来源：http://lrq.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://atu.hysaishi.cn

[Q28] 求和与平均
来源：http://vlm.fengsongda.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bke.jqgfzy.top

[Q29] 最大最小值
来源：http://mrv.52xcode.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://efm.zhiwuduotai.top

[Q30] 分组统计
来源：http://vrh.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vsg.yueranfly.top

[Q31] 分组后过滤
来源：http://nxu.316326.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jvk.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://spe.jqgfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nfo.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jxe.daria6918.cn

[Q33] 多列分组
来源：http://cfx.kuanghao11.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ehm.ivvv.top

[Q34] 每组取第一条
来源：http://wud.c1oappe.top

SELECT * FROM (
来源：http://cgw.bbcook.cn


<!-- 参考信息 -->