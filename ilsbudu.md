代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gtkokyqoq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.sjlbkw.cn/Article/details/gpgeneuak.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/gqcumkvjs.sHtML

Ruby: a.gcd(b)
来源：http://www.share.bbcook.cn/Article/details/gwgdqmmqf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.yfazqb.com/Article/details/gfgfojeur.sHtML

[N06] 判断回文字符串
来源：http://m.share.yfazqb.com/Article/details/ggeppxrbl.sHtML

Py:   s == s[::-1]
来源：http://mobile.tarul.cn/Article/details/gikxdwwgz.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gesjifopd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/ghzvlpulg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gbcwwodxn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.epnwcf.com/Article/details/guzhuninn.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.tarul.cn/Article/details/gqdgjbkmz.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gtygjclra.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/geuktxfag.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.sjlbkw.cn/Article/details/glezhmcve.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.yfazqb.com/Article/details/gmmqnkkag.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fktsv.cn/Article/details/gmznmugfx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.tarul.cn/Article/details/gckiwwayk.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gnfjhofhy.sHtML

Java: // 手写 HashMap
来源：http://blog.bbcook.cn/Article/details/gtyexftmj.sHtML

Go:   // 手写 map[int]int
来源：http://wap.epnwcf.com/Article/details/gjlfazmnz.sHtML

Ruby: // 手写 Hash
来源：http://baike.yfazqb.com/Article/details/gthgcyfey.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.vehdjk.com/Article/details/gxwyrmavz.sHtML

[N08] 生成全排列
来源：http://blog.bbcook.cn/Article/details/gfuqoeqpl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.bbcook.cn/Article/details/goteostqb.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/gtgvbvmuo.sHtML

JS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gfqkbtjsz.sHtML

TS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gshsktemg.sHtML

Java: // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gxisiprbq.sHtML

Go:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gtsptcgyl.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/gtpcuklee.sHtML

C#:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gtrakgkjx.sHtML

[N09] 栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrvdjldn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.bbcook.cn/Article/details/gbidblrtl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.bbcook.cn/Article/details/gzqxfwyph.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gkqaezywa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.vehdjk.com/Article/details/gdgpjrqrm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.tarul.cn/Article/details/gynadolhw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.sjlbkw.cn/Article/details/ghccjibbt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gsutavhvu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.epnwcf.com/Article/details/gupcqlriv.sHtML

[N10] 链表节点定义
来源：http://blog.vehdjk.com/Article/details/gcdabugxu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.sjlbkw.cn/Article/details/gebrrfubq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/gxhucvmqb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.tarul.cn/Article/details/gjjfqmfee.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.yfazqb.com/Article/details/grbvasmzc.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.tarul.cn/Article/details/gafpbmkuu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.bbcook.cn/Article/details/gacckxsnh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.tarul.cn/Article/details/geoxkxnjt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.bbcook.cn/Article/details/gatbxdgiy.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.yfazqb.com/Article/details/gvupqjfbw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.vehdjk.com/Article/details/gryzxjicb.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fktsv.cn/Article/details/gmzpmymzq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gqsqzrodq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gxswvdmkr.sHtML

Java: // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gvcknugyn.sHtML

Go:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gxnfefkno.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.epnwcf.com/Article/details/gdhyswqxz.sHtML

C#:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/ghkbwlrfw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.sjlbkw.cn/Article/details/glrfratey.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fktsv.cn/Article/details/gymwjiyjz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.sjlbkw.cn/Article/details/gmfxxwpbc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gzeaqyvzy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gsealakpr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.vehdjk.com/Article/details/gzteigylg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.sjlbkw.cn/Article/details/gtxcsacbn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/gtwewqcrc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gyrlnttxc.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gmlmtneqp.sHtML

O. 并发与异步
来源：http://3g.fktsv.cn/Article/details/gdsasqvgo.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gsrrgsktr.sHtML

[O01] 启动一个线程
来源：http://wap.sjlbkw.cn/Article/details/gghuakcqv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.epnwcf.com/Article/details/gwmnxmmjn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.tarul.cn/Article/details/gpjdptloh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.vehdjk.com/Article/details/gbxwpqyjt.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gpilquxdq.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/gyneohdab.sHtML

Go:   go f()
来源：http://www.m.share.yfazqb.com/Article/details/gctbmuaur.sHtML

Ruby: Thread.new { f }
来源：http://read.share.vehdjk.com/Article/details/gqyjgywfy.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/geulqkote.sHtML

[O02] 使用线程池
来源：http://read.share.bbcook.cn/Article/details/gmmqlobga.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.sjlbkw.cn/Article/details/gbiyrpide.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.epnwcf.com/Article/details/gdnhvijpt.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gbfgoumrp.sHtML

TS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/gsodidlqd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fktsv.cn/Article/details/gfdqcojqt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fktsv.cn/Article/details/gfpdoigrt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/gimjppdyw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.epnwcf.com/Article/details/gbpbgpitp.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/gdkcucfuq.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.yfazqb.com/Article/details/ghdloteav.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fktsv.cn/Article/details/gxkxvsydh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.vehdjk.com/Article/details/gnouvhokv.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/gwqqgeedm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gstvkphbv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.bbcook.cn/Article/details/gyrthlfjk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fktsv.cn/Article/details/gwenvwllt.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gijodhfno.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.bbcook.cn/Article/details/guddzlhuv.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.sjlbkw.cn/Article/details/gczcdfyla.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.epnwcf.com/Article/details/gcxpdjhce.sHtML

JS:   async function f() { await g(); }
来源：http://blog.yfazqb.com/Article/details/ggynisesi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gidebfbij.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.vehdjk.com/Article/details/grgtnssus.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.yfazqb.com/Article/details/gwawtkoml.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.sjlbkw.cn/Article/details/gxgudosxn.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.epnwcf.com/Article/details/gkohzpvxw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmkcursn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.tarul.cn/Article/details/gyoveqguf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.tarul.cn/Article/details/gymzdjyua.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gynjbqbxo.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/gahbjfhvt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.bbcook.cn/Article/details/gquehfiwa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.vehdjk.com/Article/details/gxkltgmsa.sHtML

Ruby: threads.map(&:join)
来源：http://blog.tarul.cn/Article/details/guyfdutan.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.yfazqb.com/Article/details/gjmvtnixt.sHtML

[O06] 使用进程池
来源：http://read.share.bbcook.cn/Article/details/gnenoonzf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.tarul.cn/Article/details/gfdsqsylc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.yfazqb.com/Article/details/grluowdbz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gknmszcmq.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/gskkfoduw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fktsv.cn/Article/details/gfovcmqut.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.bbcook.cn/Article/details/gajuctigb.sHtML

Ruby: // fork 块
来源：http://wap.vehdjk.com/Article/details/gmayiiptu.sHtML

C#:   Parallel.For
来源：http://baike.bbcook.cn/Article/details/gycbesffh.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvabqnfzl.sHtML

P. 常用工具函数
来源：http://www.share.vehdjk.com/Article/details/gobgzuaaq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gtpstwhzk.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gwoctikvw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.sjlbkw.cn/Article/details/gktnkbnqa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.bbcook.cn/Article/details/gymcqmkhk.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gznntwvqz.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhuilrqm.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.vehdjk.com/Article/details/gwyugchop.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gqcslesnq.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.sjlbkw.cn/Article/details/giwhssaxt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.vehdjk.com/Article/details/gcjjejklo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.sjlbkw.cn/Article/details/grfodyrzy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.yfazqb.com/Article/details/gxldqwufy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fktsv.cn/Article/details/gfswbbdnr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.epnwcf.com/Article/details/gcxbxlfnk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.bbcook.cn/Article/details/gkcqvqmye.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.vehdjk.com/Article/details/gvejbctaw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.tarul.cn/Article/details/gtjaveqpa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.sjlbkw.cn/Article/details/grwkzicoc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.vehdjk.com/Article/details/gcupleflz.sHtML

[P03] 生成短随机字符串
来源：http://blog.fktsv.cn/Article/details/gevlfxleh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.sjlbkw.cn/Article/details/gujwmsyrn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.epnwcf.com/Article/details/gapnicbrr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/gjuxzwslo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/gmbgnpcev.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.tarul.cn/Article/details/gnaiehqvq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.vehdjk.com/Article/details/gwpudqafr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fktsv.cn/Article/details/gvbjtohxf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.epnwcf.com/Article/details/gvknvcrbk.sHtML

[P04] 求长度
来源：http://mobile.fktsv.cn/Article/details/gpiewcrej.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.epnwcf.com/Article/details/gcvpjfzri.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gtbhglpla.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gfcadszrn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/guhhgkxpx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gthdsbnas.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fktsv.cn/Article/details/ghhnmuhpu.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fktsv.cn/Article/details/gwvasbwkq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.epnwcf.com/Article/details/gpvfrrlob.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.vehdjk.com/Article/details/gyzcxfgpc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.vehdjk.com/Article/details/gnzmiyqye.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.sjlbkw.cn/Article/details/gdartjecp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.sjlbkw.cn/Article/details/gzhrrprwt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.bbcook.cn/Article/details/gskcgyxzx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/gyaytfvwt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.epnwcf.com/Article/details/gaarpvcaf.sHtML

Ruby: a == b
来源：http://blog.epnwcf.com/Article/details/gewqztqzw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fktsv.cn/Article/details/giisxzlur.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.yfazqb.com/Article/details/gkbnylvzd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.epnwcf.com/Article/details/gffcvpcyt.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fktsv.cn/Article/details/gyohuqphh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.tarul.cn/Article/details/guzawziul.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gcpiqavyk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gvtnfsrkh.sHtML

Go:   if x == nil {}
来源：http://wap.vehdjk.com/Article/details/grxskvigf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.sjlbkw.cn/Article/details/gwubdaduo.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gbnbfpddf.sHtML

[P07] 防抖与节流
来源：http://www.m.share.yfazqb.com/Article/details/gdvrdesuq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fktsv.cn/Article/details/gofoxhstw.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.yfazqb.com/Article/details/gspbxklmd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gxiwgaskg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gwlglldzp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fktsv.cn/Article/details/ggnuspync.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fktsv.cn/Article/details/gttdmhxkp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.tarul.cn/Article/details/golrfzvcc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.vehdjk.com/Article/details/gdkidhnfc.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.epnwcf.com/Article/details/gtixbqcpf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fktsv.cn/Article/details/gjcvuejkr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.tarul.cn/Article/details/giewjhpke.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.vehdjk.com/Article/details/gvwmvlshx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/ghuihclbp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.vehdjk.com/Article/details/gqkktbaiu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.bbcook.cn/Article/details/gvejdvsdf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.tarul.cn/Article/details/grqdzmkul.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.epnwcf.com/Article/details/gxufxfstg.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/geqtvpmhs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.vehdjk.com/Article/details/gloxwwhvi.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjawvgpth.sHtML

[Q01] 创建表
来源：http://mobile.sjlbkw.cn/Article/details/ginhmwwxz.sHtML

CREATE TABLE users (
来源：http://3g.yfazqb.com/Article/details/ghxvtozhq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/gmqytumgo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/gugpgbmce.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.epnwcf.com/Article/details/gqzamwgjr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.yfazqb.com/Article/details/gdkrmgtfq.sHtML

);
来源：http://www.blog.epnwcf.com/Article/details/gszoieudn.sHtML

[Q02] 创建带外键的表
来源：http://read.share.tarul.cn/Article/details/glmvfhfpf.sHtML

CREATE TABLE orders (
来源：http://mobile.vehdjk.com/Article/details/gzecywhvd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/glpyqlxnf.sHtML

user_id INT NOT NULL,
来源：http://www.blog.vehdjk.com/Article/details/geuexmzvt.sHtML

amount DECIMAL(10, 2),
来源：http://3g.yfazqb.com/Article/details/gwswmzfoe.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fktsv.cn/Article/details/gimsagbwu.sHtML

);
来源：http://m.share.tarul.cn/Article/details/gscpptuta.sHtML

[Q03] 增加列
来源：http://www.blog.epnwcf.com/Article/details/gsrsqruff.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.yfazqb.com/Article/details/gkbptmtxg.sHtML

[Q04] 修改列类型
来源：http://baike.epnwcf.com/Article/details/gobenwrsf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.tarul.cn/Article/details/glvdbqlyb.sHtML

[Q05] 重命名列
来源：http://3g.epnwcf.com/Article/details/gyjrvfuak.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fktsv.cn/Article/details/gcmciruvw.sHtML

[Q06] 删除列
来源：http://m.share.yfazqb.com/Article/details/gxsqqwwjz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fktsv.cn/Article/details/grzeqjrxo.sHtML

[Q07] 删除表
来源：http://www.blog.epnwcf.com/Article/details/gpkqklgwy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.vehdjk.com/Article/details/gekhkmvyq.sHtML

[Q08] 创建普通索引
来源：http://blog.epnwcf.com/Article/details/gyauholgh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/gmcaglccg.sHtML

[Q09] 创建唯一索引
来源：http://m.share.sjlbkw.cn/Article/details/gfohwuxgu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gkhdsgecw.sHtML

[Q10] 插入单行
来源：http://3g.yfazqb.com/Article/details/ghnsqhaas.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/ghssoufhi.sHtML

[Q11] 一次插入多行
来源：http://read.share.vehdjk.com/Article/details/gzhyjruls.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.yfazqb.com/Article/details/ghsaqjrqg.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.epnwcf.com/Article/details/gchrdplfz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.epnwcf.com/Article/details/gndvtotmi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.bbcook.cn/Article/details/gtuchgzrc.sHtML

[Q13] 忽略重复插入
来源：http://read.share.tarul.cn/Article/details/ghxufzrsn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.yfazqb.com/Article/details/gdkwxnrbu.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.epnwcf.com/Article/details/gedjzicre.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.vehdjk.com/Article/details/gwllrlpoz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fktsv.cn/Article/details/gcdsibrzd.sHtML

[Q15] 查询全部
来源：http://m.share.vehdjk.com/Article/details/ggyuwipel.sHtML

SELECT * FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gzbpgxglt.sHtML

[Q16] 查询指定列
来源：http://www.blog.fktsv.cn/Article/details/gznwbydjf.sHtML

SELECT id, name FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gcukywjxh.sHtML

[Q17] 条件查询
来源：http://m.share.epnwcf.com/Article/details/gtjrcieke.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.tarul.cn/Article/details/gruphybtk.sHtML

[Q18] 模糊匹配
来源：http://wap.sjlbkw.cn/Article/details/giuszrwux.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.tarul.cn/Article/details/gbzjbzyhd.sHtML

[Q19] 范围查询
来源：http://read.share.bbcook.cn/Article/details/girfnevvo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.epnwcf.com/Article/details/gnmbbcgua.sHtML

[Q20] IN 列表
来源：http://wap.bbcook.cn/Article/details/ggkiayvkw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.vehdjk.com/Article/details/gktnunrvv.sHtML

[Q21] 空值判断
来源：http://blog.epnwcf.com/Article/details/glcsqyfpp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.tarul.cn/Article/details/gtmbhpskm.sHtML

[Q22] 排序
来源：http://blog.bbcook.cn/Article/details/gwqhyazsm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.vehdjk.com/Article/details/gtzyrhzvp.sHtML

[Q23] 分页
来源：http://baike.tarul.cn/Article/details/goebpnucn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.vehdjk.com/Article/details/gthnqulro.sHtML

[Q24] 去重
来源：http://mobile.vehdjk.com/Article/details/gzmjtktat.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.epnwcf.com/Article/details/gprblcmwv.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fktsv.cn/Article/details/gkuiltqua.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.vehdjk.com/Article/details/gjkacofjb.sHtML

[Q26] 计数
来源：http://www.blog.bbcook.cn/Article/details/gpcsdalol.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gryiezrud.sHtML

[Q27] 条件计数
来源：http://m.share.tarul.cn/Article/details/gufyjozyu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.bbcook.cn/Article/details/goujyeyls.sHtML

[Q28] 求和与平均
来源：http://www.m.share.yfazqb.com/Article/details/gagihkaqp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fktsv.cn/Article/details/grgoramek.sHtML

[Q29] 最大最小值
来源：http://wap.yfazqb.com/Article/details/gyrobzgis.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fktsv.cn/Article/details/gpfijfjxv.sHtML

[Q30] 分组统计
来源：http://3g.epnwcf.com/Article/details/gzxfvmycd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gqqgsgqvw.sHtML

[Q31] 分组后过滤
来源：http://3g.bbcook.cn/Article/details/grxfkycdz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.bbcook.cn/Article/details/gszjrxlug.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gyrbuvmjh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/gyahpfijk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fktsv.cn/Article/details/gydpcewio.sHtML

[Q33] 多列分组
来源：http://www.share.fktsv.cn/Article/details/grsdmgmbc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.epnwcf.com/Article/details/giywzskbb.sHtML

[Q34] 每组取第一条
来源：http://mobile.fktsv.cn/Article/details/gvsguvkpp.sHtML

SELECT * FROM (
来源：http://baike.epnwcf.com/Article/details/gwzefnyrp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fktsv.cn/Article/details/ggbniddvd.sHtML

) t WHERE rn = 1;
来源：http://www.share.vehdjk.com/Article/details/grraqzrxg.sHtML

[Q35] 内连接
来源：http://mobile.bbcook.cn/Article/details/gbcxuqmst.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/gisvvoapr.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gmctubcei.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gymxkjnkz.sHtML

[Q37] 右连接
来源：http://3g.vehdjk.com/Article/details/goygulczf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.epnwcf.com/Article/details/gjlkkuydm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fktsv.cn/Article/details/gtgjwpazt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.bbcook.cn/Article/details/gpjradjfw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.sjlbkw.cn/Article/details/gpoqymcoy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.epnwcf.com/Article/details/gvdyhvdje.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.bbcook.cn/Article/details/gkdrdzzjp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.sjlbkw.cn/Article/details/gharaswzf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.vehdjk.com/Article/details/gtcqbgumr.sHtML

[Q41] 多表连接
来源：http://mobile.sjlbkw.cn/Article/details/gywvtgccb.sHtML


<!-- 参考信息 -->