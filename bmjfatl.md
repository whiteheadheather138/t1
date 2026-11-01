代发 wailian999

Py:   itertools.permutations(arr)
来源：http://m.share.bbcook.cn/Article/details/gayoyswzq.sHtML

PHP:  // 手写递归交换
来源：http://wap.yfazqb.com/Article/details/gagmuzqtz.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gbcbdvqnd.sHtML

TS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gyynufuud.sHtML

Java: // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gmygssifj.sHtML

Go:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gwwpdyjvo.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.yfazqb.com/Article/details/gchhrnxbu.sHtML

C#:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gxhogxhpj.sHtML

[N09] 栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/gvddjtfgn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gicqxnkwb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gezgfatjg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gjreertzj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.epnwcf.com/Article/details/gixlodkvz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.bbcook.cn/Article/details/gzneftrfn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.sjlbkw.cn/Article/details/glgolhzns.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gjvkapisi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fktsv.cn/Article/details/gtfrosvzh.sHtML

[N10] 链表节点定义
来源：http://wap.tarul.cn/Article/details/gtevmfugr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.vehdjk.com/Article/details/ghobrffmd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.yfazqb.com/Article/details/gmtdjbbzh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.yfazqb.com/Article/details/gpgaswagz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fktsv.cn/Article/details/gwuoxozpu.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fktsv.cn/Article/details/gvjcsdzis.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.bbcook.cn/Article/details/ggsuygznv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fktsv.cn/Article/details/gyqdlqkjy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.tarul.cn/Article/details/ggxhjyqef.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.vehdjk.com/Article/details/gsbjcnrfs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.vehdjk.com/Article/details/gcxrmkibt.sHtML

PHP:  // 手写递归函数
来源：http://wap.tarul.cn/Article/details/gnblukfnr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/guvsszsgq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/gczezxepa.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gadnaijxw.sHtML

Go:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gpwqawnxs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.yfazqb.com/Article/details/gzuanqlhf.sHtML

C#:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gihuwtuuh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.yfazqb.com/Article/details/gtwmvtklj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.epnwcf.com/Article/details/ggcfucpbm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fktsv.cn/Article/details/glscjtsmd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/gaenfzcyp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/gptcwxzoj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/gbxjxgwta.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.bbcook.cn/Article/details/gfnzlbhzu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.yfazqb.com/Article/details/gnazbqqpz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/gmqorzpry.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gfvftgpxg.sHtML

O. 并发与异步
来源：http://3g.vehdjk.com/Article/details/gkjmdjnsx.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/grkxrlfil.sHtML

[O01] 启动一个线程
来源：http://www.share.tarul.cn/Article/details/grngdjmoe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.tarul.cn/Article/details/gxfdveqxj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.sjlbkw.cn/Article/details/gwqdlpych.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.bbcook.cn/Article/details/gjtzkjxsr.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gttjlwocx.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fktsv.cn/Article/details/gzirbmvcu.sHtML

Go:   go f()
来源：http://www.share.sjlbkw.cn/Article/details/grhzqlohy.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/gdtjgmzqd.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.epnwcf.com/Article/details/gtwdwyxxh.sHtML

[O02] 使用线程池
来源：http://www.blog.epnwcf.com/Article/details/gvgtyugue.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.yfazqb.com/Article/details/gfwcfinmm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fktsv.cn/Article/details/giuzrwtqy.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.tarul.cn/Article/details/gxsgmoqam.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/ganhczjlk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fktsv.cn/Article/details/grllbdlft.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gfwwzowbj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.yfazqb.com/Article/details/ghfkjxfdv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.vehdjk.com/Article/details/gfflrubox.sHtML

[O03] 加锁保护共享数据
来源：http://3g.bbcook.cn/Article/details/gafosgobe.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.vehdjk.com/Article/details/gnautdxdi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.tarul.cn/Article/details/gavhnxviv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.sjlbkw.cn/Article/details/gdtcjjyld.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gamczgbgi.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.bbcook.cn/Article/details/ggthczqey.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/ggpoblyvv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.sjlbkw.cn/Article/details/gofndetce.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqucupejj.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.yfazqb.com/Article/details/gzgufmbvz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.vehdjk.com/Article/details/gpfozwgal.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.bbcook.cn/Article/details/guegbohzd.sHtML

JS:   async function f() { await g(); }
来源：http://blog.sjlbkw.cn/Article/details/gbyqnrltn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.epnwcf.com/Article/details/gqoqgxdtc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.sjlbkw.cn/Article/details/goicpchlx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.yfazqb.com/Article/details/gnullemjf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.yfazqb.com/Article/details/gkkpglafj.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.epnwcf.com/Article/details/ggroyecau.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.bbcook.cn/Article/details/graeddmfb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.epnwcf.com/Article/details/gstzmennk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.epnwcf.com/Article/details/gedpgahqf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/gnoutdgfu.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gkyjabwzy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.bbcook.cn/Article/details/gmrivudac.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.vehdjk.com/Article/details/givcfrxrg.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.tarul.cn/Article/details/gwerlnmjp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.sjlbkw.cn/Article/details/ggldjzajq.sHtML

[O06] 使用进程池
来源：http://baike.yfazqb.com/Article/details/gipxpkqfa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.epnwcf.com/Article/details/gingcmowr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.tarul.cn/Article/details/genatylxg.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.yfazqb.com/Article/details/glvpwwvfe.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.sjlbkw.cn/Article/details/gfqpgywng.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.vehdjk.com/Article/details/gswreigph.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.tarul.cn/Article/details/gqnljcwrb.sHtML

Ruby: // fork 块
来源：http://www.blog.fktsv.cn/Article/details/ghyxnuiib.sHtML

C#:   Parallel.For
来源：http://m.share.sjlbkw.cn/Article/details/gyscixgfs.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gwnllvrmb.sHtML

P. 常用工具函数
来源：http://www.m.share.tarul.cn/Article/details/gfxmndydh.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gxtdtcsoo.sHtML

[P01] 生成 UUID
来源：http://blog.bbcook.cn/Article/details/gqarmdddw.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fktsv.cn/Article/details/grbzhyccc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.epnwcf.com/Article/details/gjqsriqoj.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gwmndhxgd.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/givryshas.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.vehdjk.com/Article/details/goawifxsp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.vehdjk.com/Article/details/gvloohyyb.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.vehdjk.com/Article/details/gwsggoaxo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.yfazqb.com/Article/details/ggpufucoy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.bbcook.cn/Article/details/gnoedgkyn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.yfazqb.com/Article/details/gogpnkzsy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.yfazqb.com/Article/details/gubomsgut.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fktsv.cn/Article/details/gfoyjyzoa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.yfazqb.com/Article/details/guisecczw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.tarul.cn/Article/details/gsbohqaeq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.bbcook.cn/Article/details/grfobcrnd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.yfazqb.com/Article/details/glefaevra.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/gjlixhmdh.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.tarul.cn/Article/details/glymxuzqq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.epnwcf.com/Article/details/gjaikvujq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.epnwcf.com/Article/details/gdeetgjov.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/geirdygez.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/gkjsvrucr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.yfazqb.com/Article/details/gxdhjvphx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.bbcook.cn/Article/details/gxvrqwjfl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.epnwcf.com/Article/details/gsxlicdqw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.tarul.cn/Article/details/gofddagkz.sHtML

[P04] 求长度
来源：http://m.share.yfazqb.com/Article/details/gzcdwkbjc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.vehdjk.com/Article/details/gsnjvlesu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/geyxbczqt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/gaeqihkix.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/gqkuaqxet.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.yfazqb.com/Article/details/gjlfthtfp.sHtML

Go:   len(arr);  len(m)
来源：http://3g.bbcook.cn/Article/details/gdqgtkxkb.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fktsv.cn/Article/details/gznjnadaa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.bbcook.cn/Article/details/gxcfilmju.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.yfazqb.com/Article/details/gmvrmxoxa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.yfazqb.com/Article/details/glgbhfdqo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.epnwcf.com/Article/details/guzaiftmh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.yfazqb.com/Article/details/gwanapfbs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.bbcook.cn/Article/details/gskbwjwaq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.epnwcf.com/Article/details/gityfnnpw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.epnwcf.com/Article/details/givxnctvo.sHtML

Ruby: a == b
来源：http://read.share.yfazqb.com/Article/details/gcryvxipi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.bbcook.cn/Article/details/gkavluppj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.epnwcf.com/Article/details/ggkznqbfv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fktsv.cn/Article/details/ggrvalhjz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gsucdogzb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.vehdjk.com/Article/details/gftcwtawa.sHtML

TS:   if (x == null) {}
来源：http://m.share.sjlbkw.cn/Article/details/gmkppnuyf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gcoucregu.sHtML

Go:   if x == nil {}
来源：http://3g.yfazqb.com/Article/details/goanuwmxm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.vehdjk.com/Article/details/guubceryh.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gmeijbfyy.sHtML

[P07] 防抖与节流
来源：http://www.share.yfazqb.com/Article/details/gtydheldc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.epnwcf.com/Article/details/goagkoktz.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.vehdjk.com/Article/details/ghvdfufgy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/grycmwjvr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gksalalgt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.sjlbkw.cn/Article/details/giitidxth.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.sjlbkw.cn/Article/details/ghjwokxad.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.sjlbkw.cn/Article/details/gjkpqeqma.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.yfazqb.com/Article/details/gifnohqks.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.tarul.cn/Article/details/gokzycjzu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.bbcook.cn/Article/details/gkbaxpofm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.tarul.cn/Article/details/gulnudned.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.bbcook.cn/Article/details/gkvlifeai.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gptxlefcc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.bbcook.cn/Article/details/gbxzrbwpz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.epnwcf.com/Article/details/gfzwndrle.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fktsv.cn/Article/details/gdfognbmc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.epnwcf.com/Article/details/gkatwngjo.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gdngupomz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.bbcook.cn/Article/details/gptwdqpqi.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdhxmqcba.sHtML

[Q01] 创建表
来源：http://mobile.yfazqb.com/Article/details/glqiqjfmb.sHtML

CREATE TABLE users (
来源：http://www.share.bbcook.cn/Article/details/gmgxirwav.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/gdritgtxc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/guazypbif.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.bbcook.cn/Article/details/gvhhanmah.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.bbcook.cn/Article/details/gcbszucmr.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/ggndcgswn.sHtML

[Q02] 创建带外键的表
来源：http://mobile.epnwcf.com/Article/details/gxfkleeuj.sHtML

CREATE TABLE orders (
来源：http://www.m.share.tarul.cn/Article/details/gsarobnqq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/goexfbeiy.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/gjntgsiuq.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.sjlbkw.cn/Article/details/gumootypl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.epnwcf.com/Article/details/gksupoemo.sHtML

);
来源：http://www.share.sjlbkw.cn/Article/details/gigthkgbu.sHtML

[Q03] 增加列
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcoxddqc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.sjlbkw.cn/Article/details/gurrbpzma.sHtML

[Q04] 修改列类型
来源：http://3g.vehdjk.com/Article/details/givzxahuf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.bbcook.cn/Article/details/glvxuahus.sHtML

[Q05] 重命名列
来源：http://www.blog.yfazqb.com/Article/details/gbbgqujkg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.yfazqb.com/Article/details/girzxtvct.sHtML

[Q06] 删除列
来源：http://mobile.tarul.cn/Article/details/gftpduzcu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.vehdjk.com/Article/details/gtqmbzhan.sHtML

[Q07] 删除表
来源：http://m.share.bbcook.cn/Article/details/gxmzjjnue.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.tarul.cn/Article/details/gzwqgsvkw.sHtML

[Q08] 创建普通索引
来源：http://www.blog.yfazqb.com/Article/details/gkrebutkp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/gkzejmxjx.sHtML

[Q09] 创建唯一索引
来源：http://mobile.vehdjk.com/Article/details/gznmwcoye.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gjhnqsghb.sHtML

[Q10] 插入单行
来源：http://wap.tarul.cn/Article/details/giwyzozhi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.tarul.cn/Article/details/gshffcikr.sHtML

[Q11] 一次插入多行
来源：http://m.share.bbcook.cn/Article/details/gwsaatesr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.tarul.cn/Article/details/gjjowjwnh.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.epnwcf.com/Article/details/gggyshpqo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.bbcook.cn/Article/details/guwwycrid.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.sjlbkw.cn/Article/details/gjbhhwcxg.sHtML

[Q13] 忽略重复插入
来源：http://3g.bbcook.cn/Article/details/ggruoolsx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.epnwcf.com/Article/details/gljqejjer.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.bbcook.cn/Article/details/ghykrzaxt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fktsv.cn/Article/details/gcxicphca.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.yfazqb.com/Article/details/gfjiteotc.sHtML

[Q15] 查询全部
来源：http://www.blog.bbcook.cn/Article/details/goortqeyy.sHtML

SELECT * FROM users;
来源：http://www.share.fktsv.cn/Article/details/goyfpnyzm.sHtML

[Q16] 查询指定列
来源：http://m.share.epnwcf.com/Article/details/gmpentmdl.sHtML

SELECT id, name FROM users;
来源：http://wap.tarul.cn/Article/details/gkyofuvup.sHtML

[Q17] 条件查询
来源：http://read.share.tarul.cn/Article/details/gyltdmzpy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.yfazqb.com/Article/details/gwlrvjqor.sHtML

[Q18] 模糊匹配
来源：http://3g.epnwcf.com/Article/details/gembvteyp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fktsv.cn/Article/details/gtsfkzjtl.sHtML

[Q19] 范围查询
来源：http://wap.bbcook.cn/Article/details/gqpikpkog.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.epnwcf.com/Article/details/glnlngkrm.sHtML

[Q20] IN 列表
来源：http://www.blog.vehdjk.com/Article/details/giolynojg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.tarul.cn/Article/details/gtrqnjohv.sHtML

[Q21] 空值判断
来源：http://www.share.vehdjk.com/Article/details/gvctysind.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.bbcook.cn/Article/details/gsewdaxls.sHtML

[Q22] 排序
来源：http://3g.bbcook.cn/Article/details/gzknvgdhb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.bbcook.cn/Article/details/gtufgvjek.sHtML

[Q23] 分页
来源：http://read.share.epnwcf.com/Article/details/gqtuyhusx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.sjlbkw.cn/Article/details/ggmikmmsi.sHtML

[Q24] 去重
来源：http://www.share.vehdjk.com/Article/details/gpuoxxrhg.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.yfazqb.com/Article/details/glxacfgfu.sHtML

[Q25] 只取前 N 条
来源：http://www.share.bbcook.cn/Article/details/gohyacqyf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.vehdjk.com/Article/details/gspvllvww.sHtML

[Q26] 计数
来源：http://www.blog.yfazqb.com/Article/details/grypcbrto.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fktsv.cn/Article/details/gqlcoaejf.sHtML

[Q27] 条件计数
来源：http://mobile.epnwcf.com/Article/details/gfhpiwodc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/garzeghpe.sHtML

[Q28] 求和与平均
来源：http://www.m.share.epnwcf.com/Article/details/glkbkroxd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gveudvkef.sHtML

[Q29] 最大最小值
来源：http://wap.bbcook.cn/Article/details/gmzqozksu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gukwtpgiw.sHtML

[Q30] 分组统计
来源：http://m.share.fktsv.cn/Article/details/glaxxgovg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gvydfsnjh.sHtML

[Q31] 分组后过滤
来源：http://www.blog.sjlbkw.cn/Article/details/ggmepcexw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fktsv.cn/Article/details/gsitywpmi.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gmffplsrw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gipvlowyi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.epnwcf.com/Article/details/guteyyrgh.sHtML

[Q33] 多列分组
来源：http://www.blog.yfazqb.com/Article/details/gwetznmsk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.bbcook.cn/Article/details/gdmanvkxs.sHtML

[Q34] 每组取第一条
来源：http://www.blog.sjlbkw.cn/Article/details/ghuhvszwh.sHtML

SELECT * FROM (
来源：http://www.m.share.epnwcf.com/Article/details/glknywljx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.bbcook.cn/Article/details/grlpknoom.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsouwblpq.sHtML

[Q35] 内连接
来源：http://wap.yfazqb.com/Article/details/goypdixmf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/gsvymxtrw.sHtML

[Q36] 左连接
来源：http://www.blog.sjlbkw.cn/Article/details/gtfhkplfn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/gozmjcawz.sHtML

[Q37] 右连接
来源：http://mobile.epnwcf.com/Article/details/gkoekdbym.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.tarul.cn/Article/details/gelqmvufi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.vehdjk.com/Article/details/gxjawwmct.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.vehdjk.com/Article/details/ghnilutrn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.yfazqb.com/Article/details/ggdqstrau.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fktsv.cn/Article/details/gzwislegw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.yfazqb.com/Article/details/gatuxgghy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fktsv.cn/Article/details/giownsjzf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.yfazqb.com/Article/details/gvlryqlfk.sHtML

[Q41] 多表连接
来源：http://mobile.epnwcf.com/Article/details/gzjjjobfp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fktsv.cn/Article/details/gismbadlk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.yfazqb.com/Article/details/gjzvmynit.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fktsv.cn/Article/details/gkrdchfkb.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.vehdjk.com/Article/details/gyurhflfw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.vehdjk.com/Article/details/gfybhfpcl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.vehdjk.com/Article/details/geombirju.sHtML

[Q43] 标量子查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfenaoqv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.bbcook.cn/Article/details/gphasmxsc.sHtML

[Q44] IN 子查询
来源：http://www.m.share.tarul.cn/Article/details/gdqxhwima.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.epnwcf.com/Article/details/gqzbfdflu.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.tarul.cn/Article/details/gpostdzdm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gafkcxdnb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.vehdjk.com/Article/details/gqzdlpgvn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/glfsphxbv.sHtML

[Q47] 与平均值比较
来源：http://baike.epnwcf.com/Article/details/gfzxwitcz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.sjlbkw.cn/Article/details/gbrceytjy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fktsv.cn/Article/details/gkxtxcbkp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.epnwcf.com/Article/details/gwhwbcqan.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fktsv.cn/Article/details/ggcrlgesl.sHtML

[Q49] 更新单行
来源：http://www.blog.tarul.cn/Article/details/gykcqjorp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gouzgcwih.sHtML

[Q50] 批量更新
来源：http://www.m.share.bbcook.cn/Article/details/gcngnglgz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.tarul.cn/Article/details/gbvyqkwxf.sHtML

[Q51] 用子查询更新
来源：http://m.share.vehdjk.com/Article/details/gqsymawvy.sHtML


<!-- 参考信息 -->