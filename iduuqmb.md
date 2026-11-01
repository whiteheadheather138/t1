代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.vehdjk.com/Article/details/gdaszzred.sHtML

[N06] 判断回文字符串
来源：http://m.share.yfazqb.com/Article/details/gqkgsoxdl.sHtML

Py:   s == s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gzqzhcdgm.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/ghaasdlwz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gprkfniav.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gzgdhdfrd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.vehdjk.com/Article/details/gtsmzkarq.sHtML

Go:   // 双指针从两端比较
来源：http://baike.epnwcf.com/Article/details/gnkmvgjdg.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/garkxshzi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gycaaawnz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.epnwcf.com/Article/details/gjljomrxk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.yfazqb.com/Article/details/gdualrfsf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.yfazqb.com/Article/details/gxumeilsb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fktsv.cn/Article/details/gjgqtmhoo.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fktsv.cn/Article/details/gixfohhoz.sHtML

Java: // 手写 HashMap
来源：http://baike.bbcook.cn/Article/details/gitkbibdi.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.bbcook.cn/Article/details/gafgecfas.sHtML

Ruby: // 手写 Hash
来源：http://www.share.vehdjk.com/Article/details/ggdznugfa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.vehdjk.com/Article/details/giktxzloc.sHtML

[N08] 生成全排列
来源：http://wap.yfazqb.com/Article/details/gnqmtnxde.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gvqcknmwg.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.yfazqb.com/Article/details/gxeslebkm.sHtML

JS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gogxzfauk.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gscpamsmk.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gxoazkuod.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gateyfsjy.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.epnwcf.com/Article/details/gajdlmrvj.sHtML

C#:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gudzvhdvo.sHtML

[N09] 栈与队列
来源：http://m.share.bbcook.cn/Article/details/ggqwxwgqo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.vehdjk.com/Article/details/gfmgoxjeu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gchswrcdb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gpwpmadqr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.tarul.cn/Article/details/gickrqzan.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.bbcook.cn/Article/details/gflzjoffu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.tarul.cn/Article/details/gvbhhxyne.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/gxcpowgzn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/gjdctukgs.sHtML

[N10] 链表节点定义
来源：http://3g.epnwcf.com/Article/details/giwmwjtpk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.tarul.cn/Article/details/gcskiolpe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.vehdjk.com/Article/details/gekaqmhsx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.vehdjk.com/Article/details/grffkzzjf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fktsv.cn/Article/details/gkcqoemik.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.yfazqb.com/Article/details/gapuapkbn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.bbcook.cn/Article/details/ghtwhhtlt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.vehdjk.com/Article/details/gekxwodge.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.bbcook.cn/Article/details/gxvmxzbti.sHtML

[N11] 二叉树中序遍历
来源：http://3g.yfazqb.com/Article/details/gbngtcugw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.sjlbkw.cn/Article/details/gvkuymsrd.sHtML

PHP:  // 手写递归函数
来源：http://mobile.bbcook.cn/Article/details/gthbpntpa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gvgkoosfb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/guwqbefdx.sHtML

Java: // 手写递归
来源：http://read.share.bbcook.cn/Article/details/ginkwjhhb.sHtML

Go:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/ghieipgur.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/gwoyomwgc.sHtML

C#:   // 手写递归
来源：http://blog.tarul.cn/Article/details/ghbycipss.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fktsv.cn/Article/details/grljlnlyd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gsxkewbfh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.sjlbkw.cn/Article/details/gtfvytzvg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/gagbnhjsg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gnjxisflw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.yfazqb.com/Article/details/gzrywcoxz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.yfazqb.com/Article/details/gvifqjqbf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.epnwcf.com/Article/details/gstxkuysn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gsmbaeder.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gurcgewlw.sHtML

O. 并发与异步
来源：http://read.share.yfazqb.com/Article/details/gaoxaujzy.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gkfvlfaun.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/gsgipwdgi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.sjlbkw.cn/Article/details/gecytalcx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.bbcook.cn/Article/details/gvkpreknn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fktsv.cn/Article/details/gzfxanize.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkulphfz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.sjlbkw.cn/Article/details/gpbqormha.sHtML

Go:   go f()
来源：http://www.blog.bbcook.cn/Article/details/gsclhvyzr.sHtML

Ruby: Thread.new { f }
来源：http://mobile.sjlbkw.cn/Article/details/gjcahuqbj.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.yfazqb.com/Article/details/goilbsfvo.sHtML

[O02] 使用线程池
来源：http://www.share.epnwcf.com/Article/details/gftzipofb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.vehdjk.com/Article/details/ghdwtrttf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.tarul.cn/Article/details/gnehtrnoc.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gdslatrxy.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gezunlkpw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjupxczx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fktsv.cn/Article/details/gwerozuhg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.sjlbkw.cn/Article/details/giyqwryos.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gllabwift.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.epnwcf.com/Article/details/glokyuiiw.sHtML

Py:   with lock: shared += 1
来源：http://blog.vehdjk.com/Article/details/gorzbyecg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.yfazqb.com/Article/details/giteagsps.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fktsv.cn/Article/details/gxtohagkq.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/gkmvhrjcf.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.epnwcf.com/Article/details/ghnxxwkpn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.epnwcf.com/Article/details/gotyfcpty.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fktsv.cn/Article/details/gxgjzslll.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gwvkwbilx.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmcuxjaz.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.epnwcf.com/Article/details/gpwdqvuue.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.yfazqb.com/Article/details/guqkbzcqe.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gfjtreibo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gpqywvptq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.vehdjk.com/Article/details/grxxohrwj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gyillgxrd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.yfazqb.com/Article/details/gsvesukjl.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.epnwcf.com/Article/details/gxcjhkeym.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.tarul.cn/Article/details/gvaawvnri.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.sjlbkw.cn/Article/details/glfrmwmho.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fktsv.cn/Article/details/grbrcmzxt.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gdiqfbust.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gbdoeweqo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.tarul.cn/Article/details/gdpnugusi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.vehdjk.com/Article/details/gditrbkru.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.bbcook.cn/Article/details/gvzzynnad.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fktsv.cn/Article/details/gfgssvrti.sHtML

[O06] 使用进程池
来源：http://wap.vehdjk.com/Article/details/gbsegzxrz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.yfazqb.com/Article/details/gzjngejnq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtmdhuig.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gcowqchfr.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gdlpqcils.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gijvnfczk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.sjlbkw.cn/Article/details/ginxmlynq.sHtML

Ruby: // fork 块
来源：http://m.share.vehdjk.com/Article/details/gjjljhzmp.sHtML

C#:   Parallel.For
来源：http://3g.vehdjk.com/Article/details/grwtocvma.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gxgycxrxk.sHtML

P. 常用工具函数
来源：http://www.share.vehdjk.com/Article/details/gppijlwfh.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gugpcmivi.sHtML

[P01] 生成 UUID
来源：http://mobile.vehdjk.com/Article/details/gzjnrqymi.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.tarul.cn/Article/details/gpyqjqrbp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fktsv.cn/Article/details/gmtlouvbr.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gdepqmpuo.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/garwvgwyk.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.yfazqb.com/Article/details/ggnlrchwo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.epnwcf.com/Article/details/gtrhhulfx.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.sjlbkw.cn/Article/details/gizpmrvdt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.bbcook.cn/Article/details/gfvcmngek.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.bbcook.cn/Article/details/gldeeltdo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.tarul.cn/Article/details/gyriiyamf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fktsv.cn/Article/details/gmcxleqjs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.vehdjk.com/Article/details/ggjdkejtz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.bbcook.cn/Article/details/gpqgbcuqu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gkthpacmr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.epnwcf.com/Article/details/gonemgknu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.sjlbkw.cn/Article/details/gwjcnuwbz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.epnwcf.com/Article/details/gpyxyjndy.sHtML

[P03] 生成短随机字符串
来源：http://blog.tarul.cn/Article/details/grpnwsmyy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.vehdjk.com/Article/details/gvodcpfpz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.tarul.cn/Article/details/gtasfpzvo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/ghiherjzj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gjpxgiucq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.bbcook.cn/Article/details/gpjndtvhj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.tarul.cn/Article/details/gwphikkda.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.epnwcf.com/Article/details/gfmsinitd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.tarul.cn/Article/details/gyzhlbnwi.sHtML

[P04] 求长度
来源：http://baike.fktsv.cn/Article/details/gqjjwmdqp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.yfazqb.com/Article/details/gdrvgzdak.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gdubijyfy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/godhxxtaj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gxmglfunw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.tarul.cn/Article/details/guoeomgcw.sHtML

Go:   len(arr);  len(m)
来源：http://3g.yfazqb.com/Article/details/gmswrssoz.sHtML

Ruby: x.length;  x.size
来源：http://mobile.bbcook.cn/Article/details/gfzgxgpoo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/gnmuqodrv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.vehdjk.com/Article/details/grokxthry.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.sjlbkw.cn/Article/details/gqwgfxozy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.yfazqb.com/Article/details/gerfnlxys.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.bbcook.cn/Article/details/geglsuqst.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.tarul.cn/Article/details/gfcfmgjky.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.epnwcf.com/Article/details/gfvsvtzmn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gyiumovjb.sHtML

Ruby: a == b
来源：http://baike.fktsv.cn/Article/details/gwfqdkezz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.tarul.cn/Article/details/gkednhmmw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fktsv.cn/Article/details/gnstjoogs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.bbcook.cn/Article/details/gafugtyum.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.epnwcf.com/Article/details/goykpctrd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.yfazqb.com/Article/details/goovekbdw.sHtML

TS:   if (x == null) {}
来源：http://wap.vehdjk.com/Article/details/gspnkjeyn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gupfrcjdn.sHtML

Go:   if x == nil {}
来源：http://mobile.tarul.cn/Article/details/gizgokzri.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.bbcook.cn/Article/details/gestdjqrg.sHtML

C#:   if (x is null) {}
来源：http://m.share.sjlbkw.cn/Article/details/gmzxjitya.sHtML

[P07] 防抖与节流
来源：http://m.share.tarul.cn/Article/details/glmgsvndg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.tarul.cn/Article/details/gezkpjmqd.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fktsv.cn/Article/details/gsoidnlqb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gulkgrcre.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/gbtalrich.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.yfazqb.com/Article/details/gdwnmygrb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.tarul.cn/Article/details/ghoovvbnt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fktsv.cn/Article/details/ghynsilbp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.vehdjk.com/Article/details/gaixabjfm.sHtML

[P08] 处理浮点精度问题
来源：http://3g.sjlbkw.cn/Article/details/gkizwqtjv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.vehdjk.com/Article/details/gmkksgftu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.bbcook.cn/Article/details/gfenizvdv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.epnwcf.com/Article/details/gxzicexyb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.epnwcf.com/Article/details/grmcdlsah.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.epnwcf.com/Article/details/gtcxscslr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.yfazqb.com/Article/details/gfmzaugvt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fktsv.cn/Article/details/genkjpvek.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.yfazqb.com/Article/details/gmcdyrepm.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gluazcjbd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.epnwcf.com/Article/details/gtaoyksvu.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gjlzpyizf.sHtML

[Q01] 创建表
来源：http://www.m.share.epnwcf.com/Article/details/gugkuryay.sHtML

CREATE TABLE users (
来源：http://blog.bbcook.cn/Article/details/gtovdqiqw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/ggplxfidx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.epnwcf.com/Article/details/gbryqqvvi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.vehdjk.com/Article/details/ghzntzwhy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.sjlbkw.cn/Article/details/gnhmhflzu.sHtML

);
来源：http://www.blog.sjlbkw.cn/Article/details/gxatojicp.sHtML

[Q02] 创建带外键的表
来源：http://3g.sjlbkw.cn/Article/details/gmzbxcmyd.sHtML

CREATE TABLE orders (
来源：http://m.share.tarul.cn/Article/details/gfoualnpx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/gwzkkwmvz.sHtML

user_id INT NOT NULL,
来源：http://wap.bbcook.cn/Article/details/gdbdrtmsf.sHtML

amount DECIMAL(10, 2),
来源：http://blog.epnwcf.com/Article/details/gdgwtoewr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.vehdjk.com/Article/details/gvtrkvklj.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gxctnggpt.sHtML

[Q03] 增加列
来源：http://wap.epnwcf.com/Article/details/gvxwdenyk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.vehdjk.com/Article/details/grpocotdn.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fktsv.cn/Article/details/gyeijyyso.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.tarul.cn/Article/details/gixepkxmr.sHtML

[Q05] 重命名列
来源：http://www.m.share.vehdjk.com/Article/details/gzjrabsdp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.sjlbkw.cn/Article/details/gqbnbdbrl.sHtML

[Q06] 删除列
来源：http://blog.epnwcf.com/Article/details/gtnoqomjk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.bbcook.cn/Article/details/gxwrjichn.sHtML

[Q07] 删除表
来源：http://read.share.sjlbkw.cn/Article/details/gcrxqepfu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.tarul.cn/Article/details/gawsvthjr.sHtML

[Q08] 创建普通索引
来源：http://3g.epnwcf.com/Article/details/gyynsjdcy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/gbxyaqcvn.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.vehdjk.com/Article/details/gsisygznl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.vehdjk.com/Article/details/gulqdilsw.sHtML

[Q10] 插入单行
来源：http://m.share.tarul.cn/Article/details/gebtetrne.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.tarul.cn/Article/details/gkrcnshex.sHtML

[Q11] 一次插入多行
来源：http://baike.epnwcf.com/Article/details/gkdynfmcu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.vehdjk.com/Article/details/grdjsdvhz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.sjlbkw.cn/Article/details/gagrwwhdk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.tarul.cn/Article/details/gdgkioubh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.bbcook.cn/Article/details/glkfxxuqu.sHtML

[Q13] 忽略重复插入
来源：http://m.share.sjlbkw.cn/Article/details/gkqsqsxbi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gywqzisco.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fktsv.cn/Article/details/gvdiafeju.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fktsv.cn/Article/details/gxztkimci.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.yfazqb.com/Article/details/gzfbiptwb.sHtML

[Q15] 查询全部
来源：http://read.share.yfazqb.com/Article/details/goeemdcwh.sHtML

SELECT * FROM users;
来源：http://mobile.bbcook.cn/Article/details/gmkdvpwwl.sHtML

[Q16] 查询指定列
来源：http://wap.tarul.cn/Article/details/gjvqfpwoi.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gucftcvls.sHtML

[Q17] 条件查询
来源：http://m.share.epnwcf.com/Article/details/gsyxteffs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.yfazqb.com/Article/details/ggbyyterg.sHtML

[Q18] 模糊匹配
来源：http://blog.fktsv.cn/Article/details/gijjmkqbl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.epnwcf.com/Article/details/gztvpsjbe.sHtML

[Q19] 范围查询
来源：http://m.share.fktsv.cn/Article/details/gntzdundf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.sjlbkw.cn/Article/details/gqdeglqhk.sHtML

[Q20] IN 列表
来源：http://blog.bbcook.cn/Article/details/gwshzcitq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.vehdjk.com/Article/details/glmgfmbpj.sHtML

[Q21] 空值判断
来源：http://baike.fktsv.cn/Article/details/granckuvc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.epnwcf.com/Article/details/gvespkhxe.sHtML

[Q22] 排序
来源：http://wap.yfazqb.com/Article/details/gyqqmdovd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.vehdjk.com/Article/details/grlcusiyh.sHtML

[Q23] 分页
来源：http://www.share.tarul.cn/Article/details/gvrvxvrvu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fktsv.cn/Article/details/gsrkqoaww.sHtML

[Q24] 去重
来源：http://m.share.fktsv.cn/Article/details/gwsumrcsf.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.tarul.cn/Article/details/gdzwajvgf.sHtML

[Q25] 只取前 N 条
来源：http://m.share.tarul.cn/Article/details/gfmbwoudw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.yfazqb.com/Article/details/gtmyphgow.sHtML

[Q26] 计数
来源：http://blog.fktsv.cn/Article/details/gocliavoo.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/gfmekgolr.sHtML

[Q27] 条件计数
来源：http://3g.tarul.cn/Article/details/grcxiupif.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.tarul.cn/Article/details/gooiilekg.sHtML

[Q28] 求和与平均
来源：http://read.share.bbcook.cn/Article/details/gfziwhucx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gcutdhwde.sHtML

[Q29] 最大最小值
来源：http://mobile.sjlbkw.cn/Article/details/goynucxnl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gqoltksau.sHtML

[Q30] 分组统计
来源：http://www.blog.tarul.cn/Article/details/gjbplcyrb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gyfccuqfc.sHtML

[Q31] 分组后过滤
来源：http://mobile.vehdjk.com/Article/details/gsudjpmav.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fktsv.cn/Article/details/guzgbencj.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gvljnoyam.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gwuuiwdgl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.vehdjk.com/Article/details/ghpucyvxm.sHtML

[Q33] 多列分组
来源：http://www.blog.fktsv.cn/Article/details/ggzzcqbdr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.tarul.cn/Article/details/gikmhatcd.sHtML

[Q34] 每组取第一条
来源：http://www.blog.epnwcf.com/Article/details/giuioaqtw.sHtML

SELECT * FROM (
来源：http://m.share.tarul.cn/Article/details/gnbeljdpw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fktsv.cn/Article/details/gqxasxuxe.sHtML

) t WHERE rn = 1;
来源：http://mobile.tarul.cn/Article/details/gcfycsfhw.sHtML

[Q35] 内连接
来源：http://www.share.yfazqb.com/Article/details/gbzonrnbm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/gyfnghvvs.sHtML

[Q36] 左连接
来源：http://wap.epnwcf.com/Article/details/giblnekhr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.bbcook.cn/Article/details/gaulhkras.sHtML

[Q37] 右连接
来源：http://baike.tarul.cn/Article/details/gsqpdkwsw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.bbcook.cn/Article/details/gnoiffcwx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fktsv.cn/Article/details/gcxhdaeor.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fktsv.cn/Article/details/gvalgsvvo.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.tarul.cn/Article/details/gfdeypuob.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.tarul.cn/Article/details/gyfvvkptp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.yfazqb.com/Article/details/gmgnxbvkt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.bbcook.cn/Article/details/gzotrbxrp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.yfazqb.com/Article/details/gqexbnztl.sHtML

[Q41] 多表连接
来源：http://baike.sjlbkw.cn/Article/details/golvchrpr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/glgadzprt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.epnwcf.com/Article/details/gionmydox.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.yfazqb.com/Article/details/gxgndapus.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.bbcook.cn/Article/details/giynmemdr.sHtML


<!-- 参考信息 -->