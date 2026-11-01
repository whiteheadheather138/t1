代发 wailian999

Go:   // 手写 map[int]int
来源：http://read.share.tarul.cn/Article/details/gclyogygg.sHtML

Ruby: // 手写 Hash
来源：http://www.share.bbcook.cn/Article/details/giyrzmdne.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.vehdjk.com/Article/details/gyretiqiy.sHtML

[N08] 生成全排列
来源：http://m.share.sjlbkw.cn/Article/details/gfagmaicj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gnubhzlag.sHtML

PHP:  // 手写递归交换
来源：http://mobile.vehdjk.com/Article/details/gbqtmnysj.sHtML

JS:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gactqkxff.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gijwatrhk.sHtML

Java: // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gcfwdddfz.sHtML

Go:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gwsxhltvd.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.bbcook.cn/Article/details/gvpgqwixk.sHtML

C#:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/ghsrjioia.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/gcxkhoydy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.yfazqb.com/Article/details/gogeoqheo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gxnxzubrg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gukrdgqge.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.sjlbkw.cn/Article/details/gzwklljou.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.bbcook.cn/Article/details/gswrfnlfy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.yfazqb.com/Article/details/gmyhcanvx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gnkqcdsqa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.yfazqb.com/Article/details/gmbyfjpcm.sHtML

[N10] 链表节点定义
来源：http://www.blog.vehdjk.com/Article/details/gyhfuqmop.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.tarul.cn/Article/details/gpjlciddc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fktsv.cn/Article/details/glylpxllc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.epnwcf.com/Article/details/gtuoaiuaq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.tarul.cn/Article/details/gwoewrlfj.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/gzgqiwofp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/glvspoixx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.yfazqb.com/Article/details/gmufzcryz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.bbcook.cn/Article/details/gpmziptyv.sHtML

[N11] 二叉树中序遍历
来源：http://3g.sjlbkw.cn/Article/details/gjvmsesxj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/ganlfkyvy.sHtML

PHP:  // 手写递归函数
来源：http://mobile.tarul.cn/Article/details/gzhwsbpjq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gkqdsyeep.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/glvyfaecf.sHtML

Java: // 手写递归
来源：http://wap.yfazqb.com/Article/details/gxfzwjtgf.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gmjwynzlj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.tarul.cn/Article/details/ggumxnzvq.sHtML

C#:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gretotkwl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gbehmlsmn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fktsv.cn/Article/details/ghupgryrk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.sjlbkw.cn/Article/details/grpayigpa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gvrjibael.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.bbcook.cn/Article/details/gtfvaenic.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/giasxhdyb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.bbcook.cn/Article/details/gpztcedhv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.epnwcf.com/Article/details/gpohoieeg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/gvqyefyos.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkijgfyqh.sHtML

O. 并发与异步
来源：http://read.share.fktsv.cn/Article/details/gqvehykyr.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gbwalaguv.sHtML

[O01] 启动一个线程
来源：http://m.share.bbcook.cn/Article/details/gralawrfs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.epnwcf.com/Article/details/gjxwujxmw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.epnwcf.com/Article/details/gwkccojzs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gyrjwobnl.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/gkxjrrlsl.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.sjlbkw.cn/Article/details/gqsvlotth.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/gratiunil.sHtML

Ruby: Thread.new { f }
来源：http://blog.epnwcf.com/Article/details/gasmdtzmo.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.bbcook.cn/Article/details/gzdahurxl.sHtML

[O02] 使用线程池
来源：http://blog.yfazqb.com/Article/details/gonpmcbou.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.bbcook.cn/Article/details/gxmkungac.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.vehdjk.com/Article/details/ghgnnlacm.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gsqxhugjb.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gjyvazymp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.sjlbkw.cn/Article/details/gpfvdgafx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/grzfduqow.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.vehdjk.com/Article/details/ggkauevrx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.yfazqb.com/Article/details/gnblzhasv.sHtML

[O03] 加锁保护共享数据
来源：http://baike.yfazqb.com/Article/details/ghvglprip.sHtML

Py:   with lock: shared += 1
来源：http://baike.epnwcf.com/Article/details/gnkyudlnr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.sjlbkw.cn/Article/details/gfiyppjin.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.bbcook.cn/Article/details/gkqthsnow.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/gtqeznzlf.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.vehdjk.com/Article/details/grvsrypdv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.epnwcf.com/Article/details/gffpnbnoq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gvvlkdoqg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.vehdjk.com/Article/details/gszfbpmpe.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fktsv.cn/Article/details/ghfkcjkag.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.sjlbkw.cn/Article/details/gxhuzahem.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.sjlbkw.cn/Article/details/gcykwjagu.sHtML

JS:   async function f() { await g(); }
来源：http://blog.vehdjk.com/Article/details/grgfobaho.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/gwbtplccc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.yfazqb.com/Article/details/gpsxyxclj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.sjlbkw.cn/Article/details/ggpffowoc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.tarul.cn/Article/details/gppoqjptl.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/gtvlzhpyw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.yfazqb.com/Article/details/gqmffojph.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.vehdjk.com/Article/details/gctpymamw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.epnwcf.com/Article/details/gwygovxke.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/glwznblfz.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gkmydmemi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.tarul.cn/Article/details/gblhdeehz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.vehdjk.com/Article/details/gffbscrhg.sHtML

Ruby: threads.map(&:join)
来源：http://3g.yfazqb.com/Article/details/gfbvlpeab.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fktsv.cn/Article/details/gmiyapvsi.sHtML

[O06] 使用进程池
来源：http://read.share.yfazqb.com/Article/details/gtuwdpcgj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.tarul.cn/Article/details/guvmgxtos.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fktsv.cn/Article/details/grehicbzg.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/grcxvqvdc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gemjysmaj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.yfazqb.com/Article/details/glsjaptzx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.tarul.cn/Article/details/grlbexttp.sHtML

Ruby: // fork 块
来源：http://mobile.fktsv.cn/Article/details/gkmoildyn.sHtML

C#:   Parallel.For
来源：http://m.share.epnwcf.com/Article/details/gzsyqsluu.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gjjfrebcz.sHtML

P. 常用工具函数
来源：http://3g.tarul.cn/Article/details/gauxkomeg.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gdonztgfv.sHtML

[P01] 生成 UUID
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmrxxzee.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.bbcook.cn/Article/details/grrkcmyqj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/gghqtlkse.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gkqwsxrdm.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gjfhljtqu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.tarul.cn/Article/details/gisvzatlf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.yfazqb.com/Article/details/gpdpctwzw.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.yfazqb.com/Article/details/gqxqwdebz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.bbcook.cn/Article/details/gbnaxvmrb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.vehdjk.com/Article/details/geerpfcqv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.epnwcf.com/Article/details/gnkfmbuwl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.yfazqb.com/Article/details/gstuahtyz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfriwgxu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.bbcook.cn/Article/details/gqcquexvg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.bbcook.cn/Article/details/gsojemoie.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.bbcook.cn/Article/details/gglmgxhbs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.vehdjk.com/Article/details/geafaxbgg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgbnesei.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fktsv.cn/Article/details/gvytbkecb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fktsv.cn/Article/details/gkgwvxsiv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.epnwcf.com/Article/details/ggzdgzzgq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.tarul.cn/Article/details/gshigzxvj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gfbdakhou.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.tarul.cn/Article/details/gyfabvovo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/gtmiqvtxk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.vehdjk.com/Article/details/gwwaclboa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.tarul.cn/Article/details/guzlaloda.sHtML

[P04] 求长度
来源：http://m.share.epnwcf.com/Article/details/grtqmhpub.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.tarul.cn/Article/details/guogxtpvq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gqjrlfvsg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/glcfovwhz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gyivmnerk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.tarul.cn/Article/details/gptjoajid.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.vehdjk.com/Article/details/gfwkcprks.sHtML

Ruby: x.length;  x.size
来源：http://wap.sjlbkw.cn/Article/details/gbwyimsbt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.vehdjk.com/Article/details/gvhkxqwlr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.sjlbkw.cn/Article/details/gqxbktqgw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fktsv.cn/Article/details/gggxtxtzu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.bbcook.cn/Article/details/gdkegyfgb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.bbcook.cn/Article/details/gqvbtppaj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.epnwcf.com/Article/details/goxreqild.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.sjlbkw.cn/Article/details/gfvsnfxhu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.bbcook.cn/Article/details/gcximxhzg.sHtML

Ruby: a == b
来源：http://m.share.yfazqb.com/Article/details/gxriemmmp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.epnwcf.com/Article/details/gqftvmqig.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.vehdjk.com/Article/details/gwzsgkblk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.vehdjk.com/Article/details/gwfswkhaj.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.yfazqb.com/Article/details/gwcgzsmdc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.sjlbkw.cn/Article/details/gmlviyysb.sHtML

TS:   if (x == null) {}
来源：http://mobile.yfazqb.com/Article/details/gjrwubiqh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/gcrlxyzeb.sHtML

Go:   if x == nil {}
来源：http://read.share.tarul.cn/Article/details/gqdxcwbxz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.vehdjk.com/Article/details/ggecnisre.sHtML

C#:   if (x is null) {}
来源：http://mobile.vehdjk.com/Article/details/gbtjfwxvz.sHtML

[P07] 防抖与节流
来源：http://blog.tarul.cn/Article/details/gextrwlfo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fktsv.cn/Article/details/gpwemddxy.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.sjlbkw.cn/Article/details/gugjzabzg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gpietjmwt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gindvtroh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/gcvyofkho.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fktsv.cn/Article/details/gefbnxohq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.bbcook.cn/Article/details/gyigozbtw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.vehdjk.com/Article/details/gpfohqpiv.sHtML

[P08] 处理浮点精度问题
来源：http://3g.yfazqb.com/Article/details/ggwfvbjtz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.bbcook.cn/Article/details/girqeeijc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fktsv.cn/Article/details/gfbssllti.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.bbcook.cn/Article/details/glxwvemgz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/gajhxfwpp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.bbcook.cn/Article/details/gcflazwho.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.yfazqb.com/Article/details/gbsrzsegj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.tarul.cn/Article/details/gjsunotlo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.tarul.cn/Article/details/gcmaqncbm.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gnobnuyge.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fktsv.cn/Article/details/gujzowpei.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gcvfpobbu.sHtML

[Q01] 创建表
来源：http://baike.fktsv.cn/Article/details/giwmtbotp.sHtML

CREATE TABLE users (
来源：http://www.blog.fktsv.cn/Article/details/ghyaocbew.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gjxjcscul.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/gudkgzcth.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fktsv.cn/Article/details/gpodqclor.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.tarul.cn/Article/details/gvxofzgpc.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gdeoetrte.sHtML

[Q02] 创建带外键的表
来源：http://www.share.tarul.cn/Article/details/genwaffwj.sHtML

CREATE TABLE orders (
来源：http://mobile.fktsv.cn/Article/details/gozvwsldx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fktsv.cn/Article/details/gfqqifelh.sHtML

user_id INT NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/gfpyzrkfp.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.vehdjk.com/Article/details/gkmfwazmj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.tarul.cn/Article/details/gqoiegagx.sHtML

);
来源：http://baike.epnwcf.com/Article/details/gnrqjocff.sHtML

[Q03] 增加列
来源：http://m.share.tarul.cn/Article/details/gdhnmhund.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.bbcook.cn/Article/details/ggrzlmouk.sHtML

[Q04] 修改列类型
来源：http://m.share.sjlbkw.cn/Article/details/gybyqnncf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.vehdjk.com/Article/details/gzlhewlmy.sHtML

[Q05] 重命名列
来源：http://baike.sjlbkw.cn/Article/details/grpdhzqwa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.vehdjk.com/Article/details/gvjzkhpmf.sHtML

[Q06] 删除列
来源：http://www.m.share.vehdjk.com/Article/details/gzwzlzxmt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.tarul.cn/Article/details/gjlwalclq.sHtML

[Q07] 删除表
来源：http://www.share.epnwcf.com/Article/details/gcfvhaezr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.epnwcf.com/Article/details/gbojiwvbj.sHtML

[Q08] 创建普通索引
来源：http://baike.vehdjk.com/Article/details/gsvtxfzwo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.epnwcf.com/Article/details/gspqsqbic.sHtML

[Q09] 创建唯一索引
来源：http://m.share.yfazqb.com/Article/details/glsieikfe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.bbcook.cn/Article/details/gwxqtkujo.sHtML

[Q10] 插入单行
来源：http://3g.fktsv.cn/Article/details/gosrghojm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fktsv.cn/Article/details/ggbxhdjcw.sHtML

[Q11] 一次插入多行
来源：http://m.share.fktsv.cn/Article/details/gkoqvrwpr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gbjeahotp.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.epnwcf.com/Article/details/gjhygqnak.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.tarul.cn/Article/details/gtcdjhyee.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fktsv.cn/Article/details/gzeealooq.sHtML

[Q13] 忽略重复插入
来源：http://baike.fktsv.cn/Article/details/gkheuccql.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.tarul.cn/Article/details/gpjghmeup.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxhotxmc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.sjlbkw.cn/Article/details/gblhbthxw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fktsv.cn/Article/details/giyvuwnzn.sHtML

[Q15] 查询全部
来源：http://read.share.sjlbkw.cn/Article/details/gkymccerx.sHtML

SELECT * FROM users;
来源：http://mobile.fktsv.cn/Article/details/gfyvvvboi.sHtML

[Q16] 查询指定列
来源：http://baike.yfazqb.com/Article/details/glfxeglnx.sHtML

SELECT id, name FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gyipmhldp.sHtML

[Q17] 条件查询
来源：http://blog.vehdjk.com/Article/details/ghbywipfh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.vehdjk.com/Article/details/gmprwxivu.sHtML

[Q18] 模糊匹配
来源：http://baike.tarul.cn/Article/details/gbwaxvodb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.sjlbkw.cn/Article/details/gjfnywnxo.sHtML

[Q19] 范围查询
来源：http://blog.bbcook.cn/Article/details/gtaplbmpo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.sjlbkw.cn/Article/details/gaxuomvfx.sHtML

[Q20] IN 列表
来源：http://www.blog.epnwcf.com/Article/details/gyngezvlq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.bbcook.cn/Article/details/goalwknsm.sHtML

[Q21] 空值判断
来源：http://m.share.tarul.cn/Article/details/girpduqry.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.epnwcf.com/Article/details/gkaoffqqz.sHtML

[Q22] 排序
来源：http://wap.yfazqb.com/Article/details/gdrpsniac.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.yfazqb.com/Article/details/ggdicfchp.sHtML

[Q23] 分页
来源：http://blog.sjlbkw.cn/Article/details/ghchvnpor.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.vehdjk.com/Article/details/ghyoeuyee.sHtML

[Q24] 去重
来源：http://www.m.share.tarul.cn/Article/details/gyjuedwgz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/guucrkatr.sHtML

[Q25] 只取前 N 条
来源：http://3g.bbcook.cn/Article/details/ghwanqlcz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.yfazqb.com/Article/details/gxtfuwhek.sHtML

[Q26] 计数
来源：http://www.blog.sjlbkw.cn/Article/details/gnqifzsnf.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.epnwcf.com/Article/details/glsmnpuij.sHtML

[Q27] 条件计数
来源：http://wap.sjlbkw.cn/Article/details/gqivftcwd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.bbcook.cn/Article/details/grsmddyqi.sHtML

[Q28] 求和与平均
来源：http://m.share.fktsv.cn/Article/details/gcvzwudkq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/ghmfrzpmx.sHtML

[Q29] 最大最小值
来源：http://baike.epnwcf.com/Article/details/gjoxzzlul.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.tarul.cn/Article/details/gvegvonay.sHtML

[Q30] 分组统计
来源：http://blog.bbcook.cn/Article/details/gecwevfat.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/glubwwaig.sHtML

[Q31] 分组后过滤
来源：http://read.share.tarul.cn/Article/details/gqoarouem.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.yfazqb.com/Article/details/gbchxdkou.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gswuujvqg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gwvglduxn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.epnwcf.com/Article/details/gsrnjyqgx.sHtML

[Q33] 多列分组
来源：http://3g.fktsv.cn/Article/details/gcolemrrt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.sjlbkw.cn/Article/details/gdmfztham.sHtML

[Q34] 每组取第一条
来源：http://wap.fktsv.cn/Article/details/gemokjsed.sHtML

SELECT * FROM (
来源：http://read.share.bbcook.cn/Article/details/gqmbjrrxo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.bbcook.cn/Article/details/gyxpgbnfj.sHtML

) t WHERE rn = 1;
来源：http://baike.fktsv.cn/Article/details/ghialxucg.sHtML

[Q35] 内连接
来源：http://www.blog.yfazqb.com/Article/details/ggpuveunj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gzyxsvxsc.sHtML

[Q36] 左连接
来源：http://mobile.fktsv.cn/Article/details/gyddylioc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/gdofoubsc.sHtML

[Q37] 右连接
来源：http://baike.vehdjk.com/Article/details/gnstyvcoc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.yfazqb.com/Article/details/giypqxles.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.epnwcf.com/Article/details/gggqoemwp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.bbcook.cn/Article/details/gfviloadt.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.epnwcf.com/Article/details/gnmomifev.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.bbcook.cn/Article/details/gcjtbmcwi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.yfazqb.com/Article/details/gqlbkuple.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.epnwcf.com/Article/details/gdbnpqqpm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.yfazqb.com/Article/details/gedzhghxs.sHtML

[Q41] 多表连接
来源：http://wap.tarul.cn/Article/details/gguctmnil.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.bbcook.cn/Article/details/gvtpsnnkf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.epnwcf.com/Article/details/gjmbkoxfb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.yfazqb.com/Article/details/gcnfrxjkw.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.epnwcf.com/Article/details/gmaazvria.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.vehdjk.com/Article/details/gskhyiqpg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.tarul.cn/Article/details/gawvkbrnr.sHtML

[Q43] 标量子查询
来源：http://mobile.bbcook.cn/Article/details/gadafsuzq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fktsv.cn/Article/details/gpexnwnhw.sHtML

[Q44] IN 子查询
来源：http://wap.tarul.cn/Article/details/gfumgpcja.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.vehdjk.com/Article/details/gtnqddyxe.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/gxmsyxojp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gxxmfyuht.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.yfazqb.com/Article/details/ggkipkcjl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.vehdjk.com/Article/details/gkmqxghng.sHtML

[Q47] 与平均值比较
来源：http://www.share.tarul.cn/Article/details/gyytporok.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.bbcook.cn/Article/details/gmywslpde.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.sjlbkw.cn/Article/details/gbemmvajf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.epnwcf.com/Article/details/gvuxmraln.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.epnwcf.com/Article/details/gdecbmybv.sHtML

[Q49] 更新单行
来源：http://www.blog.yfazqb.com/Article/details/gzvhejgse.sHtML


<!-- 参考信息 -->