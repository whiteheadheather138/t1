代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.yfazqb.com/Article/details/gothszmns.sHtML

[N06] 判断回文字符串
来源：http://www.share.vehdjk.com/Article/details/gzrnqnecs.sHtML

Py:   s == s[::-1]
来源：http://blog.vehdjk.com/Article/details/gdkzqunoo.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.vehdjk.com/Article/details/gienigtyq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gspchhmje.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gngxzwcxy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.tarul.cn/Article/details/gapbgaepr.sHtML

Go:   // 双指针从两端比较
来源：http://baike.epnwcf.com/Article/details/gzxgimvoj.sHtML

Ruby: s == s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gmicmadqf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gaohohowh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/gnoniiyfx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.epnwcf.com/Article/details/gkdddfqlu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fktsv.cn/Article/details/gdigxxfhv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fktsv.cn/Article/details/gysfveics.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.vehdjk.com/Article/details/grhohxyhn.sHtML

Java: // 手写 HashMap
来源：http://www.blog.epnwcf.com/Article/details/gxxugkjen.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.sjlbkw.cn/Article/details/gwyhzfyli.sHtML

Ruby: // 手写 Hash
来源：http://baike.sjlbkw.cn/Article/details/gqxcxlcvx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.vehdjk.com/Article/details/ghimmbhst.sHtML

[N08] 生成全排列
来源：http://www.m.share.tarul.cn/Article/details/geqifxlcl.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.epnwcf.com/Article/details/gbkxwzpps.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.yfazqb.com/Article/details/gqktvucot.sHtML

JS:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gooiivuzu.sHtML

TS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/ghtmqkqlg.sHtML

Java: // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/ghcorlako.sHtML

Go:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gegelzztv.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.vehdjk.com/Article/details/gprlersqn.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gmeogomwm.sHtML

[N09] 栈与队列
来源：http://mobile.epnwcf.com/Article/details/gfxhlvmrv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.vehdjk.com/Article/details/gfpzaudbj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.bbcook.cn/Article/details/guigcnkxp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gkfzmztgm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.sjlbkw.cn/Article/details/gywwjpyrf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gtqtchjsg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.yfazqb.com/Article/details/gsitgfjxw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/gdxcypzfq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.yfazqb.com/Article/details/gsngcqcif.sHtML

[N10] 链表节点定义
来源：http://3g.tarul.cn/Article/details/gkxpeefaf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.yfazqb.com/Article/details/gdfxgnjvg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.tarul.cn/Article/details/gshkmzmem.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.vehdjk.com/Article/details/grbhczpke.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.vehdjk.com/Article/details/gqpuldiqc.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.sjlbkw.cn/Article/details/gilldgauc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.yfazqb.com/Article/details/ggnesjdok.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.sjlbkw.cn/Article/details/gwovhpjhd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/gokuudjyc.sHtML

[N11] 二叉树中序遍历
来源：http://baike.epnwcf.com/Article/details/gtrtrerwo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.vehdjk.com/Article/details/gsbdndrss.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.vehdjk.com/Article/details/guqrzrbmm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gfrrvncti.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gxbwpjcfk.sHtML

Java: // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gahsrufkg.sHtML

Go:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gcdhgvdft.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.epnwcf.com/Article/details/gkefqdcix.sHtML

C#:   // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gokjcivwh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.yfazqb.com/Article/details/gdcwocckb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.yfazqb.com/Article/details/gplqgrora.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.yfazqb.com/Article/details/gnyjfejqw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gcqlvtozn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gcgejkvie.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/guknonybz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.vehdjk.com/Article/details/gdeuyttmt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.tarul.cn/Article/details/gfdxaridt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/gfiwfrneq.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbkgcolme.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/gabptgeen.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gutzcctcp.sHtML

[O01] 启动一个线程
来源：http://3g.fktsv.cn/Article/details/gjhxzueze.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.epnwcf.com/Article/details/gybykcqvz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/gpxwbrdoa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.epnwcf.com/Article/details/gydrrfrou.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gxiwsjlqa.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.bbcook.cn/Article/details/guyubztbb.sHtML

Go:   go f()
来源：http://www.blog.bbcook.cn/Article/details/glckqnwbp.sHtML

Ruby: Thread.new { f }
来源：http://3g.vehdjk.com/Article/details/gqcueshdq.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.sjlbkw.cn/Article/details/gizyyrela.sHtML

[O02] 使用线程池
来源：http://wap.fktsv.cn/Article/details/gnxgumhyg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.sjlbkw.cn/Article/details/gqzlbhybz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.tarul.cn/Article/details/gojwqbcyg.sHtML

JS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/genfghcde.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/gfnwawowl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.sjlbkw.cn/Article/details/gefhakzwb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.vehdjk.com/Article/details/geaavjyjx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.tarul.cn/Article/details/ghztvawtr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.sjlbkw.cn/Article/details/gnipqczih.sHtML

[O03] 加锁保护共享数据
来源：http://baike.epnwcf.com/Article/details/gasfyynpq.sHtML

Py:   with lock: shared += 1
来源：http://wap.yfazqb.com/Article/details/gktbpkhez.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.epnwcf.com/Article/details/gbrvirhin.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.tarul.cn/Article/details/gylnnitut.sHtML

TS:   // 同 JS
来源：http://www.blog.tarul.cn/Article/details/gyijqwndi.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.yfazqb.com/Article/details/gjhwrndbr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fktsv.cn/Article/details/glzofjcjz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.epnwcf.com/Article/details/gbexjyxol.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.yfazqb.com/Article/details/gnprockpf.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gqtnnlcbm.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.vehdjk.com/Article/details/gpmgvzcec.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.sjlbkw.cn/Article/details/gamqzduqr.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.bbcook.cn/Article/details/gmnevmfhg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.epnwcf.com/Article/details/gkstvumdd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.bbcook.cn/Article/details/gzefstceo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.tarul.cn/Article/details/gjwhcgkca.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.vehdjk.com/Article/details/gxlbynaut.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.epnwcf.com/Article/details/gxyiplohr.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.yfazqb.com/Article/details/gpsbhunre.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/gziqwuybn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fktsv.cn/Article/details/gynasoukz.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gvkyhzbwo.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gcqmpxvdf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.yfazqb.com/Article/details/gjnkcvlae.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.vehdjk.com/Article/details/ggvsnidqg.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.vehdjk.com/Article/details/gctxmtbkn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.yfazqb.com/Article/details/gtirivoye.sHtML

[O06] 使用进程池
来源：http://wap.epnwcf.com/Article/details/gkjnzxcuf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.sjlbkw.cn/Article/details/govucwxez.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.vehdjk.com/Article/details/gzopbmhbx.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/ghoobtwrt.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/gkpdpjegk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.epnwcf.com/Article/details/goinizbig.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.tarul.cn/Article/details/gzbcaktdb.sHtML

Ruby: // fork 块
来源：http://3g.bbcook.cn/Article/details/gzsutycdh.sHtML

C#:   Parallel.For
来源：http://3g.fktsv.cn/Article/details/gzfarmhhj.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gsqqepcbk.sHtML

P. 常用工具函数
来源：http://www.share.epnwcf.com/Article/details/gzryupwef.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gejwpxygj.sHtML

[P01] 生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/ghqoxdfyo.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.tarul.cn/Article/details/gfvrojaei.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/glnmhowyr.sHtML

JS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gfgmxutgg.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gmjxkbkwo.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fktsv.cn/Article/details/ghnbcfkjt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gmfttwdag.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fktsv.cn/Article/details/gnswzwmob.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.vehdjk.com/Article/details/glibxwsbe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fktsv.cn/Article/details/glxmffcve.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.yfazqb.com/Article/details/gwwmrqorp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.vehdjk.com/Article/details/glrlwrjnf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.vehdjk.com/Article/details/geclclhub.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.vehdjk.com/Article/details/gkccxhywa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.bbcook.cn/Article/details/gufpdhhuz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzotvycfd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/ghxotnpxs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.epnwcf.com/Article/details/gfjetrwhv.sHtML

[P03] 生成短随机字符串
来源：http://read.share.bbcook.cn/Article/details/gkmzzyzxd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.bbcook.cn/Article/details/gcgsxdmfv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.yfazqb.com/Article/details/gdxymqfbk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.tarul.cn/Article/details/gdyocelgc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/gcmqqzbmg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fktsv.cn/Article/details/gszkrllsz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.sjlbkw.cn/Article/details/gzkpwwxjj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.bbcook.cn/Article/details/ghudpvozr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.epnwcf.com/Article/details/grxehyolm.sHtML

[P04] 求长度
来源：http://read.share.sjlbkw.cn/Article/details/gapvqmuny.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.sjlbkw.cn/Article/details/gxvsxwjpa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gjlomtulw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gyfxjfjhe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/gcwqipctd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.yfazqb.com/Article/details/gdrmmvtmy.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.bbcook.cn/Article/details/gfodxueqj.sHtML

Ruby: x.length;  x.size
来源：http://3g.sjlbkw.cn/Article/details/geljrfhnj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/gwnhcddgo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.epnwcf.com/Article/details/gtycrlgeg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.epnwcf.com/Article/details/gkrsxqncs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.sjlbkw.cn/Article/details/gitbwqjqj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.epnwcf.com/Article/details/gpruzgcge.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/gxrhrqwlf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.tarul.cn/Article/details/gbffxyrzc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fktsv.cn/Article/details/glxplfefj.sHtML

Ruby: a == b
来源：http://m.share.tarul.cn/Article/details/gkdjfalbq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.yfazqb.com/Article/details/gjdptoohr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.tarul.cn/Article/details/gvlmrlgcg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.sjlbkw.cn/Article/details/gaplrpsbl.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.yfazqb.com/Article/details/golwcopyb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.tarul.cn/Article/details/gzdhkdtuo.sHtML

TS:   if (x == null) {}
来源：http://mobile.vehdjk.com/Article/details/gzqfeokhy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/gzujenvpq.sHtML

Go:   if x == nil {}
来源：http://www.share.sjlbkw.cn/Article/details/goczvfrki.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.yfazqb.com/Article/details/gzupfnhyu.sHtML

C#:   if (x is null) {}
来源：http://mobile.yfazqb.com/Article/details/gimttnycv.sHtML

[P07] 防抖与节流
来源：http://blog.bbcook.cn/Article/details/gozlrxhry.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.epnwcf.com/Article/details/gidmescno.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.vehdjk.com/Article/details/grckfltjn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gnnlmuvzn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gvlgheckc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.epnwcf.com/Article/details/goatxrooa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.sjlbkw.cn/Article/details/ggboosyvm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.bbcook.cn/Article/details/gnnfujsvi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.epnwcf.com/Article/details/gdykobzky.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.epnwcf.com/Article/details/gqdzqwkox.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.vehdjk.com/Article/details/gixpgrxme.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.bbcook.cn/Article/details/gddqagjha.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.bbcook.cn/Article/details/gtecgiahi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.vehdjk.com/Article/details/gzsawpnkm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fktsv.cn/Article/details/gohqqjije.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fktsv.cn/Article/details/gjrlqqfbb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.sjlbkw.cn/Article/details/gemxzdvmv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.epnwcf.com/Article/details/gmcghcaqr.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gmjjrknpj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.bbcook.cn/Article/details/gsggyvuwb.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmwfkvjak.sHtML

[Q01] 创建表
来源：http://read.share.bbcook.cn/Article/details/grvtugzma.sHtML

CREATE TABLE users (
来源：http://wap.tarul.cn/Article/details/gqxqstuuv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gmjxkyqsc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/gttkfqfjg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.vehdjk.com/Article/details/gmqyijlca.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.tarul.cn/Article/details/givzgbtjc.sHtML

);
来源：http://baike.vehdjk.com/Article/details/gxtvndxyg.sHtML

[Q02] 创建带外键的表
来源：http://3g.bbcook.cn/Article/details/gdnpztcwo.sHtML

CREATE TABLE orders (
来源：http://www.blog.bbcook.cn/Article/details/glsxkjyje.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/gjodugvpq.sHtML

user_id INT NOT NULL,
来源：http://www.blog.sjlbkw.cn/Article/details/gyczxdatx.sHtML

amount DECIMAL(10, 2),
来源：http://baike.bbcook.cn/Article/details/gsjuqnuof.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.bbcook.cn/Article/details/gcshamycv.sHtML

);
来源：http://www.m.share.yfazqb.com/Article/details/gydrebmea.sHtML

[Q03] 增加列
来源：http://baike.bbcook.cn/Article/details/gnhwzygni.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.sjlbkw.cn/Article/details/gnlczidoc.sHtML

[Q04] 修改列类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrnoyrtb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fktsv.cn/Article/details/gctepjxdf.sHtML

[Q05] 重命名列
来源：http://read.share.vehdjk.com/Article/details/gmiqxjxdz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.vehdjk.com/Article/details/gjbkaaasp.sHtML

[Q06] 删除列
来源：http://read.share.vehdjk.com/Article/details/gjnalmiya.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.tarul.cn/Article/details/ghqfghlwf.sHtML

[Q07] 删除表
来源：http://mobile.sjlbkw.cn/Article/details/gsjdnumtk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.bbcook.cn/Article/details/ghuwbwvmt.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.tarul.cn/Article/details/gziktuoya.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gkibxtrkq.sHtML

[Q09] 创建唯一索引
来源：http://blog.tarul.cn/Article/details/gzwxmcvym.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/gxnyouhpt.sHtML

[Q10] 插入单行
来源：http://www.m.share.bbcook.cn/Article/details/gmomnomio.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.epnwcf.com/Article/details/gzvfkxlzg.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fktsv.cn/Article/details/gtigilewz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.yfazqb.com/Article/details/geiqcxsrf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fktsv.cn/Article/details/gifreugdx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.yfazqb.com/Article/details/griskkpdn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.sjlbkw.cn/Article/details/glskqegcc.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fktsv.cn/Article/details/gvojlbcfi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gavmzdums.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.epnwcf.com/Article/details/gozrwpkfw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.tarul.cn/Article/details/gbloljifq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.yfazqb.com/Article/details/gehfaecgw.sHtML

[Q15] 查询全部
来源：http://blog.yfazqb.com/Article/details/gqjgqgjdo.sHtML

SELECT * FROM users;
来源：http://m.share.bbcook.cn/Article/details/getsklqyz.sHtML

[Q16] 查询指定列
来源：http://blog.sjlbkw.cn/Article/details/gimpdfcdj.sHtML

SELECT id, name FROM users;
来源：http://wap.vehdjk.com/Article/details/gqeidevmf.sHtML

[Q17] 条件查询
来源：http://blog.fktsv.cn/Article/details/gcxyjymmh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.bbcook.cn/Article/details/gaqxvegig.sHtML

[Q18] 模糊匹配
来源：http://3g.bbcook.cn/Article/details/gdgrtudtp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.vehdjk.com/Article/details/gfisdclcn.sHtML

[Q19] 范围查询
来源：http://3g.yfazqb.com/Article/details/gfrqvygrb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.tarul.cn/Article/details/gufekcfio.sHtML

[Q20] IN 列表
来源：http://www.m.share.epnwcf.com/Article/details/gvffcctbr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.yfazqb.com/Article/details/gtuhvmveb.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gytnoshjl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.tarul.cn/Article/details/ghzpuhwkq.sHtML

[Q22] 排序
来源：http://www.share.tarul.cn/Article/details/gzwjkwmxy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.vehdjk.com/Article/details/grijwqdos.sHtML

[Q23] 分页
来源：http://www.m.share.bbcook.cn/Article/details/gwcdpifqg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fktsv.cn/Article/details/gddcugwnn.sHtML

[Q24] 去重
来源：http://wap.yfazqb.com/Article/details/gqmwspbnl.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.vehdjk.com/Article/details/gfeqxrfte.sHtML

[Q25] 只取前 N 条
来源：http://blog.fktsv.cn/Article/details/geiyjtyey.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fktsv.cn/Article/details/gdldwrbra.sHtML

[Q26] 计数
来源：http://baike.tarul.cn/Article/details/grpqrwnmt.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.bbcook.cn/Article/details/gsocdgqfp.sHtML

[Q27] 条件计数
来源：http://mobile.sjlbkw.cn/Article/details/gqlskkjth.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.tarul.cn/Article/details/grhklntnm.sHtML

[Q28] 求和与平均
来源：http://wap.bbcook.cn/Article/details/gzemfbszw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gyxlpjurx.sHtML

[Q29] 最大最小值
来源：http://mobile.yfazqb.com/Article/details/gfxnzpbjb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.epnwcf.com/Article/details/gjeftkhbj.sHtML

[Q30] 分组统计
来源：http://3g.vehdjk.com/Article/details/gjcuyffrq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gaqmmxold.sHtML

[Q31] 分组后过滤
来源：http://read.share.epnwcf.com/Article/details/gtsnpuyzm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.vehdjk.com/Article/details/gwwjmgxji.sHtML

[Q32] 分组拼接字符串
来源：http://3g.epnwcf.com/Article/details/gscvhdhxw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/grtieqeew.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbghtfgy.sHtML

[Q33] 多列分组
来源：http://baike.bbcook.cn/Article/details/gqytxamqe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.yfazqb.com/Article/details/girdhizqk.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.vehdjk.com/Article/details/gagrwlrou.sHtML

SELECT * FROM (
来源：http://3g.tarul.cn/Article/details/gfgfzrmiw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fktsv.cn/Article/details/gfrkohnwf.sHtML

) t WHERE rn = 1;
来源：http://3g.bbcook.cn/Article/details/gdkvsesul.sHtML

[Q35] 内连接
来源：http://mobile.vehdjk.com/Article/details/gskpbwoye.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gimwcgosw.sHtML

[Q36] 左连接
来源：http://www.share.vehdjk.com/Article/details/gaubvdloq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.sjlbkw.cn/Article/details/gflcypgbj.sHtML

[Q37] 右连接
来源：http://www.share.sjlbkw.cn/Article/details/gvhnecddh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.sjlbkw.cn/Article/details/gwzluexkn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.vehdjk.com/Article/details/gdzsmdnjg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.bbcook.cn/Article/details/gikjyhirk.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.bbcook.cn/Article/details/gwgaqchgn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.yfazqb.com/Article/details/gmlllzwxx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.yfazqb.com/Article/details/ggwptbpgm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.tarul.cn/Article/details/gousjfare.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.sjlbkw.cn/Article/details/gqgwvbwkr.sHtML

[Q41] 多表连接
来源：http://3g.bbcook.cn/Article/details/gxeoqgyem.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.tarul.cn/Article/details/glljerork.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.bbcook.cn/Article/details/gekoxrumm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fktsv.cn/Article/details/gmqamdfem.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.bbcook.cn/Article/details/gmbpajoul.sHtML


<!-- 参考信息 -->