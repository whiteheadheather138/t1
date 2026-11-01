代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gufwzjnxl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.vehdjk.com/Article/details/gzfhugyxk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fktsv.cn/Article/details/gblzwxdvb.sHtML

Ruby: a.gcd(b)
来源：http://blog.yfazqb.com/Article/details/gldizrfdg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.vehdjk.com/Article/details/gpnkmqkxi.sHtML

[N06] 判断回文字符串
来源：http://read.share.epnwcf.com/Article/details/gudhrgofo.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/gryzpwyqb.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gjdynbzqt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gqsxertoo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gtoekygqi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.vehdjk.com/Article/details/gqsnlqnuc.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.yfazqb.com/Article/details/geumhfeum.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gdrtqkmsa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/ggoreefdh.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.sjlbkw.cn/Article/details/glzpvznum.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.sjlbkw.cn/Article/details/gfyqbuckl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.vehdjk.com/Article/details/gmoybhbea.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.bbcook.cn/Article/details/gwskntewy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/gjupkruif.sHtML

Java: // 手写 HashMap
来源：http://wap.sjlbkw.cn/Article/details/gerpmpumx.sHtML

Go:   // 手写 map[int]int
来源：http://baike.epnwcf.com/Article/details/gjyyngxlq.sHtML

Ruby: // 手写 Hash
来源：http://read.share.bbcook.cn/Article/details/gruognebb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/gsfkmcjbo.sHtML

[N08] 生成全排列
来源：http://wap.fktsv.cn/Article/details/gbbxpyohn.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.epnwcf.com/Article/details/gcoukwfty.sHtML

PHP:  // 手写递归交换
来源：http://wap.yfazqb.com/Article/details/gbhzzltki.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gcdsqrzvz.sHtML

TS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/glqxwvvdo.sHtML

Java: // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gycrhtcia.sHtML

Go:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gyfixtbhi.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.epnwcf.com/Article/details/gomkeipha.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gdhaylljj.sHtML

[N09] 栈与队列
来源：http://blog.vehdjk.com/Article/details/gokkmtwcq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.sjlbkw.cn/Article/details/ghibhtdsb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gmefygjsz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gfieccvcq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.vehdjk.com/Article/details/gvkfbwfsy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.tarul.cn/Article/details/gmsivwyec.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.yfazqb.com/Article/details/gbnqtnsnp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gmqsnjzbr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.epnwcf.com/Article/details/gjrufhqsz.sHtML

[N10] 链表节点定义
来源：http://blog.bbcook.cn/Article/details/gspalsiwb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fktsv.cn/Article/details/gxcekigis.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fktsv.cn/Article/details/gobvoioxc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.bbcook.cn/Article/details/gwblkoidi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.yfazqb.com/Article/details/gztvxvqhj.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.sjlbkw.cn/Article/details/gefwsqrsw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fktsv.cn/Article/details/gacyemgkv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fktsv.cn/Article/details/gearhanke.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.yfazqb.com/Article/details/gyqtdzyit.sHtML

[N11] 二叉树中序遍历
来源：http://blog.vehdjk.com/Article/details/grafofkce.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fktsv.cn/Article/details/ggfuyyaij.sHtML

PHP:  // 手写递归函数
来源：http://baike.sjlbkw.cn/Article/details/gelgjtldf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gqelnnrfb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gxsqehxfe.sHtML

Java: // 手写递归
来源：http://wap.epnwcf.com/Article/details/gknvwiidr.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gsshqqhux.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.sjlbkw.cn/Article/details/grkqunumz.sHtML

C#:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gtcwvabhz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.bbcook.cn/Article/details/gyjthcxwa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.yfazqb.com/Article/details/gsqkmrgwp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.sjlbkw.cn/Article/details/gmpohjqkg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gdpwfknyh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/girtjmwzj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/gebsfysva.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.vehdjk.com/Article/details/glwvsockh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.sjlbkw.cn/Article/details/gjvsrprlu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/gynhsptsj.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gflsrwkdp.sHtML

O. 并发与异步
来源：http://www.m.share.vehdjk.com/Article/details/gierfdcee.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwqjotmvb.sHtML

[O01] 启动一个线程
来源：http://blog.bbcook.cn/Article/details/gxnwtmvbl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.sjlbkw.cn/Article/details/gtwqsxtgc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/gdzajxnzn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.tarul.cn/Article/details/gtvdbcaxe.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/gooqfvgmk.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gfwnrcqex.sHtML

Go:   go f()
来源：http://blog.tarul.cn/Article/details/gnenbdtth.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.tarul.cn/Article/details/gmaanpebm.sHtML

C#:   Task.Run(() => F());
来源：http://wap.vehdjk.com/Article/details/godwaftdh.sHtML

[O02] 使用线程池
来源：http://mobile.tarul.cn/Article/details/gxhrkysnq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.tarul.cn/Article/details/gnqbfvlsw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.sjlbkw.cn/Article/details/ghmsskcjf.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gxgdnuqdw.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/gplpzjghp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.sjlbkw.cn/Article/details/glbfmlxmm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.vehdjk.com/Article/details/gzmjsceaj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.vehdjk.com/Article/details/ghbmjujlm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fktsv.cn/Article/details/grsngonei.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.sjlbkw.cn/Article/details/gbuqmwifx.sHtML

Py:   with lock: shared += 1
来源：http://read.share.bbcook.cn/Article/details/gdaucqsyj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.epnwcf.com/Article/details/gicwhdsvq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fktsv.cn/Article/details/gvavbkqyc.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/gykpaltpe.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fktsv.cn/Article/details/giymcvvar.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.tarul.cn/Article/details/guuhawsbx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fktsv.cn/Article/details/gnqwqteso.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/ghxqhmfyz.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/grzivdwfn.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.tarul.cn/Article/details/grwolsbct.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gupframcv.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gatoglxtt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.bbcook.cn/Article/details/gakztevge.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgpeqvow.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fktsv.cn/Article/details/gzgvhoxrn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fktsv.cn/Article/details/gwxlufxtg.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.vehdjk.com/Article/details/gmqsxaoeb.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fktsv.cn/Article/details/grkhikdje.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/gerxuwtli.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.tarul.cn/Article/details/gqiynrpou.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gesegjnvz.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fktsv.cn/Article/details/gupsgzbrw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.yfazqb.com/Article/details/gtdjptdgz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.sjlbkw.cn/Article/details/gzvzvruvf.sHtML

Ruby: threads.map(&:join)
来源：http://3g.bbcook.cn/Article/details/gqdgfdmzv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fktsv.cn/Article/details/grtivkaqj.sHtML

[O06] 使用进程池
来源：http://m.share.tarul.cn/Article/details/gjlxwrvhk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.bbcook.cn/Article/details/gprsddioq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.epnwcf.com/Article/details/gnminauye.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gotkevose.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gkgxtchgc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fktsv.cn/Article/details/grhfldeak.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.sjlbkw.cn/Article/details/glbpfwcge.sHtML

Ruby: // fork 块
来源：http://3g.sjlbkw.cn/Article/details/grzhqcmez.sHtML

C#:   Parallel.For
来源：http://baike.bbcook.cn/Article/details/ghinzcztg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grzejitid.sHtML

P. 常用工具函数
来源：http://www.share.epnwcf.com/Article/details/grdaluazm.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gutzkujgy.sHtML

[P01] 生成 UUID
来源：http://www.share.fktsv.cn/Article/details/gocjzqoqm.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.epnwcf.com/Article/details/gljpnbjzj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gmuochwzt.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/gjvndkszr.sHtML

TS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gjpuqjmzt.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.tarul.cn/Article/details/giyteqozq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.bbcook.cn/Article/details/gsutczrax.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.tarul.cn/Article/details/goicpnizs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fktsv.cn/Article/details/gyzgnzapr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fktsv.cn/Article/details/gzxqjztss.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.bbcook.cn/Article/details/guluzhozi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.epnwcf.com/Article/details/gcpnoafpt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.yfazqb.com/Article/details/gsqfwaesl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.bbcook.cn/Article/details/gcvcjkuav.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.vehdjk.com/Article/details/gwouocnfe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.yfazqb.com/Article/details/gjahzxhnx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.bbcook.cn/Article/details/goqeimlcq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.sjlbkw.cn/Article/details/ghsuswjpt.sHtML

[P03] 生成短随机字符串
来源：http://wap.fktsv.cn/Article/details/gxopvvnee.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fktsv.cn/Article/details/gizzikuya.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.epnwcf.com/Article/details/ggawatgto.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gkaohoulm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gzuxlxteh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.vehdjk.com/Article/details/gimvwmgua.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.sjlbkw.cn/Article/details/ggaspgcjs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.epnwcf.com/Article/details/gdvryufnd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.epnwcf.com/Article/details/gseezblfe.sHtML

[P04] 求长度
来源：http://www.blog.fktsv.cn/Article/details/gjsahuios.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.sjlbkw.cn/Article/details/gbkleokae.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/giaaybbjn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/glqdxzyng.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gxhorzgqy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.bbcook.cn/Article/details/ghkiiyoes.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.sjlbkw.cn/Article/details/gxjaoeqcn.sHtML

Ruby: x.length;  x.size
来源：http://m.share.vehdjk.com/Article/details/gpagxjykj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.yfazqb.com/Article/details/gbushptpg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/gpupidmwe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.tarul.cn/Article/details/gcnklfuqr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fktsv.cn/Article/details/geuqrorrp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.tarul.cn/Article/details/gfkbxqcwp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.tarul.cn/Article/details/giqtyakqe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.yfazqb.com/Article/details/gbndsolev.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.yfazqb.com/Article/details/gyclirsxb.sHtML

Ruby: a == b
来源：http://read.share.tarul.cn/Article/details/gnmmujhte.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fktsv.cn/Article/details/gyeqzncya.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fktsv.cn/Article/details/gclmyrzgq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.tarul.cn/Article/details/glsziufnq.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.bbcook.cn/Article/details/gmwjtnste.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.bbcook.cn/Article/details/gpspnuxbr.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fktsv.cn/Article/details/gwusauibn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhuhbubw.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/gqmgsipma.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fktsv.cn/Article/details/gynfwqxbl.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmwausqv.sHtML

[P07] 防抖与节流
来源：http://read.share.tarul.cn/Article/details/gpenexpsu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.bbcook.cn/Article/details/gbjecamfe.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.epnwcf.com/Article/details/gbhdsryln.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/grprhekai.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gbqwlcdsc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.bbcook.cn/Article/details/gcvkvzvwa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fktsv.cn/Article/details/gmnipewsb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.yfazqb.com/Article/details/gedoxvkad.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fktsv.cn/Article/details/gjtjkafnr.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.yfazqb.com/Article/details/gdhevbgbq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.vehdjk.com/Article/details/gdaprabzp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.bbcook.cn/Article/details/gezqpfddf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fktsv.cn/Article/details/guamfjirq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gsnixaflj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.yfazqb.com/Article/details/gbvgijioi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.sjlbkw.cn/Article/details/gmklsnulz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.tarul.cn/Article/details/gqnykinvg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.epnwcf.com/Article/details/gaihydmuv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grdcxuqte.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.tarul.cn/Article/details/ggxotxzgs.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqmyrmuuz.sHtML

[Q01] 创建表
来源：http://3g.tarul.cn/Article/details/gdbmpqexs.sHtML

CREATE TABLE users (
来源：http://www.share.yfazqb.com/Article/details/gxljmqujm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/guknrkwxz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/gegdbnhin.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.yfazqb.com/Article/details/gaepfmtfe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.sjlbkw.cn/Article/details/guhscjpow.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gymdifere.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.vehdjk.com/Article/details/gpjgmaffe.sHtML

CREATE TABLE orders (
来源：http://www.blog.epnwcf.com/Article/details/gbroxqwnh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/gdquakpsj.sHtML

user_id INT NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/gkdjiizng.sHtML

amount DECIMAL(10, 2),
来源：http://baike.sjlbkw.cn/Article/details/gyucgfyeq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.sjlbkw.cn/Article/details/gczprfohe.sHtML

);
来源：http://www.blog.fktsv.cn/Article/details/gjdxmanrp.sHtML

[Q03] 增加列
来源：http://m.share.sjlbkw.cn/Article/details/gzquqmarz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/ggeaylyhm.sHtML

[Q04] 修改列类型
来源：http://blog.yfazqb.com/Article/details/ghpeztukd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fktsv.cn/Article/details/gmwtejtlf.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/gkkfpjxtj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.yfazqb.com/Article/details/gxiamtcco.sHtML

[Q06] 删除列
来源：http://blog.fktsv.cn/Article/details/gtvydfauw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.yfazqb.com/Article/details/getrxmjgm.sHtML

[Q07] 删除表
来源：http://www.m.share.epnwcf.com/Article/details/gbqmkszpp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.tarul.cn/Article/details/gpqpvwlyz.sHtML

[Q08] 创建普通索引
来源：http://www.share.tarul.cn/Article/details/gaajpdfjm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.bbcook.cn/Article/details/ggqleeuxl.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fktsv.cn/Article/details/gqtownhul.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gzcoonaww.sHtML

[Q10] 插入单行
来源：http://blog.epnwcf.com/Article/details/gydnyhjsp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.bbcook.cn/Article/details/gohidtvxv.sHtML

[Q11] 一次插入多行
来源：http://baike.tarul.cn/Article/details/gpnpyyosj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.yfazqb.com/Article/details/gikzawhid.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.vehdjk.com/Article/details/gnojnjjqs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.yfazqb.com/Article/details/gvdjnweio.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.yfazqb.com/Article/details/gaahkblik.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fktsv.cn/Article/details/gbhakczfg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.tarul.cn/Article/details/griupadqk.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.bbcook.cn/Article/details/ghbzhdhow.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.epnwcf.com/Article/details/gneqbwccu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.epnwcf.com/Article/details/gwxyidgpd.sHtML

[Q15] 查询全部
来源：http://blog.epnwcf.com/Article/details/gfpghkldz.sHtML

SELECT * FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gkhwvcwyo.sHtML

[Q16] 查询指定列
来源：http://mobile.vehdjk.com/Article/details/gormwidsg.sHtML

SELECT id, name FROM users;
来源：http://mobile.yfazqb.com/Article/details/ggflchcti.sHtML

[Q17] 条件查询
来源：http://www.share.epnwcf.com/Article/details/gcozwbksr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.yfazqb.com/Article/details/giqfosvws.sHtML

[Q18] 模糊匹配
来源：http://read.share.bbcook.cn/Article/details/gvfwnauzx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fktsv.cn/Article/details/gnuqlpihj.sHtML

[Q19] 范围查询
来源：http://baike.tarul.cn/Article/details/gicmqydjn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.tarul.cn/Article/details/gybvjzqkk.sHtML

[Q20] IN 列表
来源：http://3g.sjlbkw.cn/Article/details/gakcfcgij.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.yfazqb.com/Article/details/gasnffhwi.sHtML

[Q21] 空值判断
来源：http://baike.yfazqb.com/Article/details/gyqgmhzvo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/gvmiwoavv.sHtML

[Q22] 排序
来源：http://m.share.epnwcf.com/Article/details/gxfhkaqxb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.epnwcf.com/Article/details/gsuijqdqx.sHtML

[Q23] 分页
来源：http://wap.bbcook.cn/Article/details/ggbbjwjxf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.vehdjk.com/Article/details/gutfzcsxc.sHtML

[Q24] 去重
来源：http://read.share.yfazqb.com/Article/details/gihxewfrw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.epnwcf.com/Article/details/gvvoeyqgb.sHtML

[Q25] 只取前 N 条
来源：http://mobile.tarul.cn/Article/details/gihnqjool.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.vehdjk.com/Article/details/gppvdydyf.sHtML

[Q26] 计数
来源：http://www.share.yfazqb.com/Article/details/gpzvqucne.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.vehdjk.com/Article/details/ghjgykytp.sHtML

[Q27] 条件计数
来源：http://blog.epnwcf.com/Article/details/gdjyxbxhp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gprvrnovl.sHtML

[Q28] 求和与平均
来源：http://www.share.yfazqb.com/Article/details/glogqgjlw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gevinjikg.sHtML

[Q29] 最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/gjzyqxywn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gnsuwoqum.sHtML

[Q30] 分组统计
来源：http://blog.vehdjk.com/Article/details/gokrlkswi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/getbchsxg.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/gwhvmfnea.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fktsv.cn/Article/details/gxmjeufwm.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fktsv.cn/Article/details/gwtbuqycg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gzhpjkhhe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fktsv.cn/Article/details/gqczedjgc.sHtML

[Q33] 多列分组
来源：http://read.share.epnwcf.com/Article/details/goiwdqalx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.vehdjk.com/Article/details/gxcbtpyux.sHtML

[Q34] 每组取第一条
来源：http://www.blog.epnwcf.com/Article/details/gevlbgsdm.sHtML

SELECT * FROM (
来源：http://read.share.epnwcf.com/Article/details/gkhngvtye.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.bbcook.cn/Article/details/gjiwcodju.sHtML

) t WHERE rn = 1;
来源：http://www.blog.tarul.cn/Article/details/gxdxwdblf.sHtML

[Q35] 内连接
来源：http://www.share.sjlbkw.cn/Article/details/gkaoqauvt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gyfxufcoh.sHtML

[Q36] 左连接
来源：http://3g.yfazqb.com/Article/details/gupzxljhm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/gmaauqrgi.sHtML

[Q37] 右连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuyrbkmh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fktsv.cn/Article/details/gzzyowwwc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.vehdjk.com/Article/details/gvxwswcyi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.epnwcf.com/Article/details/gffyiamlp.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.yfazqb.com/Article/details/gdkxcozrw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.epnwcf.com/Article/details/gxfqaflvo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.yfazqb.com/Article/details/gtegwfggu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.yfazqb.com/Article/details/grcltfinl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.tarul.cn/Article/details/guqhvieto.sHtML

[Q41] 多表连接
来源：http://mobile.epnwcf.com/Article/details/gbmymiutk.sHtML


<!-- 参考信息 -->