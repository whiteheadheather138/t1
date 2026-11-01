代发 wailian999

[N05] 最大公约数
来源：http://m.share.vehdjk.com/Article/details/gkrasdzoh.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gotiuqmtn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.vehdjk.com/Article/details/gblkvypdy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/grtjixgri.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gowvsboht.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.epnwcf.com/Article/details/gvushbtzt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fktsv.cn/Article/details/gyvzzhehe.sHtML

Ruby: a.gcd(b)
来源：http://www.share.tarul.cn/Article/details/glelywcgg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.vehdjk.com/Article/details/gvyfgiuou.sHtML

[N06] 判断回文字符串
来源：http://blog.epnwcf.com/Article/details/gjzlzgjov.sHtML

Py:   s == s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/grfzcmbyb.sHtML

PHP:  $s === strrev($s);
来源：http://3g.epnwcf.com/Article/details/gcewwtijb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gycyfighy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gfclfvhpz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.tarul.cn/Article/details/gxscjlfkw.sHtML

Go:   // 双指针从两端比较
来源：http://blog.vehdjk.com/Article/details/gvhidvlyi.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gzlisezfs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gcxcwxaxu.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.epnwcf.com/Article/details/ggifhyxde.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.bbcook.cn/Article/details/grtxiwhvz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/gjmxgkadz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fktsv.cn/Article/details/gtgzyehuw.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gutlubgsp.sHtML

Java: // 手写 HashMap
来源：http://baike.bbcook.cn/Article/details/gayurjuhm.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.vehdjk.com/Article/details/gmucxxljt.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fktsv.cn/Article/details/gdmexwcwa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.bbcook.cn/Article/details/gyxlymkgm.sHtML

[N08] 生成全排列
来源：http://read.share.fktsv.cn/Article/details/gmdawoexl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.epnwcf.com/Article/details/gypehpxtc.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fktsv.cn/Article/details/ghtznzals.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gvkmocxqk.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gismrrlbh.sHtML

Java: // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gfnyqkcof.sHtML

Go:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gqssywxrg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.vehdjk.com/Article/details/gcalgapje.sHtML

C#:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/grhgannam.sHtML

[N09] 栈与队列
来源：http://baike.bbcook.cn/Article/details/gkidbugsw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.tarul.cn/Article/details/ghtrarjxo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gnprgnrhp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gqfjeuuix.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.tarul.cn/Article/details/gplrybqdd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/ggjgltyfk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.tarul.cn/Article/details/gpqdxdajx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gmdrkaetx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fktsv.cn/Article/details/gkugmqfil.sHtML

[N10] 链表节点定义
来源：http://www.m.share.yfazqb.com/Article/details/gpggdgltx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.bbcook.cn/Article/details/ghuuxyryr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.sjlbkw.cn/Article/details/gjfcxflry.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gybvpldka.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.vehdjk.com/Article/details/gpeyufhpx.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.bbcook.cn/Article/details/gqjwlkgjc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.vehdjk.com/Article/details/gbygbwirw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.yfazqb.com/Article/details/gbxccuckz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlrbwtef.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.yfazqb.com/Article/details/gylakpyvk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.yfazqb.com/Article/details/gqohgmdea.sHtML

PHP:  // 手写递归函数
来源：http://www.share.epnwcf.com/Article/details/ghkhgjbcu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gefasggnc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gyxgkgoeu.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/gcblvdcer.sHtML

Go:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gnsdnvstt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.vehdjk.com/Article/details/gfsznamzf.sHtML

C#:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gmtlvsshb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.yfazqb.com/Article/details/gygzdlrzn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.vehdjk.com/Article/details/gabgocycq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fktsv.cn/Article/details/geqxggzik.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/grtjivwin.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.bbcook.cn/Article/details/gvizoekvl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/gqcsihvqi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.epnwcf.com/Article/details/gtsckuumk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.bbcook.cn/Article/details/giivsmsje.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gnggnzljy.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gosnjjpuw.sHtML

O. 并发与异步
来源：http://wap.vehdjk.com/Article/details/gfymmsgly.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gwjzonjkc.sHtML

[O01] 启动一个线程
来源：http://www.blog.yfazqb.com/Article/details/ggkakaswr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.tarul.cn/Article/details/gkhlojpnd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.tarul.cn/Article/details/gnqtjqguk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fktsv.cn/Article/details/gyerknido.sHtML

TS:   // 同 JS
来源：http://www.share.vehdjk.com/Article/details/gcruskazs.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fktsv.cn/Article/details/guvtrtvqc.sHtML

Go:   go f()
来源：http://m.share.fktsv.cn/Article/details/gvjabguqk.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/gcvocaalq.sHtML

C#:   Task.Run(() => F());
来源：http://baike.sjlbkw.cn/Article/details/gyvpmscqb.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/gjgndekxk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzolxxcb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.bbcook.cn/Article/details/gemwwrhid.sHtML

JS:   // worker_threads 线程池
来源：http://3g.vehdjk.com/Article/details/gdiyqwisg.sHtML

TS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/goejxcnpd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.yfazqb.com/Article/details/gifgupbyd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.bbcook.cn/Article/details/ggcunufvc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.vehdjk.com/Article/details/gamgoqlwg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fktsv.cn/Article/details/gudivzlje.sHtML

[O03] 加锁保护共享数据
来源：http://wap.epnwcf.com/Article/details/gybzsdrfi.sHtML

Py:   with lock: shared += 1
来源：http://www.share.yfazqb.com/Article/details/geedqvbad.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.bbcook.cn/Article/details/gkfcenwuw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fktsv.cn/Article/details/gvgfualce.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gsueelofd.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gbusomxsf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fktsv.cn/Article/details/ggxrlhoya.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.vehdjk.com/Article/details/gmufyxmgl.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.epnwcf.com/Article/details/grxeymtjx.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.tarul.cn/Article/details/glrxvwttw.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.bbcook.cn/Article/details/gjcmtkvtb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.epnwcf.com/Article/details/goxhmjxjz.sHtML

JS:   async function f() { await g(); }
来源：http://blog.yfazqb.com/Article/details/grgwseayg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/goqkavxjs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.yfazqb.com/Article/details/gxdvywotp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fktsv.cn/Article/details/gkecqubzg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.bbcook.cn/Article/details/glnacqxkc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/giowyxlfs.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.bbcook.cn/Article/details/gzsatgckw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fktsv.cn/Article/details/gmogsjslx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.epnwcf.com/Article/details/gyrmlpyka.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/gdnnkqcrq.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gsuoustwn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.vehdjk.com/Article/details/gojkjghfe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.yfazqb.com/Article/details/gcdfidqbh.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/ghhiafcwb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gwtphwnyo.sHtML

[O06] 使用进程池
来源：http://m.share.tarul.cn/Article/details/gzeejdgpo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.epnwcf.com/Article/details/gyhurfseb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.tarul.cn/Article/details/gnmnilyov.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gsqvopwue.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/gubazwvrx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.bbcook.cn/Article/details/guzhgurem.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.tarul.cn/Article/details/gscatwvzu.sHtML

Ruby: // fork 块
来源：http://3g.yfazqb.com/Article/details/gecvxbvhq.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/ghvcawyoc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grrouljws.sHtML

P. 常用工具函数
来源：http://mobile.vehdjk.com/Article/details/gvmqesegn.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gymhudvul.sHtML

[P01] 生成 UUID
来源：http://blog.epnwcf.com/Article/details/glgfcfaro.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.bbcook.cn/Article/details/giikepgvk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.tarul.cn/Article/details/gpsjodctv.sHtML

JS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/guzwoxgvt.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gvmszovoa.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fktsv.cn/Article/details/geyzbghxu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.sjlbkw.cn/Article/details/geprzdpws.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/gwkuxjrxy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.bbcook.cn/Article/details/gvmydvhvv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.bbcook.cn/Article/details/gjllteeet.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.sjlbkw.cn/Article/details/gbndxlosy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.bbcook.cn/Article/details/gqlrkygje.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.bbcook.cn/Article/details/goqqubfni.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.epnwcf.com/Article/details/guggwwtxb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gtitsxtjp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.yfazqb.com/Article/details/galxdverq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.vehdjk.com/Article/details/gkledodwr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.tarul.cn/Article/details/glznmdsmd.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/gjkfgnhso.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.sjlbkw.cn/Article/details/ggjkqpfmi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.vehdjk.com/Article/details/gbeymzwns.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/glxdjetvk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/girrcixds.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.tarul.cn/Article/details/gfjqtqrbv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.sjlbkw.cn/Article/details/gknizaosy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.epnwcf.com/Article/details/gvejgmhgh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.sjlbkw.cn/Article/details/ggiqytgdt.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/gacpqbysr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.epnwcf.com/Article/details/gcotwnszx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/ghjoxproa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/gqlbuxljj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/ghkitfvpd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gcilbqkbu.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fktsv.cn/Article/details/gqxsdrjkf.sHtML

Ruby: x.length;  x.size
来源：http://mobile.epnwcf.com/Article/details/ggukpbrif.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.yfazqb.com/Article/details/gdmlcrwbu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyvdoxgy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.tarul.cn/Article/details/geosazebo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fktsv.cn/Article/details/galgeehqj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/gdhycreiq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/gazfuempa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.yfazqb.com/Article/details/gbqkcmqgr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.tarul.cn/Article/details/ghdbveoal.sHtML

Ruby: a == b
来源：http://read.share.fktsv.cn/Article/details/gylmtunpn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.bbcook.cn/Article/details/gxusdbytl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.vehdjk.com/Article/details/ghgxktbud.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.yfazqb.com/Article/details/gaqrjidmb.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fktsv.cn/Article/details/gkffxfxwo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.tarul.cn/Article/details/ghrxunoir.sHtML

TS:   if (x == null) {}
来源：http://wap.yfazqb.com/Article/details/gowwntpwx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gikmixtht.sHtML

Go:   if x == nil {}
来源：http://read.share.bbcook.cn/Article/details/guwieuual.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.epnwcf.com/Article/details/guxaywray.sHtML

C#:   if (x is null) {}
来源：http://m.share.fktsv.cn/Article/details/gsolrstxh.sHtML

[P07] 防抖与节流
来源：http://blog.epnwcf.com/Article/details/ggekwzpyp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.sjlbkw.cn/Article/details/gypadqtzc.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.bbcook.cn/Article/details/gpdinqbms.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/glcxnmjtp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gspuejxpq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.sjlbkw.cn/Article/details/gznlgftmm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.sjlbkw.cn/Article/details/gcigdresr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.bbcook.cn/Article/details/gjixjmcyi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.vehdjk.com/Article/details/gnhipzmuc.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.bbcook.cn/Article/details/gufervbvd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.epnwcf.com/Article/details/gvynbbmcs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.epnwcf.com/Article/details/gcoxvnjry.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.tarul.cn/Article/details/goszqhrdn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.yfazqb.com/Article/details/gmrgsllfc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.bbcook.cn/Article/details/gizhmkcln.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.bbcook.cn/Article/details/gsmufxwak.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.vehdjk.com/Article/details/gigzvmieq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.sjlbkw.cn/Article/details/gbgtbpdcx.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gosuwuxri.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.epnwcf.com/Article/details/gigyhrbst.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/guschrjxj.sHtML

[Q01] 创建表
来源：http://3g.epnwcf.com/Article/details/grpfnzwuw.sHtML

CREATE TABLE users (
来源：http://wap.sjlbkw.cn/Article/details/gclrkjkqk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/gctnmvhuw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.vehdjk.com/Article/details/gxqkhsfta.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fktsv.cn/Article/details/gtlkhnwxh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.tarul.cn/Article/details/gwfeppopn.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/ggvokmwia.sHtML

[Q02] 创建带外键的表
来源：http://baike.yfazqb.com/Article/details/gbcvikgkz.sHtML

CREATE TABLE orders (
来源：http://blog.sjlbkw.cn/Article/details/gsjdtbyrx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.epnwcf.com/Article/details/geujejkff.sHtML

user_id INT NOT NULL,
来源：http://wap.epnwcf.com/Article/details/gghoumlhh.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.sjlbkw.cn/Article/details/gigmwhgvf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.tarul.cn/Article/details/gvlpdofgu.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/guzlnlymt.sHtML

[Q03] 增加列
来源：http://m.share.vehdjk.com/Article/details/gselgsutu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.yfazqb.com/Article/details/gpqqrwghl.sHtML

[Q04] 修改列类型
来源：http://www.share.sjlbkw.cn/Article/details/gnflcripq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.bbcook.cn/Article/details/gmrueedox.sHtML

[Q05] 重命名列
来源：http://blog.vehdjk.com/Article/details/gtopmcszp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.tarul.cn/Article/details/gilrtlckf.sHtML

[Q06] 删除列
来源：http://www.share.vehdjk.com/Article/details/gtaymmyot.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.bbcook.cn/Article/details/gauppahfx.sHtML

[Q07] 删除表
来源：http://mobile.vehdjk.com/Article/details/gaurnzpby.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fktsv.cn/Article/details/galissmcs.sHtML

[Q08] 创建普通索引
来源：http://3g.epnwcf.com/Article/details/gpnspcubr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/giwmpsoey.sHtML

[Q09] 创建唯一索引
来源：http://mobile.sjlbkw.cn/Article/details/gfrqiiivy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fktsv.cn/Article/details/gjbpghwas.sHtML

[Q10] 插入单行
来源：http://3g.sjlbkw.cn/Article/details/gamjfbmxk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gulrvycad.sHtML

[Q11] 一次插入多行
来源：http://www.share.fktsv.cn/Article/details/gkupklnaj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.epnwcf.com/Article/details/gygxrmuep.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.sjlbkw.cn/Article/details/gchlmonvv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.bbcook.cn/Article/details/gmwfmpros.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/gaznyltmm.sHtML

[Q13] 忽略重复插入
来源：http://read.share.sjlbkw.cn/Article/details/gtknfpemb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fktsv.cn/Article/details/gklniqjzy.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.vehdjk.com/Article/details/glmzuuxno.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.tarul.cn/Article/details/giupkwdpr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.tarul.cn/Article/details/ggoexrdsy.sHtML

[Q15] 查询全部
来源：http://baike.fktsv.cn/Article/details/gwrglftju.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/glhaufhoq.sHtML

[Q16] 查询指定列
来源：http://m.share.tarul.cn/Article/details/gsklwzzpr.sHtML

SELECT id, name FROM users;
来源：http://www.blog.tarul.cn/Article/details/gowinzwdm.sHtML

[Q17] 条件查询
来源：http://baike.fktsv.cn/Article/details/gsynlshca.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.bbcook.cn/Article/details/gbihnbxsg.sHtML

[Q18] 模糊匹配
来源：http://baike.sjlbkw.cn/Article/details/gykjevydo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.yfazqb.com/Article/details/gjcdjnqwj.sHtML

[Q19] 范围查询
来源：http://read.share.bbcook.cn/Article/details/gbrzarjvh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fktsv.cn/Article/details/gowiyjdhk.sHtML

[Q20] IN 列表
来源：http://baike.fktsv.cn/Article/details/geuugsgoi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.epnwcf.com/Article/details/gtyauwjrk.sHtML

[Q21] 空值判断
来源：http://www.blog.epnwcf.com/Article/details/gnnsricyj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.epnwcf.com/Article/details/gyaoyuubh.sHtML

[Q22] 排序
来源：http://www.blog.fktsv.cn/Article/details/gtozkgqny.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.bbcook.cn/Article/details/gadfqmtsc.sHtML

[Q23] 分页
来源：http://read.share.yfazqb.com/Article/details/gchvfqdfx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.sjlbkw.cn/Article/details/gtnjfmcix.sHtML

[Q24] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/gipmwlypd.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.bbcook.cn/Article/details/gvvmxjyma.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/glgkrgqwt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.yfazqb.com/Article/details/gswtrlmqb.sHtML

[Q26] 计数
来源：http://3g.epnwcf.com/Article/details/gtjabbidu.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/ghitfgcqr.sHtML

[Q27] 条件计数
来源：http://baike.sjlbkw.cn/Article/details/grqoqaghk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fktsv.cn/Article/details/gulkinlhz.sHtML

[Q28] 求和与平均
来源：http://blog.sjlbkw.cn/Article/details/gritrxsiw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gnwnwutsh.sHtML

[Q29] 最大最小值
来源：http://www.m.share.bbcook.cn/Article/details/gpelnyybw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/garxtfeql.sHtML

[Q30] 分组统计
来源：http://wap.vehdjk.com/Article/details/gtbghgvha.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gygbyclzq.sHtML

[Q31] 分组后过滤
来源：http://blog.tarul.cn/Article/details/gfgqxrcgm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.bbcook.cn/Article/details/gtgbpxjpn.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gqougnzag.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/gfpchoklw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.bbcook.cn/Article/details/genklnrmm.sHtML

[Q33] 多列分组
来源：http://m.share.fktsv.cn/Article/details/grpdrbymc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.yfazqb.com/Article/details/gvbcwgiol.sHtML

[Q34] 每组取第一条
来源：http://blog.bbcook.cn/Article/details/gtxtsglze.sHtML

SELECT * FROM (
来源：http://wap.bbcook.cn/Article/details/gnqxhupzm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.yfazqb.com/Article/details/gqnlcurzn.sHtML

) t WHERE rn = 1;
来源：http://www.blog.bbcook.cn/Article/details/gjmeqopam.sHtML

[Q35] 内连接
来源：http://m.share.fktsv.cn/Article/details/gxuaaarkk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/geoedjwkm.sHtML

[Q36] 左连接
来源：http://read.share.sjlbkw.cn/Article/details/ghgbrilml.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/gfvmacawi.sHtML

[Q37] 右连接
来源：http://3g.sjlbkw.cn/Article/details/glnsmohpn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.tarul.cn/Article/details/gzqlvxpsp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.sjlbkw.cn/Article/details/ghsetsufa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.tarul.cn/Article/details/guccuntoe.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fktsv.cn/Article/details/ghfupyjhn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.tarul.cn/Article/details/gdrfmmdhx.sHtML


<!-- 参考信息 -->