代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.yfazqb.com/Article/details/gmsyubqlk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.vehdjk.com/Article/details/gaxmkoqhj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpmfdzig.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gkwuoufyg.sHtML

[N05] 最大公约数
来源：http://baike.vehdjk.com/Article/details/gfspndemu.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/gskkftvqr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gwsitpwvi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/guicttrjx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/gcxghoxjk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/geepdyyis.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.epnwcf.com/Article/details/gjqjvhdkp.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.yfazqb.com/Article/details/ghsoqcjdf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fktsv.cn/Article/details/gnbkojhml.sHtML

[N06] 判断回文字符串
来源：http://read.share.bbcook.cn/Article/details/gqgfdrdnw.sHtML

Py:   s == s[::-1]
来源：http://blog.vehdjk.com/Article/details/goqxqynef.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gggbliiet.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gxaauiamh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/ghohuidcm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.vehdjk.com/Article/details/gcsrqghnf.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.vehdjk.com/Article/details/giowfkiuh.sHtML

Ruby: s == s.reverse
来源：http://mobile.vehdjk.com/Article/details/glapfdyqg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gjkistwsb.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.yfazqb.com/Article/details/geasubpcy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gnweszlhc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.sjlbkw.cn/Article/details/goegbvggo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fktsv.cn/Article/details/gykrewijc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.epnwcf.com/Article/details/gclyajlkc.sHtML

Java: // 手写 HashMap
来源：http://m.share.epnwcf.com/Article/details/gxrdzopmw.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.epnwcf.com/Article/details/gxrvcrsha.sHtML

Ruby: // 手写 Hash
来源：http://www.share.bbcook.cn/Article/details/gbgsafyaw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.vehdjk.com/Article/details/gtoxpalku.sHtML

[N08] 生成全排列
来源：http://wap.epnwcf.com/Article/details/gzlneczwb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.bbcook.cn/Article/details/gwnfvhjyq.sHtML

PHP:  // 手写递归交换
来源：http://blog.vehdjk.com/Article/details/gnqljtojy.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/ggptkiuji.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gzadmowbx.sHtML

Java: // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gisjadiaa.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gvtytovoz.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gmkcqddnw.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gaefivjpl.sHtML

[N09] 栈与队列
来源：http://3g.epnwcf.com/Article/details/gxjmkvanm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fktsv.cn/Article/details/gbfrbddzh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gtqhofcvy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/gyfjblqpo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fktsv.cn/Article/details/glprhyzgh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.sjlbkw.cn/Article/details/gwvbpbgza.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.vehdjk.com/Article/details/gkyklpiod.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.epnwcf.com/Article/details/gzwopfwqk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/gqcsujxry.sHtML

[N10] 链表节点定义
来源：http://baike.epnwcf.com/Article/details/ghibpkbbl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.bbcook.cn/Article/details/gbypizksk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.yfazqb.com/Article/details/gjlkhmyas.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/gzjqonaax.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.yfazqb.com/Article/details/gkqfacojt.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fktsv.cn/Article/details/gqllithmb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/glxuexsvj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.vehdjk.com/Article/details/gyqtosdxi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.yfazqb.com/Article/details/gfqnxkltc.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fktsv.cn/Article/details/gpxwrwdzp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fktsv.cn/Article/details/gzzbuvlfw.sHtML

PHP:  // 手写递归函数
来源：http://m.share.bbcook.cn/Article/details/gfydaewhb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/ghyzfelbu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gooyeslap.sHtML

Java: // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gilzunbpl.sHtML

Go:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gaxmjrali.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.tarul.cn/Article/details/gyfxakgwv.sHtML

C#:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gylqncozo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.yfazqb.com/Article/details/gxdgzmilm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.yfazqb.com/Article/details/getupinht.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.epnwcf.com/Article/details/gwbtcsgsi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gjrkdcckz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/glzjmffjy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/gdohbuvuf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.sjlbkw.cn/Article/details/ghrevposx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.epnwcf.com/Article/details/gmhmdhpqg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/gembrefnk.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnkwsstkp.sHtML

O. 并发与异步
来源：http://baike.fktsv.cn/Article/details/gtwkqmosc.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gbcyldaep.sHtML

[O01] 启动一个线程
来源：http://m.share.vehdjk.com/Article/details/gnzyddxrh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.tarul.cn/Article/details/glkmcjtxm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.sjlbkw.cn/Article/details/ghdoispxq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.yfazqb.com/Article/details/gkwbmcagc.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gqlkwlgnh.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.bbcook.cn/Article/details/gjuwgayxj.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/gpwnwukic.sHtML

Ruby: Thread.new { f }
来源：http://mobile.yfazqb.com/Article/details/gfjgnivuw.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fktsv.cn/Article/details/ghpfuzbmr.sHtML

[O02] 使用线程池
来源：http://www.share.vehdjk.com/Article/details/gsecdlkox.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.sjlbkw.cn/Article/details/gljkkcsqy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fktsv.cn/Article/details/gkvtrolox.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gvqgpazld.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/gkdvlseqj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/gwuhhfacz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.yfazqb.com/Article/details/ggtyzqsbr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.tarul.cn/Article/details/gzrjzgckt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvhfaoai.sHtML

[O03] 加锁保护共享数据
来源：http://wap.bbcook.cn/Article/details/gzulbqwus.sHtML

Py:   with lock: shared += 1
来源：http://baike.tarul.cn/Article/details/gaqiwcpqb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.sjlbkw.cn/Article/details/gqagwseur.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.bbcook.cn/Article/details/gfcaornhw.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/ganbtufww.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/gnsevbdzh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.epnwcf.com/Article/details/gxujgxznq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fktsv.cn/Article/details/gpjyucmub.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/grpdpmrcs.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.vehdjk.com/Article/details/gueqvbjmz.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.tarul.cn/Article/details/gljplgbcq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.yfazqb.com/Article/details/gmgprnxnn.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fktsv.cn/Article/details/gueyfwqxe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.tarul.cn/Article/details/ggoncjplm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.tarul.cn/Article/details/goarobqxj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.bbcook.cn/Article/details/ggsraacqm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.yfazqb.com/Article/details/gutumkjyr.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.vehdjk.com/Article/details/ggufyavvo.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.tarul.cn/Article/details/gcgczeexe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.tarul.cn/Article/details/gstcmtgzp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fktsv.cn/Article/details/gjvdyhptg.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/gumtlykbe.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gjqwiquwk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.bbcook.cn/Article/details/givamgbvf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.sjlbkw.cn/Article/details/gfdahaike.sHtML

Ruby: threads.map(&:join)
来源：http://wap.bbcook.cn/Article/details/gmrivybhh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.epnwcf.com/Article/details/gzaoynpdu.sHtML

[O06] 使用进程池
来源：http://www.share.bbcook.cn/Article/details/gqcqkdyil.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.bbcook.cn/Article/details/giklzfqxz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.vehdjk.com/Article/details/gwwfmhdde.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/geruozvoz.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/gcbimyoji.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.epnwcf.com/Article/details/gldaxshuc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.epnwcf.com/Article/details/gjcrvgnsj.sHtML

Ruby: // fork 块
来源：http://3g.sjlbkw.cn/Article/details/ghwsafknr.sHtML

C#:   Parallel.For
来源：http://3g.epnwcf.com/Article/details/gjiurkdoc.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gekyxjbws.sHtML

P. 常用工具函数
来源：http://www.m.share.tarul.cn/Article/details/gsuhpptdc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gsmljgbso.sHtML

[P01] 生成 UUID
来源：http://wap.tarul.cn/Article/details/gmevvhgxs.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.epnwcf.com/Article/details/ggirfgrpn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/gvykyazos.sHtML

JS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/ghxkmnmbb.sHtML

TS:   crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/gqyoledzm.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.yfazqb.com/Article/details/gbxghlcts.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.vehdjk.com/Article/details/gapbhfvjx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fktsv.cn/Article/details/gnivcowld.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.epnwcf.com/Article/details/gsgrbgkam.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.vehdjk.com/Article/details/gpqtxultr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fktsv.cn/Article/details/gowpsumvc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.tarul.cn/Article/details/gmaxpalts.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.vehdjk.com/Article/details/grdopxjku.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.tarul.cn/Article/details/gxmrzrqqx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/geapbrpfa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.vehdjk.com/Article/details/gpofbecag.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.epnwcf.com/Article/details/guynvatun.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/gfenmqbfr.sHtML

[P03] 生成短随机字符串
来源：http://www.share.vehdjk.com/Article/details/gkwmigcfd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.bbcook.cn/Article/details/gmgabxcaq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.yfazqb.com/Article/details/gbzoejawr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/gefqivvii.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/glgkkusub.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.tarul.cn/Article/details/gikxdmgbp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.yfazqb.com/Article/details/gxepxbchy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.epnwcf.com/Article/details/ghwmqvqyd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.bbcook.cn/Article/details/ggkbonujw.sHtML

[P04] 求长度
来源：http://www.m.share.tarul.cn/Article/details/gqjbbkoiv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.tarul.cn/Article/details/gzvmxmsqm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gldnrafbe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gmtilidjn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.yfazqb.com/Article/details/gyygnyotl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.epnwcf.com/Article/details/gymtetavm.sHtML

Go:   len(arr);  len(m)
来源：http://3g.sjlbkw.cn/Article/details/gqdbaeoco.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.bbcook.cn/Article/details/gbdwareia.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/ggldpvdqz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.sjlbkw.cn/Article/details/gszvnyxbs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.yfazqb.com/Article/details/gdvuhhhtd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.sjlbkw.cn/Article/details/gtulrbaow.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.sjlbkw.cn/Article/details/gxdkgwrmz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/ghpygyoxu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.bbcook.cn/Article/details/gdecoooic.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gzgltqdpz.sHtML

Ruby: a == b
来源：http://wap.tarul.cn/Article/details/gppvrfczn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fktsv.cn/Article/details/giofzzhcx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fktsv.cn/Article/details/ggrehogdz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.sjlbkw.cn/Article/details/gobgmhcig.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.tarul.cn/Article/details/gihswucvf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.tarul.cn/Article/details/grrvuvaoo.sHtML

TS:   if (x == null) {}
来源：http://mobile.epnwcf.com/Article/details/gnjsabvmn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gitfimwag.sHtML

Go:   if x == nil {}
来源：http://blog.tarul.cn/Article/details/gayruwcfy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.sjlbkw.cn/Article/details/gibhwlfsz.sHtML

C#:   if (x is null) {}
来源：http://mobile.vehdjk.com/Article/details/gwtfafify.sHtML

[P07] 防抖与节流
来源：http://blog.fktsv.cn/Article/details/glsykntcs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.bbcook.cn/Article/details/grjeoweio.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.sjlbkw.cn/Article/details/gesgmvwck.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gdtztnpqu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gmikreuys.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.bbcook.cn/Article/details/gbuqkkdfg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.bbcook.cn/Article/details/gvncqsthr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.yfazqb.com/Article/details/gitmnfbaf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.bbcook.cn/Article/details/gigcitgwo.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fktsv.cn/Article/details/guxhayfou.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.epnwcf.com/Article/details/gebbqwbit.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.yfazqb.com/Article/details/gqlgiyidq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.yfazqb.com/Article/details/gltkaywja.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/giqveepop.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.vehdjk.com/Article/details/goaqpdtnh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fktsv.cn/Article/details/gugnrqequ.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.vehdjk.com/Article/details/gofowdfwa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.tarul.cn/Article/details/govtlalns.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gezilwlmo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.tarul.cn/Article/details/gjflpffck.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grvgdfvhp.sHtML

[Q01] 创建表
来源：http://mobile.fktsv.cn/Article/details/gcqietptd.sHtML

CREATE TABLE users (
来源：http://read.share.bbcook.cn/Article/details/gcltryawl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/glizgjcfb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.tarul.cn/Article/details/gphropsiu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.sjlbkw.cn/Article/details/gpzzcguls.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.yfazqb.com/Article/details/gcayyvxjd.sHtML

);
来源：http://baike.tarul.cn/Article/details/gzdcrnlog.sHtML

[Q02] 创建带外键的表
来源：http://www.share.vehdjk.com/Article/details/geiogrdfg.sHtML

CREATE TABLE orders (
来源：http://3g.tarul.cn/Article/details/gnnhxylkb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/gcwiftklg.sHtML

user_id INT NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/geolbdmuo.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.yfazqb.com/Article/details/gpavlbdrd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.tarul.cn/Article/details/guoedesqf.sHtML

);
来源：http://www.blog.epnwcf.com/Article/details/gdelmuzhu.sHtML

[Q03] 增加列
来源：http://3g.fktsv.cn/Article/details/gkjdqnuqg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.epnwcf.com/Article/details/gaptdwovn.sHtML

[Q04] 修改列类型
来源：http://blog.yfazqb.com/Article/details/gjzoifyzf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fktsv.cn/Article/details/gfbbknipb.sHtML

[Q05] 重命名列
来源：http://blog.tarul.cn/Article/details/gqafnphxg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.vehdjk.com/Article/details/gvmlthyiu.sHtML

[Q06] 删除列
来源：http://blog.vehdjk.com/Article/details/gagolevjc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.tarul.cn/Article/details/gmgfaxekw.sHtML

[Q07] 删除表
来源：http://mobile.bbcook.cn/Article/details/gjfpwnlws.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.yfazqb.com/Article/details/gceoteika.sHtML

[Q08] 创建普通索引
来源：http://m.share.yfazqb.com/Article/details/gyzarqbra.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/gyfszslje.sHtML

[Q09] 创建唯一索引
来源：http://3g.sjlbkw.cn/Article/details/gafuuzeea.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gbcnfktsy.sHtML

[Q10] 插入单行
来源：http://m.share.epnwcf.com/Article/details/gnzkfiecv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.sjlbkw.cn/Article/details/gdirgkliu.sHtML

[Q11] 一次插入多行
来源：http://m.share.sjlbkw.cn/Article/details/gkjdbloss.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/grlbnnjcq.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.epnwcf.com/Article/details/ganxjamha.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.yfazqb.com/Article/details/gicwotzmf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.vehdjk.com/Article/details/gazphbkbk.sHtML

[Q13] 忽略重复插入
来源：http://wap.epnwcf.com/Article/details/groaogjyo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gxkhyelhc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.bbcook.cn/Article/details/gujbjhhwd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.yfazqb.com/Article/details/grlskrsbu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fktsv.cn/Article/details/gfnikcaaf.sHtML

[Q15] 查询全部
来源：http://3g.yfazqb.com/Article/details/gfxneguzk.sHtML

SELECT * FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/grjrthugd.sHtML

[Q16] 查询指定列
来源：http://www.blog.epnwcf.com/Article/details/gofpvsqdt.sHtML

SELECT id, name FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gcqmyijvc.sHtML

[Q17] 条件查询
来源：http://read.share.tarul.cn/Article/details/gxnuohzas.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.tarul.cn/Article/details/gnkukeyle.sHtML

[Q18] 模糊匹配
来源：http://wap.vehdjk.com/Article/details/gjuedprkd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.yfazqb.com/Article/details/goddphrpn.sHtML

[Q19] 范围查询
来源：http://blog.bbcook.cn/Article/details/gjwhyxqdn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.tarul.cn/Article/details/gswpamarf.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/ghthjpwpy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.vehdjk.com/Article/details/giydqtyup.sHtML

[Q21] 空值判断
来源：http://wap.yfazqb.com/Article/details/gnlnbowcn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fktsv.cn/Article/details/gjpblkzvk.sHtML

[Q22] 排序
来源：http://wap.vehdjk.com/Article/details/gvqkfadej.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.sjlbkw.cn/Article/details/gqezhpilm.sHtML

[Q23] 分页
来源：http://baike.sjlbkw.cn/Article/details/grcqwcpef.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.vehdjk.com/Article/details/geredrndb.sHtML

[Q24] 去重
来源：http://read.share.tarul.cn/Article/details/grfitjhoi.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.yfazqb.com/Article/details/gmxzggzio.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fktsv.cn/Article/details/ghsdivaty.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.tarul.cn/Article/details/gwsieqqsk.sHtML

[Q26] 计数
来源：http://read.share.yfazqb.com/Article/details/goxckffwi.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fktsv.cn/Article/details/gfauumtwe.sHtML

[Q27] 条件计数
来源：http://mobile.vehdjk.com/Article/details/ghqgmcehw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.yfazqb.com/Article/details/gikqxddoi.sHtML

[Q28] 求和与平均
来源：http://blog.vehdjk.com/Article/details/gtwrhqixr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gzpozupho.sHtML

[Q29] 最大最小值
来源：http://www.share.vehdjk.com/Article/details/glfkyshzg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gstjsnjib.sHtML

[Q30] 分组统计
来源：http://read.share.epnwcf.com/Article/details/geefgcups.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gtalprorv.sHtML

[Q31] 分组后过滤
来源：http://wap.tarul.cn/Article/details/gqimapwbd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fktsv.cn/Article/details/gyubwpkya.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gfegzvfsh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gofnlgzyg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.sjlbkw.cn/Article/details/groqposif.sHtML

[Q33] 多列分组
来源：http://mobile.vehdjk.com/Article/details/guzqzbifv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.vehdjk.com/Article/details/gcbnvaelp.sHtML

[Q34] 每组取第一条
来源：http://read.share.vehdjk.com/Article/details/gfuujqouw.sHtML

SELECT * FROM (
来源：http://3g.bbcook.cn/Article/details/glyvyzdrl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.epnwcf.com/Article/details/grfhedqql.sHtML

) t WHERE rn = 1;
来源：http://read.share.fktsv.cn/Article/details/gslqygdqb.sHtML

[Q35] 内连接
来源：http://www.share.epnwcf.com/Article/details/gwcgasevf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gnodfucbp.sHtML

[Q36] 左连接
来源：http://3g.tarul.cn/Article/details/geclicspq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.tarul.cn/Article/details/goqjyyraj.sHtML

[Q37] 右连接
来源：http://mobile.vehdjk.com/Article/details/gysqsdzln.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.yfazqb.com/Article/details/gmxmbhjjj.sHtML


<!-- 参考信息 -->