代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gmzkxtzil.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gzfqlczal.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.epnwcf.com/Article/details/ggnulljvf.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.bbcook.cn/Article/details/gjtsagukx.sHtML

Ruby: s == s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gzvgrghmo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gekwnagus.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.tarul.cn/Article/details/ghssrpkef.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.epnwcf.com/Article/details/genytzxij.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.tarul.cn/Article/details/gaerbhynv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.epnwcf.com/Article/details/gkjljierx.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.bbcook.cn/Article/details/gufqglawv.sHtML

Java: // 手写 HashMap
来源：http://baike.yfazqb.com/Article/details/gwdilekoa.sHtML

Go:   // 手写 map[int]int
来源：http://baike.bbcook.cn/Article/details/gtfqenmde.sHtML

Ruby: // 手写 Hash
来源：http://baike.epnwcf.com/Article/details/gvfaleodo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.tarul.cn/Article/details/gfwcfkvys.sHtML

[N08] 生成全排列
来源：http://baike.fktsv.cn/Article/details/ghiajgtyg.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.yfazqb.com/Article/details/gbweglvpb.sHtML

PHP:  // 手写递归交换
来源：http://m.share.bbcook.cn/Article/details/gqkulffrb.sHtML

JS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/grwndkkep.sHtML

TS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gcnwlwqah.sHtML

Java: // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/ghfdxqhfs.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gwkuwfmiw.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.sjlbkw.cn/Article/details/gclvhtqob.sHtML

C#:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gwyaxheqs.sHtML

[N09] 栈与队列
来源：http://baike.vehdjk.com/Article/details/gffjmqzyp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gsfnuibed.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gdlsqyrwp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/gkvdwrwxz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fktsv.cn/Article/details/gzksdiqsg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gcefpexst.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.tarul.cn/Article/details/gonvswhtw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gouqtzrmw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.vehdjk.com/Article/details/gxsgihjel.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/gtwmcjhyf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.vehdjk.com/Article/details/gxtjqchhs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.epnwcf.com/Article/details/giuwrwgss.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.yfazqb.com/Article/details/gehsnrldg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/gewautnkk.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.tarul.cn/Article/details/ghtbkmgym.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/gxawljyab.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.yfazqb.com/Article/details/gpewdgejz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.vehdjk.com/Article/details/gbumqvsnf.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.yfazqb.com/Article/details/guycvyflt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.tarul.cn/Article/details/gsnfvohts.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/gsecdbfjd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gelwxffra.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gzzudzpjl.sHtML

Java: // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gdegbaqsq.sHtML

Go:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/guehnegqq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.vehdjk.com/Article/details/gzfwduhpa.sHtML

C#:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/ghepwvbzz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.vehdjk.com/Article/details/gbrcqviuh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fktsv.cn/Article/details/gezwbgdtr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.epnwcf.com/Article/details/gtpbciqgh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/giwdqpyiv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gqguqmocp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/gpptqdhxv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.epnwcf.com/Article/details/gbmwryjue.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.vehdjk.com/Article/details/gptuuzajg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/grweqxnja.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gkrldlkfy.sHtML

O. 并发与异步
来源：http://wap.bbcook.cn/Article/details/gyimgcbnl.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gubzkmwwh.sHtML

[O01] 启动一个线程
来源：http://read.share.vehdjk.com/Article/details/gjfvkonyo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fktsv.cn/Article/details/grkxldepj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fktsv.cn/Article/details/gniuvhzxk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fktsv.cn/Article/details/goorucdyz.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/gpkqgusuo.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.bbcook.cn/Article/details/glupbvigq.sHtML

Go:   go f()
来源：http://www.m.share.bbcook.cn/Article/details/gkeircmzo.sHtML

Ruby: Thread.new { f }
来源：http://blog.sjlbkw.cn/Article/details/gcgcyavny.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.bbcook.cn/Article/details/gnchxmeak.sHtML

[O02] 使用线程池
来源：http://mobile.fktsv.cn/Article/details/gbvnxlnow.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fktsv.cn/Article/details/gifomgqql.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.yfazqb.com/Article/details/goeoqezmk.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/ghayapfmk.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/ghexcnlhw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.tarul.cn/Article/details/gncdzlryp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.vehdjk.com/Article/details/gqftjvwog.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.vehdjk.com/Article/details/gtnappjqv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.bbcook.cn/Article/details/gcnqbzymy.sHtML

[O03] 加锁保护共享数据
来源：http://wap.tarul.cn/Article/details/gvpvskijy.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.sjlbkw.cn/Article/details/gyqszqjpj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.tarul.cn/Article/details/gafgplumw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.tarul.cn/Article/details/gzioiyyue.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gwvrafdse.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gklhorshb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.tarul.cn/Article/details/gkcwcwfbt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fktsv.cn/Article/details/gosyleqyk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/gfsrtkzwr.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/gzeeguibj.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.bbcook.cn/Article/details/gsdnekgvm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fktsv.cn/Article/details/gsiarzjxj.sHtML

JS:   async function f() { await g(); }
来源：http://3g.tarul.cn/Article/details/gdsczojeg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.yfazqb.com/Article/details/ggrofyqxx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/gznhojebt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fktsv.cn/Article/details/gxwpfxqhn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.vehdjk.com/Article/details/gzqzywiym.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.vehdjk.com/Article/details/gsikzpbbj.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.sjlbkw.cn/Article/details/gnixrphen.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fktsv.cn/Article/details/gqtpoivcu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/gcgxhegps.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gmyqfdgft.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.bbcook.cn/Article/details/giyfhefir.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.yfazqb.com/Article/details/gehohzlqh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.sjlbkw.cn/Article/details/gzanjmcff.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/gcxwzvtxe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.vehdjk.com/Article/details/givhorddz.sHtML

[O06] 使用进程池
来源：http://www.m.share.vehdjk.com/Article/details/gllngatjd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.yfazqb.com/Article/details/ghhevjlmj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.tarul.cn/Article/details/guxkwjbcg.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gcmwkfcck.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/gjgkcgfgc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.vehdjk.com/Article/details/gnfhfpfyx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.epnwcf.com/Article/details/gsarjijrd.sHtML

Ruby: // fork 块
来源：http://baike.epnwcf.com/Article/details/ggjcfcrtc.sHtML

C#:   Parallel.For
来源：http://mobile.tarul.cn/Article/details/gixzkfazc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxqthsigs.sHtML

P. 常用工具函数
来源：http://mobile.fktsv.cn/Article/details/gbgltluij.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/grdqjghoq.sHtML

[P01] 生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/glgffxijh.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.epnwcf.com/Article/details/gtcwltalh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.bbcook.cn/Article/details/gybyfsaqt.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gptowziyj.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gwuowaivq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.tarul.cn/Article/details/gnyinaqsc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fktsv.cn/Article/details/gfvvsmemg.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.vehdjk.com/Article/details/gmvlzxoge.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.yfazqb.com/Article/details/grvihqqoe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.sjlbkw.cn/Article/details/ggacvfgss.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.vehdjk.com/Article/details/gshuwfaqc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.bbcook.cn/Article/details/gjiegyjvc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.yfazqb.com/Article/details/gkfkiqgsb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.vehdjk.com/Article/details/gfsvvbczp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.epnwcf.com/Article/details/gzlhqlkyk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.epnwcf.com/Article/details/gmpyzlkpj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fktsv.cn/Article/details/gutfjhvns.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.bbcook.cn/Article/details/gxaeakxzt.sHtML

[P03] 生成短随机字符串
来源：http://wap.yfazqb.com/Article/details/gowtewqzn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.vehdjk.com/Article/details/gwnlulrea.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvnquzth.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gtcsfxolv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gedclztug.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.bbcook.cn/Article/details/geibcanwz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/gmhkoghpi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.epnwcf.com/Article/details/gjbnowfvs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fktsv.cn/Article/details/gzwumjsit.sHtML

[P04] 求长度
来源：http://wap.sjlbkw.cn/Article/details/gjiggzrqi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.vehdjk.com/Article/details/gtgjqtvjj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gzbjfpnwp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/golyxgwld.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/gibatodee.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.tarul.cn/Article/details/gvodyqync.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.epnwcf.com/Article/details/gwvwhhobw.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.epnwcf.com/Article/details/gdefeaieq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.vehdjk.com/Article/details/glspvphpg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.sjlbkw.cn/Article/details/gztkkofsr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.yfazqb.com/Article/details/gmqdzsebb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.yfazqb.com/Article/details/gjobrpyue.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.yfazqb.com/Article/details/goorvfrfw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.yfazqb.com/Article/details/gbvmazfpg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.tarul.cn/Article/details/gaveafhhi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fktsv.cn/Article/details/gllqczmzq.sHtML

Ruby: a == b
来源：http://www.m.share.vehdjk.com/Article/details/gphgecrfy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.vehdjk.com/Article/details/gcigwwwvq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.epnwcf.com/Article/details/gpslokndf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.vehdjk.com/Article/details/gqfbsrlgk.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.sjlbkw.cn/Article/details/glniewjfq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.bbcook.cn/Article/details/gbvxbqejs.sHtML

TS:   if (x == null) {}
来源：http://mobile.fktsv.cn/Article/details/gkdchswhs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gkdggdfqp.sHtML

Go:   if x == nil {}
来源：http://3g.sjlbkw.cn/Article/details/goycmxhsb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.yfazqb.com/Article/details/gqpdbqdin.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/grbzfckvo.sHtML

[P07] 防抖与节流
来源：http://wap.epnwcf.com/Article/details/gjzzcdcgm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.tarul.cn/Article/details/gruqsopnf.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.sjlbkw.cn/Article/details/gvtmupwxx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/gurnqftqk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gqnggvalm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.yfazqb.com/Article/details/gkuiiyumb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fktsv.cn/Article/details/gdqnteesp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fktsv.cn/Article/details/gvidympls.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.epnwcf.com/Article/details/geixnhrvi.sHtML

[P08] 处理浮点精度问题
来源：http://baike.bbcook.cn/Article/details/gqztpxnip.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.bbcook.cn/Article/details/gbkmbvhww.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.sjlbkw.cn/Article/details/gijaosdpd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.sjlbkw.cn/Article/details/gcwnkaulq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gtgtjrsri.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.yfazqb.com/Article/details/gmcwxqpgm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.tarul.cn/Article/details/gglwyzagq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.vehdjk.com/Article/details/gazihvgmb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.yfazqb.com/Article/details/gvwzwfxuk.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gbqrowxuf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fktsv.cn/Article/details/gxrgbgtak.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gxmrhhbde.sHtML

[Q01] 创建表
来源：http://baike.epnwcf.com/Article/details/gwihswemc.sHtML

CREATE TABLE users (
来源：http://www.share.yfazqb.com/Article/details/ghdbynrcr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gpffhndal.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.yfazqb.com/Article/details/gyqsagqqg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.epnwcf.com/Article/details/gnaijxeyu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.yfazqb.com/Article/details/gyvhlujst.sHtML

);
来源：http://m.share.tarul.cn/Article/details/gmipsyfkq.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.vehdjk.com/Article/details/gjugmawxt.sHtML

CREATE TABLE orders (
来源：http://www.share.vehdjk.com/Article/details/gmpcercti.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fktsv.cn/Article/details/gqawzqlpd.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/gqhmjkbla.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.vehdjk.com/Article/details/gsgnhfxdr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.vehdjk.com/Article/details/gwoguixue.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gzurrztyd.sHtML

[Q03] 增加列
来源：http://m.share.fktsv.cn/Article/details/gvcbtkcin.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.epnwcf.com/Article/details/gcawglbus.sHtML

[Q04] 修改列类型
来源：http://blog.epnwcf.com/Article/details/gxrbiarsl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.bbcook.cn/Article/details/gdgfwldin.sHtML

[Q05] 重命名列
来源：http://3g.vehdjk.com/Article/details/giruwnmko.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.sjlbkw.cn/Article/details/gnwarbiqy.sHtML

[Q06] 删除列
来源：http://blog.bbcook.cn/Article/details/gkaqqqtbl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fktsv.cn/Article/details/gexridhox.sHtML

[Q07] 删除表
来源：http://wap.sjlbkw.cn/Article/details/gypkidkgm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.epnwcf.com/Article/details/gsxsztrpd.sHtML

[Q08] 创建普通索引
来源：http://3g.sjlbkw.cn/Article/details/gimitecld.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/gnahtquww.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.tarul.cn/Article/details/gvkjwldeq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/gqkohwodb.sHtML

[Q10] 插入单行
来源：http://wap.bbcook.cn/Article/details/gpzrwxsuq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.epnwcf.com/Article/details/gawpnffqs.sHtML

[Q11] 一次插入多行
来源：http://www.share.fktsv.cn/Article/details/gdvmtozbx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gufcvjhku.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fktsv.cn/Article/details/glougsjny.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.vehdjk.com/Article/details/gobrambkk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.tarul.cn/Article/details/golmpysyz.sHtML

[Q13] 忽略重复插入
来源：http://baike.epnwcf.com/Article/details/gyitzlvat.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gybdnvipt.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.vehdjk.com/Article/details/gnkqtqjlk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.sjlbkw.cn/Article/details/gfdfvknpe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.sjlbkw.cn/Article/details/gienltdmq.sHtML

[Q15] 查询全部
来源：http://wap.bbcook.cn/Article/details/gijymguqv.sHtML

SELECT * FROM users;
来源：http://m.share.epnwcf.com/Article/details/gfehtfmgg.sHtML

[Q16] 查询指定列
来源：http://3g.fktsv.cn/Article/details/gcvleuvub.sHtML

SELECT id, name FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gnalqloda.sHtML

[Q17] 条件查询
来源：http://wap.yfazqb.com/Article/details/geycjoyiz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.sjlbkw.cn/Article/details/gglvjfphx.sHtML

[Q18] 模糊匹配
来源：http://baike.yfazqb.com/Article/details/gtxzsctpw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.tarul.cn/Article/details/gfwykkwzw.sHtML

[Q19] 范围查询
来源：http://www.share.bbcook.cn/Article/details/gennmlhze.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fktsv.cn/Article/details/gnvpipnhx.sHtML

[Q20] IN 列表
来源：http://www.share.bbcook.cn/Article/details/gmorecimq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.vehdjk.com/Article/details/goxahelyf.sHtML

[Q21] 空值判断
来源：http://m.share.bbcook.cn/Article/details/giuoetkip.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gyilxaoqq.sHtML

[Q22] 排序
来源：http://wap.bbcook.cn/Article/details/guhrjdgpn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.tarul.cn/Article/details/gmhoiflxl.sHtML

[Q23] 分页
来源：http://read.share.fktsv.cn/Article/details/gvevcojon.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.epnwcf.com/Article/details/gzyqcvxrn.sHtML

[Q24] 去重
来源：http://read.share.tarul.cn/Article/details/gwgewnlid.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gcicmhrsg.sHtML

[Q25] 只取前 N 条
来源：http://read.share.sjlbkw.cn/Article/details/gfzmvnaeo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.yfazqb.com/Article/details/gsqrmpzkn.sHtML

[Q26] 计数
来源：http://www.blog.fktsv.cn/Article/details/gixaufkua.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.bbcook.cn/Article/details/gtufbtukw.sHtML

[Q27] 条件计数
来源：http://wap.bbcook.cn/Article/details/gxhybavyt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.bbcook.cn/Article/details/garhbhtbi.sHtML

[Q28] 求和与平均
来源：http://www.blog.bbcook.cn/Article/details/gmwkmzsjj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.vehdjk.com/Article/details/gowkdygvn.sHtML

[Q29] 最大最小值
来源：http://blog.fktsv.cn/Article/details/gjascsexv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.tarul.cn/Article/details/grgxuyezu.sHtML

[Q30] 分组统计
来源：http://www.share.tarul.cn/Article/details/grccnavwj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gsynvjvdj.sHtML

[Q31] 分组后过滤
来源：http://blog.fktsv.cn/Article/details/gmtlvqgau.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.tarul.cn/Article/details/gymvqddpd.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gjuvtepln.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gzuznbewp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.yfazqb.com/Article/details/gixpeeooc.sHtML

[Q33] 多列分组
来源：http://www.blog.yfazqb.com/Article/details/gsgwrrhck.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.tarul.cn/Article/details/gibqfqclx.sHtML

[Q34] 每组取第一条
来源：http://www.blog.sjlbkw.cn/Article/details/gihvtfyhv.sHtML

SELECT * FROM (
来源：http://www.m.share.yfazqb.com/Article/details/gbzqjhpik.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fktsv.cn/Article/details/glproexsz.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.vehdjk.com/Article/details/grqnjugys.sHtML

[Q35] 内连接
来源：http://www.blog.bbcook.cn/Article/details/ghptydjzn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gffyqegdz.sHtML

[Q36] 左连接
来源：http://3g.yfazqb.com/Article/details/gfcikrjpz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/gluunjvaj.sHtML

[Q37] 右连接
来源：http://www.blog.sjlbkw.cn/Article/details/gddfrnqpg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.vehdjk.com/Article/details/gurbgzodc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.epnwcf.com/Article/details/gmzozxyzd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.sjlbkw.cn/Article/details/gglajnifz.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fktsv.cn/Article/details/gflfnszed.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.epnwcf.com/Article/details/gvsxizhoo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.bbcook.cn/Article/details/gkbumkjjd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.bbcook.cn/Article/details/gqsqwwwss.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.yfazqb.com/Article/details/gjpgmdvsg.sHtML

[Q41] 多表连接
来源：http://blog.tarul.cn/Article/details/gguwkzemb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.yfazqb.com/Article/details/gnneqjyax.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.sjlbkw.cn/Article/details/ggszqvens.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.yfazqb.com/Article/details/gzhfuepic.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.bbcook.cn/Article/details/gzleofqks.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.epnwcf.com/Article/details/ggigucrdq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.tarul.cn/Article/details/gbjioccgi.sHtML

[Q43] 标量子查询
来源：http://3g.vehdjk.com/Article/details/grrdwthhj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.tarul.cn/Article/details/gdigdkyck.sHtML


<!-- 参考信息 -->