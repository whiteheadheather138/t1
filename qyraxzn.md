代发 wailian999

[N05] 最大公约数
来源：http://baike.epnwcf.com/Article/details/gkdunolgh.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.vehdjk.com/Article/details/gqllmmesk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gvtbebhtp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/gqsnemmbd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/guykmopxz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.yfazqb.com/Article/details/gbwdctbyz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.yfazqb.com/Article/details/gkeqkmhhj.sHtML

Ruby: a.gcd(b)
来源：http://read.share.yfazqb.com/Article/details/ghrzyanfn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.sjlbkw.cn/Article/details/gfjrjrezh.sHtML

[N06] 判断回文字符串
来源：http://m.share.fktsv.cn/Article/details/gwyyydhof.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gmlshxtcr.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gjyqnsbam.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gtxdfteyc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gvxsxkrbd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.tarul.cn/Article/details/ggrxocpxd.sHtML

Go:   // 双指针从两端比较
来源：http://3g.yfazqb.com/Article/details/gqyqojkth.sHtML

Ruby: s == s.reverse
来源：http://m.share.fktsv.cn/Article/details/grgmlbsxc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/guwhdybtm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.bbcook.cn/Article/details/gpqjhpktu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.yfazqb.com/Article/details/gdkpvdvya.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.tarul.cn/Article/details/gkoxkyeer.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.yfazqb.com/Article/details/gyvwzrefm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fktsv.cn/Article/details/gjskatxht.sHtML

Java: // 手写 HashMap
来源：http://www.blog.tarul.cn/Article/details/gjwtatqjd.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.bbcook.cn/Article/details/glarchngx.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fktsv.cn/Article/details/gigrpdbvw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.yfazqb.com/Article/details/gglbfocuf.sHtML

[N08] 生成全排列
来源：http://mobile.sjlbkw.cn/Article/details/gbsobgrdf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.bbcook.cn/Article/details/gvylsmfpm.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.vehdjk.com/Article/details/gskkbjnjj.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gvnxomsen.sHtML

TS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/geoegyhyp.sHtML

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gcwsghoiv.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gjfehmrxn.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.bbcook.cn/Article/details/gozfxndbl.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gihzeluiw.sHtML

[N09] 栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gzchqvuwd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.sjlbkw.cn/Article/details/glxymyegc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.vehdjk.com/Article/details/gyipncuyn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gddefcepc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.vehdjk.com/Article/details/gogzzdojj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.yfazqb.com/Article/details/gurmxsrnk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.vehdjk.com/Article/details/gnvmapmdp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gjqbjozxh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.vehdjk.com/Article/details/gvuohyqzf.sHtML

[N10] 链表节点定义
来源：http://m.share.yfazqb.com/Article/details/ggrofvptl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.yfazqb.com/Article/details/gjgojjxhf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.epnwcf.com/Article/details/gbrglvpqw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.vehdjk.com/Article/details/gxedbvcvr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/gxntqgksd.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.yfazqb.com/Article/details/glkuaixih.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fktsv.cn/Article/details/gutlxoysc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.vehdjk.com/Article/details/gemqcymvs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghwzndikn.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.sjlbkw.cn/Article/details/gojhtalmu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.vehdjk.com/Article/details/gxonivhyj.sHtML

PHP:  // 手写递归函数
来源：http://m.share.tarul.cn/Article/details/ghuhtoydi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gydcvnbjk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gntpnbyfk.sHtML

Java: // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gbflxnvzy.sHtML

Go:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gfqjetczq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.vehdjk.com/Article/details/gbopgspcv.sHtML

C#:   // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gukvsazmq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.yfazqb.com/Article/details/gblvailxk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.tarul.cn/Article/details/gqipumira.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.epnwcf.com/Article/details/gitbvosqi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.bbcook.cn/Article/details/gqopxsubn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gzayivvqw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/ggwluvcor.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/gtxngwhcp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fktsv.cn/Article/details/glnzcrthu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/gjbszujja.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gqdhcyple.sHtML

O. 并发与异步
来源：http://www.share.bbcook.cn/Article/details/grugkehrb.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gvpygsgov.sHtML

[O01] 启动一个线程
来源：http://blog.vehdjk.com/Article/details/gkfvhrzar.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fktsv.cn/Article/details/gdxepkove.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.sjlbkw.cn/Article/details/geopiieeh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.bbcook.cn/Article/details/gujlulibq.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gfjkrymgm.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.bbcook.cn/Article/details/gmfxanlyz.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/gurcrhund.sHtML

Ruby: Thread.new { f }
来源：http://wap.epnwcf.com/Article/details/gqcrlgsuy.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.tarul.cn/Article/details/gvsydmzmt.sHtML

[O02] 使用线程池
来源：http://m.share.fktsv.cn/Article/details/gelkvjins.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.yfazqb.com/Article/details/ghiknzate.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.yfazqb.com/Article/details/gmnhvlbay.sHtML

JS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/gwkewefsy.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/ggdxeswrq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.bbcook.cn/Article/details/gbowyfpia.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.yfazqb.com/Article/details/gslabbrow.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.epnwcf.com/Article/details/gqrpfkuca.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fktsv.cn/Article/details/giztcdlwo.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fktsv.cn/Article/details/gnmcfuyrd.sHtML

Py:   with lock: shared += 1
来源：http://baike.fktsv.cn/Article/details/gumbtkaeq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.yfazqb.com/Article/details/ggmyknefd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.sjlbkw.cn/Article/details/gsmmfkanx.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/ghtsnwosk.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gfrxadqkl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fktsv.cn/Article/details/gcadtejge.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.vehdjk.com/Article/details/gznlgccdj.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gahssqwbc.sHtML

[O04] 定义异步函数并等待
来源：http://baike.vehdjk.com/Article/details/gfflqghvg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.epnwcf.com/Article/details/ggryewzsi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.tarul.cn/Article/details/ghczpqjxl.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.vehdjk.com/Article/details/gjsrbokex.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gqvofzddn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fktsv.cn/Article/details/gvzkgukdl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.epnwcf.com/Article/details/gnbwpdhjs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.yfazqb.com/Article/details/ggovleevv.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/gideosjtv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.yfazqb.com/Article/details/gbnfoprep.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.tarul.cn/Article/details/gcmvprmsc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.vehdjk.com/Article/details/gpghytgkv.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gugijxdnj.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/garcpgohh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.yfazqb.com/Article/details/gfpiykykq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.vehdjk.com/Article/details/gomuvdtjl.sHtML

Ruby: threads.map(&:join)
来源：http://3g.sjlbkw.cn/Article/details/giistxdsu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.sjlbkw.cn/Article/details/gmqxqkycj.sHtML

[O06] 使用进程池
来源：http://read.share.vehdjk.com/Article/details/gbcxiiohw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fktsv.cn/Article/details/gejsbiarf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.bbcook.cn/Article/details/gkhjqfasx.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gyumqndkj.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/gzzqmqbgw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.tarul.cn/Article/details/geqnbzaou.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.vehdjk.com/Article/details/gntbzalet.sHtML

Ruby: // fork 块
来源：http://www.share.epnwcf.com/Article/details/gyxvdogbm.sHtML

C#:   Parallel.For
来源：http://www.share.bbcook.cn/Article/details/gulmduedr.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gffhxydsq.sHtML

P. 常用工具函数
来源：http://3g.epnwcf.com/Article/details/gyfklutoc.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmlqsuvuv.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/gfotkwwwr.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.bbcook.cn/Article/details/gcfsfvgkq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gcofpyuyo.sHtML

JS:   crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gsvzwqjhs.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gclmzwaqz.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.sjlbkw.cn/Article/details/geokcmslh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.sjlbkw.cn/Article/details/gvrskectd.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.epnwcf.com/Article/details/ggumnagbz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.epnwcf.com/Article/details/gjcptpnzh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fktsv.cn/Article/details/gmuvtjemr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fktsv.cn/Article/details/ghltpqdxp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.bbcook.cn/Article/details/gafjqwykk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.yfazqb.com/Article/details/gmummzlzc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fktsv.cn/Article/details/gufofjult.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gzpzpzcjd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.epnwcf.com/Article/details/gnlvrybcj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.vehdjk.com/Article/details/gabluireh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.sjlbkw.cn/Article/details/gcchoetwr.sHtML

[P03] 生成短随机字符串
来源：http://wap.tarul.cn/Article/details/gskaitxtk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.yfazqb.com/Article/details/gxgfyccyn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.yfazqb.com/Article/details/gygehihvj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/gfplzsesu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/gutvvwaoq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.vehdjk.com/Article/details/gnyllxghm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.sjlbkw.cn/Article/details/gbnfunidg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.epnwcf.com/Article/details/gvlqpniwv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.vehdjk.com/Article/details/gayqslxxk.sHtML

[P04] 求长度
来源：http://www.share.tarul.cn/Article/details/godgrpikt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.bbcook.cn/Article/details/gysuvytjl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gdcjnkizy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gnqnrygmn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/gktnsmsqh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.bbcook.cn/Article/details/gjahlsxdn.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.vehdjk.com/Article/details/gxdriusxx.sHtML

Ruby: x.length;  x.size
来源：http://blog.epnwcf.com/Article/details/gtymtcpum.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.vehdjk.com/Article/details/giiadykdy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.tarul.cn/Article/details/ggbamousg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.epnwcf.com/Article/details/gnfcofovo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fktsv.cn/Article/details/gdozghwrc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.yfazqb.com/Article/details/gvcwmnpzc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.tarul.cn/Article/details/gtihpewfz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fktsv.cn/Article/details/gxdmwskng.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.tarul.cn/Article/details/gkeaztqly.sHtML

Ruby: a == b
来源：http://wap.fktsv.cn/Article/details/gjjvtuvww.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fktsv.cn/Article/details/glmyptecz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.yfazqb.com/Article/details/gccwtbege.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzhznonp.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.yfazqb.com/Article/details/gpfpxisel.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.tarul.cn/Article/details/givkqrdda.sHtML

TS:   if (x == null) {}
来源：http://m.share.bbcook.cn/Article/details/gqtismmao.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gwrjefcra.sHtML

Go:   if x == nil {}
来源：http://baike.epnwcf.com/Article/details/gepmlyjlj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.vehdjk.com/Article/details/gwwyuxavw.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fktsv.cn/Article/details/gcuzhgldj.sHtML

[P07] 防抖与节流
来源：http://blog.bbcook.cn/Article/details/gzrwdwbid.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.sjlbkw.cn/Article/details/gpyhicwkz.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.vehdjk.com/Article/details/gisxlmowj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gmzrudixq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gshwwjmtd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.tarul.cn/Article/details/gjdpmomko.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.sjlbkw.cn/Article/details/gogcsiuux.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.tarul.cn/Article/details/gmgskzoyo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.bbcook.cn/Article/details/gjphhybmr.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.epnwcf.com/Article/details/grwouwpyw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.sjlbkw.cn/Article/details/gpnuukpng.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.tarul.cn/Article/details/gqoyyoyae.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.vehdjk.com/Article/details/ghoxighlm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.sjlbkw.cn/Article/details/goolzfpaa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.yfazqb.com/Article/details/gwhdwijkb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.tarul.cn/Article/details/gjjjdftsa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fktsv.cn/Article/details/grluosweu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.tarul.cn/Article/details/gcmdunsbo.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjthfzkmi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fktsv.cn/Article/details/grixnicnr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gfovsimed.sHtML

[Q01] 创建表
来源：http://3g.epnwcf.com/Article/details/gailcbqvx.sHtML

CREATE TABLE users (
来源：http://3g.yfazqb.com/Article/details/gsrdxuiwi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gujzkseof.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gnhejtdmq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.tarul.cn/Article/details/gquaxbcun.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.bbcook.cn/Article/details/gyvoxhozw.sHtML

);
来源：http://blog.tarul.cn/Article/details/gqlagbwru.sHtML

[Q02] 创建带外键的表
来源：http://mobile.sjlbkw.cn/Article/details/gctprfkta.sHtML

CREATE TABLE orders (
来源：http://mobile.bbcook.cn/Article/details/gywjzpjdk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.vehdjk.com/Article/details/ghbifrinj.sHtML

user_id INT NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/gmgovzslh.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.yfazqb.com/Article/details/gshzgxelb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.bbcook.cn/Article/details/gcrojjgkc.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gnbkonfxu.sHtML

[Q03] 增加列
来源：http://baike.bbcook.cn/Article/details/gspqjhiuv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.yfazqb.com/Article/details/gzmidierw.sHtML

[Q04] 修改列类型
来源：http://baike.tarul.cn/Article/details/gqapzketd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.epnwcf.com/Article/details/gidoisphq.sHtML

[Q05] 重命名列
来源：http://3g.vehdjk.com/Article/details/gtzgpdeiq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.vehdjk.com/Article/details/gxfkdjrqf.sHtML

[Q06] 删除列
来源：http://www.m.share.sjlbkw.cn/Article/details/gffwglumd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.yfazqb.com/Article/details/getoevkju.sHtML

[Q07] 删除表
来源：http://blog.sjlbkw.cn/Article/details/gkphupxtc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.tarul.cn/Article/details/ghveyujty.sHtML

[Q08] 创建普通索引
来源：http://baike.tarul.cn/Article/details/gwqmqzyln.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.tarul.cn/Article/details/gtqujhoqi.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.yfazqb.com/Article/details/gmnjcscna.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.bbcook.cn/Article/details/ghngspxxi.sHtML

[Q10] 插入单行
来源：http://wap.epnwcf.com/Article/details/ghecnwpsc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.vehdjk.com/Article/details/giymdprqf.sHtML

[Q11] 一次插入多行
来源：http://3g.fktsv.cn/Article/details/ggwswkvdm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fktsv.cn/Article/details/ggqlooktg.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.epnwcf.com/Article/details/gafxnmlwr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fktsv.cn/Article/details/gomzzaypo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.vehdjk.com/Article/details/gmawczcko.sHtML

[Q13] 忽略重复插入
来源：http://wap.tarul.cn/Article/details/giatqzzpt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gvixdtacm.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.yfazqb.com/Article/details/gsblhqacd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.tarul.cn/Article/details/giltoucjs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.sjlbkw.cn/Article/details/givffwpub.sHtML

[Q15] 查询全部
来源：http://m.share.vehdjk.com/Article/details/gitjmcaqy.sHtML

SELECT * FROM users;
来源：http://baike.bbcook.cn/Article/details/gqmwrlgbr.sHtML

[Q16] 查询指定列
来源：http://3g.bbcook.cn/Article/details/gkiuyfeph.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gxnkulpwh.sHtML

[Q17] 条件查询
来源：http://3g.bbcook.cn/Article/details/gyxheldti.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gwcecejvx.sHtML

[Q18] 模糊匹配
来源：http://wap.sjlbkw.cn/Article/details/gsyvauwqe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.tarul.cn/Article/details/gwccjydhe.sHtML

[Q19] 范围查询
来源：http://m.share.epnwcf.com/Article/details/gotjyevxm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.bbcook.cn/Article/details/ggpfvdhug.sHtML

[Q20] IN 列表
来源：http://read.share.fktsv.cn/Article/details/ghbvrrxft.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.tarul.cn/Article/details/gvqyjvngw.sHtML

[Q21] 空值判断
来源：http://baike.sjlbkw.cn/Article/details/gdubwodom.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.tarul.cn/Article/details/gelrbqzte.sHtML

[Q22] 排序
来源：http://www.share.epnwcf.com/Article/details/gjnoeviid.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fktsv.cn/Article/details/gonakbrli.sHtML

[Q23] 分页
来源：http://www.blog.tarul.cn/Article/details/gyowkmetk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.vehdjk.com/Article/details/gbifqgeoy.sHtML

[Q24] 去重
来源：http://baike.sjlbkw.cn/Article/details/gkjrdwyur.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/giqdyrxog.sHtML

[Q25] 只取前 N 条
来源：http://m.share.vehdjk.com/Article/details/gkzbnduno.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.epnwcf.com/Article/details/ggybmkpst.sHtML

[Q26] 计数
来源：http://m.share.fktsv.cn/Article/details/gxszmzfcn.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.bbcook.cn/Article/details/giaemzocy.sHtML

[Q27] 条件计数
来源：http://m.share.vehdjk.com/Article/details/gikrxmoqb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.bbcook.cn/Article/details/ghwzfooom.sHtML

[Q28] 求和与平均
来源：http://baike.yfazqb.com/Article/details/gyuhdfoew.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gkfskpllt.sHtML

[Q29] 最大最小值
来源：http://baike.sjlbkw.cn/Article/details/gedadxcxd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gzzxarzyx.sHtML

[Q30] 分组统计
来源：http://m.share.sjlbkw.cn/Article/details/guhpollhg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gssjhwzgi.sHtML

[Q31] 分组后过滤
来源：http://3g.sjlbkw.cn/Article/details/gqiiayfgq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.epnwcf.com/Article/details/gepagvgjj.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.yfazqb.com/Article/details/glplaobia.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gzpqzswwl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.tarul.cn/Article/details/gpgbkkfrj.sHtML

[Q33] 多列分组
来源：http://baike.fktsv.cn/Article/details/gnweygixx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.bbcook.cn/Article/details/gqvcuzgku.sHtML

[Q34] 每组取第一条
来源：http://www.share.epnwcf.com/Article/details/gsxvmiwzc.sHtML

SELECT * FROM (
来源：http://3g.epnwcf.com/Article/details/gpsivxvhx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.sjlbkw.cn/Article/details/gnvjoxysu.sHtML

) t WHERE rn = 1;
来源：http://mobile.tarul.cn/Article/details/gqnansyfo.sHtML

[Q35] 内连接
来源：http://wap.sjlbkw.cn/Article/details/gpgtuuvhk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/glztcorxr.sHtML

[Q36] 左连接
来源：http://wap.yfazqb.com/Article/details/gkunaufbc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gdjszkrhj.sHtML

[Q37] 右连接
来源：http://blog.fktsv.cn/Article/details/gcgcocbyg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.vehdjk.com/Article/details/gpmvomrdf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.yfazqb.com/Article/details/givgdlgzy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.sjlbkw.cn/Article/details/gjifhtxwr.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.bbcook.cn/Article/details/glpxcneqr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.bbcook.cn/Article/details/gnjcvfxep.sHtML


<!-- 参考信息 -->