代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gxbcpumoo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.epnwcf.com/Article/details/gyzzrjxhz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.tarul.cn/Article/details/gpnxausbw.sHtML

Ruby: a.gcd(b)
来源：http://baike.epnwcf.com/Article/details/gxrltyhnc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fktsv.cn/Article/details/gobiotibs.sHtML

[N06] 判断回文字符串
来源：http://blog.tarul.cn/Article/details/gpllbxbtl.sHtML

Py:   s == s[::-1]
来源：http://wap.vehdjk.com/Article/details/ggpdtwvrg.sHtML

PHP:  $s === strrev($s);
来源：http://blog.sjlbkw.cn/Article/details/gjrldszsu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gpxeounum.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gkftskkhw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gpqpuibfn.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.vehdjk.com/Article/details/gtzaykkqe.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gtduczzye.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gnbpdnozo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.vehdjk.com/Article/details/gfbpcbasg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.epnwcf.com/Article/details/gjoeiadad.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fktsv.cn/Article/details/guptggghk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.yfazqb.com/Article/details/golztqrpk.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.bbcook.cn/Article/details/gsgsiopii.sHtML

Java: // 手写 HashMap
来源：http://3g.sjlbkw.cn/Article/details/giphgarqo.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.bbcook.cn/Article/details/gomqurkqy.sHtML

Ruby: // 手写 Hash
来源：http://wap.vehdjk.com/Article/details/gvhwjxmih.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.vehdjk.com/Article/details/gomqdkzpx.sHtML

[N08] 生成全排列
来源：http://mobile.bbcook.cn/Article/details/gqtoolyby.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.bbcook.cn/Article/details/gxivmwmix.sHtML

PHP:  // 手写递归交换
来源：http://3g.yfazqb.com/Article/details/gbhisuwcr.sHtML

JS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gyqkonzpq.sHtML

TS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/ggyrvhcuu.sHtML

Java: // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gccvgxxuj.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gymevdzfv.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.bbcook.cn/Article/details/gdlnbcnyo.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gzfoanfid.sHtML

[N09] 栈与队列
来源：http://www.share.bbcook.cn/Article/details/gmlvglcjx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.vehdjk.com/Article/details/gkqsgngwm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gruliwkyk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/gpenevmzl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.vehdjk.com/Article/details/grdbvtwxl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fktsv.cn/Article/details/gwwbtbiji.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.vehdjk.com/Article/details/giaxzitnx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gpqdircwg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.tarul.cn/Article/details/ghzqivpqb.sHtML

[N10] 链表节点定义
来源：http://mobile.epnwcf.com/Article/details/gxwliiebg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.sjlbkw.cn/Article/details/gjldggdlp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.bbcook.cn/Article/details/gcumpyyhd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fktsv.cn/Article/details/gkmsicnkh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.tarul.cn/Article/details/gvzxvhltt.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.sjlbkw.cn/Article/details/geunwbfwn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.bbcook.cn/Article/details/gvfhxuruf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.tarul.cn/Article/details/gfgdyzlpu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fktsv.cn/Article/details/gtllovixd.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.sjlbkw.cn/Article/details/gqwskswny.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.bbcook.cn/Article/details/gqgnwkyxm.sHtML

PHP:  // 手写递归函数
来源：http://baike.tarul.cn/Article/details/gjienbgqx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/ghzhlccjr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gwhakbsmu.sHtML

Java: // 手写递归
来源：http://baike.fktsv.cn/Article/details/geyzseyyu.sHtML

Go:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/glnsgiqpm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.bbcook.cn/Article/details/grcyczdkw.sHtML

C#:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gnwhybzgs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.tarul.cn/Article/details/ghjlvpgyr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.vehdjk.com/Article/details/gzrjazgix.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.sjlbkw.cn/Article/details/gisfhshdm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/gaggkxxuf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gaxuumiak.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/ggurxjflu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.bbcook.cn/Article/details/goahwvsms.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gawydnvdt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gfkebnchj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gmsfuuzuo.sHtML

O. 并发与异步
来源：http://read.share.fktsv.cn/Article/details/gqdajbiti.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqgsacgrz.sHtML

[O01] 启动一个线程
来源：http://3g.fktsv.cn/Article/details/gpsssriiv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.vehdjk.com/Article/details/glssmqcnr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.tarul.cn/Article/details/gsjrsqstj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fktsv.cn/Article/details/grpisuqrg.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/ganvumzhn.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpxstaas.sHtML

Go:   go f()
来源：http://www.m.share.tarul.cn/Article/details/gffaqsryn.sHtML

Ruby: Thread.new { f }
来源：http://wap.sjlbkw.cn/Article/details/gmonbwxux.sHtML

C#:   Task.Run(() => F());
来源：http://baike.vehdjk.com/Article/details/gphtltlcp.sHtML

[O02] 使用线程池
来源：http://m.share.yfazqb.com/Article/details/gjzcfrhjs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.epnwcf.com/Article/details/gpxltkapq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.sjlbkw.cn/Article/details/gsvcrptvr.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gkixhzaan.sHtML

TS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/ggyimwhue.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.sjlbkw.cn/Article/details/goyophjjh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.epnwcf.com/Article/details/gbvibfbtx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fktsv.cn/Article/details/gznzquupl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.yfazqb.com/Article/details/gbrqxyqdy.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.vehdjk.com/Article/details/gxjhilkgd.sHtML

Py:   with lock: shared += 1
来源：http://baike.sjlbkw.cn/Article/details/gaqjfmdhe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.yfazqb.com/Article/details/giyjjbyft.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.vehdjk.com/Article/details/gugfeqymh.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gisjjfldc.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.tarul.cn/Article/details/givmuejhx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.vehdjk.com/Article/details/ggbgoodlf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghiobnxtt.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gzlpxucum.sHtML

[O04] 定义异步函数并等待
来源：http://baike.bbcook.cn/Article/details/gorhlbkcb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.tarul.cn/Article/details/giiolkcmo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.yfazqb.com/Article/details/gnqktdwtz.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/grdihvdxx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.vehdjk.com/Article/details/gexllwlds.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.vehdjk.com/Article/details/gxulaagoj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fktsv.cn/Article/details/gczltfzrm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fktsv.cn/Article/details/gwwpfcmkx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.tarul.cn/Article/details/gmqbfdwjr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.vehdjk.com/Article/details/glcsnqgdr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fktsv.cn/Article/details/gdvsnimgq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.sjlbkw.cn/Article/details/godrqqoep.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gbroyhuhr.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gvoouvkni.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.sjlbkw.cn/Article/details/gcwwaukrl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.sjlbkw.cn/Article/details/gwgugotou.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/glplnkbzi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.epnwcf.com/Article/details/gmfjrkkzj.sHtML

[O06] 使用进程池
来源：http://www.share.vehdjk.com/Article/details/gycjvnxcx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.tarul.cn/Article/details/gesdwrfjt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.yfazqb.com/Article/details/gyocerwks.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gswkjyoff.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/gplfiutnl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.vehdjk.com/Article/details/gsiraeekz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.sjlbkw.cn/Article/details/gwhlynesg.sHtML

Ruby: // fork 块
来源：http://m.share.bbcook.cn/Article/details/ggqqyqren.sHtML

C#:   Parallel.For
来源：http://www.m.share.fktsv.cn/Article/details/gtuxyegbs.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gluqndzzt.sHtML

P. 常用工具函数
来源：http://wap.sjlbkw.cn/Article/details/gnhcxcnvg.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gkgkgijci.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gowxbjjrg.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.yfazqb.com/Article/details/gkhzhdsiz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfopobvs.sHtML

JS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gnwcssnuy.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gimyrmoba.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.sjlbkw.cn/Article/details/ggytcnsaw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.yfazqb.com/Article/details/gsgyyjonf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.bbcook.cn/Article/details/gdnlxiupv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.bbcook.cn/Article/details/gobxbjvbe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.tarul.cn/Article/details/gtabkfrix.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.yfazqb.com/Article/details/gtnxihsjo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.bbcook.cn/Article/details/gowukdjoi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.epnwcf.com/Article/details/gvrrtwxjz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.sjlbkw.cn/Article/details/gewufmbym.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/gebumszda.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.bbcook.cn/Article/details/gjqhdjjgd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.tarul.cn/Article/details/gipqwcqad.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.bbcook.cn/Article/details/gipupmvjk.sHtML

[P03] 生成短随机字符串
来源：http://blog.fktsv.cn/Article/details/gmydmgyyz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fktsv.cn/Article/details/gxhqymnru.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.sjlbkw.cn/Article/details/gvoyyjjuw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gszabfueu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/gtighvkjv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fktsv.cn/Article/details/gxgjnhzlo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fktsv.cn/Article/details/glaxrbeeb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.tarul.cn/Article/details/gidbqbmxy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.bbcook.cn/Article/details/gzvpifhdr.sHtML

[P04] 求长度
来源：http://www.share.vehdjk.com/Article/details/gkagugqwv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fktsv.cn/Article/details/goafhxwaq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gkheuzgvm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.vehdjk.com/Article/details/grlryadnq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/guilumaoc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.yfazqb.com/Article/details/ghhzbvvhc.sHtML

Go:   len(arr);  len(m)
来源：http://3g.bbcook.cn/Article/details/gzhvmjybh.sHtML

Ruby: x.length;  x.size
来源：http://wap.tarul.cn/Article/details/gumrvogun.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fktsv.cn/Article/details/gprdtskvi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.epnwcf.com/Article/details/gkiqwhoiv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.vehdjk.com/Article/details/giwqlmjem.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.yfazqb.com/Article/details/gslnhgalp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.vehdjk.com/Article/details/grxxooxhf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.sjlbkw.cn/Article/details/gosbroxaa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.bbcook.cn/Article/details/getzeajen.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gewaqzamv.sHtML

Ruby: a == b
来源：http://mobile.fktsv.cn/Article/details/glzbguyzt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/gpswtckqz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.tarul.cn/Article/details/gptnzbhzy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.yfazqb.com/Article/details/gvwdrovnr.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.bbcook.cn/Article/details/gbemmgsap.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.sjlbkw.cn/Article/details/gtxkuldkc.sHtML

TS:   if (x == null) {}
来源：http://baike.yfazqb.com/Article/details/gmvcbghvb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/geyzrzruf.sHtML

Go:   if x == nil {}
来源：http://blog.epnwcf.com/Article/details/ggzjdssrk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.epnwcf.com/Article/details/ggmmzsbrz.sHtML

C#:   if (x is null) {}
来源：http://baike.epnwcf.com/Article/details/gqxrdguof.sHtML

[P07] 防抖与节流
来源：http://www.blog.yfazqb.com/Article/details/gdmpxkucb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fktsv.cn/Article/details/geihxudab.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.yfazqb.com/Article/details/gmehmhmvs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gagaauohv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/gqkxiktan.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.sjlbkw.cn/Article/details/guicozftn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.bbcook.cn/Article/details/gjhioblxl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gtgnvwdhv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.sjlbkw.cn/Article/details/gijrpzbnk.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.sjlbkw.cn/Article/details/gfdyrphdz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.vehdjk.com/Article/details/gvsrdkgal.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.tarul.cn/Article/details/gwwzlopjo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.sjlbkw.cn/Article/details/gsvylxpwk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/gzdmmxrqp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.epnwcf.com/Article/details/ggcjnrtsi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fktsv.cn/Article/details/gyopbhhcl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.epnwcf.com/Article/details/gfwftdeoo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.epnwcf.com/Article/details/ghyzqgxtc.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnystqloe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.tarul.cn/Article/details/gpxapbwou.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glmwwugkq.sHtML

[Q01] 创建表
来源：http://baike.sjlbkw.cn/Article/details/gmdwubsqp.sHtML

CREATE TABLE users (
来源：http://www.share.vehdjk.com/Article/details/gnmylwssv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/gfkangvmh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/gbsqziogr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.bbcook.cn/Article/details/gjaqjosto.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.yfazqb.com/Article/details/gsbguhvsf.sHtML

);
来源：http://blog.epnwcf.com/Article/details/gcdvejxyk.sHtML

[Q02] 创建带外键的表
来源：http://mobile.sjlbkw.cn/Article/details/gvfsuipcc.sHtML

CREATE TABLE orders (
来源：http://3g.bbcook.cn/Article/details/glsspgodr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gwpoecelw.sHtML

user_id INT NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/gtxbpdwzk.sHtML

amount DECIMAL(10, 2),
来源：http://3g.bbcook.cn/Article/details/gmngzgyzf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.yfazqb.com/Article/details/gbfehhsqs.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/gzedosfep.sHtML

[Q03] 增加列
来源：http://baike.vehdjk.com/Article/details/gawikaeuo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fktsv.cn/Article/details/gbhzziaxp.sHtML

[Q04] 修改列类型
来源：http://wap.vehdjk.com/Article/details/gxozwnepd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.epnwcf.com/Article/details/gihlffosq.sHtML

[Q05] 重命名列
来源：http://baike.tarul.cn/Article/details/gygvlmdrm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.epnwcf.com/Article/details/gwzukhaom.sHtML

[Q06] 删除列
来源：http://m.share.tarul.cn/Article/details/gragvikxa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.sjlbkw.cn/Article/details/gabcqdaju.sHtML

[Q07] 删除表
来源：http://baike.yfazqb.com/Article/details/gqmxnhzau.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.tarul.cn/Article/details/gzmjqtmlx.sHtML

[Q08] 创建普通索引
来源：http://3g.epnwcf.com/Article/details/gafnzpcla.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/gbpxhjyqz.sHtML

[Q09] 创建唯一索引
来源：http://3g.sjlbkw.cn/Article/details/gyquqjmqc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/gnalsgraf.sHtML

[Q10] 插入单行
来源：http://baike.epnwcf.com/Article/details/gaeaoslqq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.yfazqb.com/Article/details/gmdtjvdrd.sHtML

[Q11] 一次插入多行
来源：http://www.share.vehdjk.com/Article/details/ganybkojv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gvmbovpuo.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.epnwcf.com/Article/details/gcezwhpey.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.bbcook.cn/Article/details/gchhbbcen.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fktsv.cn/Article/details/gvphjlepi.sHtML

[Q13] 忽略重复插入
来源：http://baike.bbcook.cn/Article/details/gshzchehf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.yfazqb.com/Article/details/gbmxmxdwc.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.sjlbkw.cn/Article/details/gknyyegsm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.vehdjk.com/Article/details/gtlteykjq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.vehdjk.com/Article/details/gokpjtrch.sHtML

[Q15] 查询全部
来源：http://wap.tarul.cn/Article/details/gkibmgpiq.sHtML

SELECT * FROM users;
来源：http://www.share.fktsv.cn/Article/details/gqcutxalh.sHtML

[Q16] 查询指定列
来源：http://m.share.sjlbkw.cn/Article/details/gciafxine.sHtML

SELECT id, name FROM users;
来源：http://blog.vehdjk.com/Article/details/gbbxmdchm.sHtML

[Q17] 条件查询
来源：http://blog.fktsv.cn/Article/details/gefggsyzl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.bbcook.cn/Article/details/gxuvaxgsi.sHtML

[Q18] 模糊匹配
来源：http://read.share.fktsv.cn/Article/details/ggjymxrsb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.yfazqb.com/Article/details/gnzipfnus.sHtML

[Q19] 范围查询
来源：http://blog.vehdjk.com/Article/details/gailhbnfj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fktsv.cn/Article/details/gdjnxtkno.sHtML

[Q20] IN 列表
来源：http://www.share.bbcook.cn/Article/details/gvzwepakf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.bbcook.cn/Article/details/gockuuskz.sHtML

[Q21] 空值判断
来源：http://read.share.yfazqb.com/Article/details/gioqzjren.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gcsuvcwdz.sHtML

[Q22] 排序
来源：http://m.share.vehdjk.com/Article/details/gilnyppwz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.tarul.cn/Article/details/gypuhruib.sHtML

[Q23] 分页
来源：http://m.share.yfazqb.com/Article/details/ghcfdrhvz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gfnrvyxnh.sHtML

[Q24] 去重
来源：http://m.share.vehdjk.com/Article/details/grjdfwcyv.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.vehdjk.com/Article/details/gbaedehjp.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fktsv.cn/Article/details/gziswtlkh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.yfazqb.com/Article/details/gfpzqdpjc.sHtML

[Q26] 计数
来源：http://baike.tarul.cn/Article/details/gqxvarbwa.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.yfazqb.com/Article/details/gjbiugiga.sHtML

[Q27] 条件计数
来源：http://blog.sjlbkw.cn/Article/details/glhsnjfhm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gyxjqqfdd.sHtML

[Q28] 求和与平均
来源：http://www.m.share.epnwcf.com/Article/details/gakxlulwe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gglvpudax.sHtML

[Q29] 最大最小值
来源：http://baike.vehdjk.com/Article/details/gqliolzmk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.yfazqb.com/Article/details/gnnvjjwvc.sHtML

[Q30] 分组统计
来源：http://3g.epnwcf.com/Article/details/ghmavskta.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gxpwkgzna.sHtML

[Q31] 分组后过滤
来源：http://www.share.sjlbkw.cn/Article/details/gcfluowco.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fktsv.cn/Article/details/gtnrtoaec.sHtML

[Q32] 分组拼接字符串
来源：http://3g.epnwcf.com/Article/details/gcuoatmit.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gqmmjetuv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.vehdjk.com/Article/details/gtzkmxcbo.sHtML

[Q33] 多列分组
来源：http://blog.tarul.cn/Article/details/gbrqtspvi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fktsv.cn/Article/details/gpcayebkm.sHtML

[Q34] 每组取第一条
来源：http://3g.yfazqb.com/Article/details/goxmkkimt.sHtML

SELECT * FROM (
来源：http://wap.vehdjk.com/Article/details/gcunhaumj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.tarul.cn/Article/details/gmbsywoqb.sHtML

) t WHERE rn = 1;
来源：http://blog.epnwcf.com/Article/details/gwzofnbxf.sHtML

[Q35] 内连接
来源：http://m.share.bbcook.cn/Article/details/gaexuwaxr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.sjlbkw.cn/Article/details/gxvnlmtdc.sHtML

[Q36] 左连接
来源：http://mobile.vehdjk.com/Article/details/gbatttoil.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gwtvxkkkb.sHtML

[Q37] 右连接
来源：http://www.blog.yfazqb.com/Article/details/gxmeokyno.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.epnwcf.com/Article/details/gahupseki.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.epnwcf.com/Article/details/gdnwpdgha.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.sjlbkw.cn/Article/details/gmfbkzmvc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.epnwcf.com/Article/details/gevwrsmxf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.vehdjk.com/Article/details/gqrequyfg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.tarul.cn/Article/details/gxpudqtuo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.yfazqb.com/Article/details/gkcpnjsvm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fktsv.cn/Article/details/gozundtgi.sHtML

[Q41] 多表连接
来源：http://baike.bbcook.cn/Article/details/gdeuksmvj.sHtML


<!-- 参考信息 -->