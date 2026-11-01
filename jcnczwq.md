代发 wailian999

Java: // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gmsxyhpnv.sHtML

Go:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gzbqwhkgm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.tarul.cn/Article/details/gkiuquxsj.sHtML

C#:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/ggtzeksgq.sHtML

[N09] 栈与队列
来源：http://read.share.bbcook.cn/Article/details/guoxdcaie.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.epnwcf.com/Article/details/gzpynszqw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.tarul.cn/Article/details/guxdilysn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/ghoexodgx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/guxfjokwe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/givyfablx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fktsv.cn/Article/details/gnbachwvv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gnzanbclv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.yfazqb.com/Article/details/gwpyifjow.sHtML

[N10] 链表节点定义
来源：http://m.share.tarul.cn/Article/details/ghkjzhawy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.yfazqb.com/Article/details/gswovdwdm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.tarul.cn/Article/details/glxkuqobj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.sjlbkw.cn/Article/details/gqbgfbjhv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.yfazqb.com/Article/details/gwvxqbwwa.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fktsv.cn/Article/details/ggrhhgjwp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.sjlbkw.cn/Article/details/gpthalghw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.yfazqb.com/Article/details/giirtaqrx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.tarul.cn/Article/details/gsermxiey.sHtML

[N11] 二叉树中序遍历
来源：http://blog.bbcook.cn/Article/details/gzobzbukb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.tarul.cn/Article/details/glexliunq.sHtML

PHP:  // 手写递归函数
来源：http://blog.yfazqb.com/Article/details/gxxihjiqn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/ghbxblhzr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.tarul.cn/Article/details/gnevpwesa.sHtML

Java: // 手写递归
来源：http://blog.bbcook.cn/Article/details/gnneoarfg.sHtML

Go:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gwrmfsirl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.sjlbkw.cn/Article/details/gsfllxszm.sHtML

C#:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gvpdpejvf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.yfazqb.com/Article/details/guucxdglj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.vehdjk.com/Article/details/glndewdzq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fktsv.cn/Article/details/gfkiiuppo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gdudvquro.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gjzlfmlaq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gziezqgdw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.vehdjk.com/Article/details/gqsjufprc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fktsv.cn/Article/details/gymaxdlxh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.epnwcf.com/Article/details/gvswxrlhy.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gbfmemljs.sHtML

O. 并发与异步
来源：http://www.share.sjlbkw.cn/Article/details/gvhiivtxp.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gpnrfprve.sHtML

[O01] 启动一个线程
来源：http://blog.fktsv.cn/Article/details/gezwovioj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.yfazqb.com/Article/details/gobsaqrdt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.sjlbkw.cn/Article/details/gapnxesgv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.epnwcf.com/Article/details/gtedijeqk.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gbbzcylfj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fktsv.cn/Article/details/gagtcieec.sHtML

Go:   go f()
来源：http://3g.yfazqb.com/Article/details/gxtlwdqro.sHtML

Ruby: Thread.new { f }
来源：http://www.share.sjlbkw.cn/Article/details/gcjgilhvt.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.bbcook.cn/Article/details/gqjczasdf.sHtML

[O02] 使用线程池
来源：http://m.share.sjlbkw.cn/Article/details/gbngltcco.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.bbcook.cn/Article/details/gkmyeavug.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.vehdjk.com/Article/details/gxqedwbaj.sHtML

JS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gpakpvtfg.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/ggyuesaru.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.bbcook.cn/Article/details/gowngmwoo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/gibvhdtxo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.tarul.cn/Article/details/ghqmqzylf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.yfazqb.com/Article/details/gnwtqbvms.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxhxucks.sHtML

Py:   with lock: shared += 1
来源：http://3g.tarul.cn/Article/details/gtbnjmnvw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.tarul.cn/Article/details/gdkxjhfan.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.yfazqb.com/Article/details/ggcspuxiv.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/gzbpuodjh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/ggglthozs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.epnwcf.com/Article/details/gjuegvpem.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.tarul.cn/Article/details/gvmaqndtq.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gfnlivypj.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.yfazqb.com/Article/details/gybeiezpg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.vehdjk.com/Article/details/gxttbevov.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.epnwcf.com/Article/details/gzhjpcthl.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gkmamyhuq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.sjlbkw.cn/Article/details/gxwrxzoqq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/glyzmysor.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.vehdjk.com/Article/details/gcauykzov.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.vehdjk.com/Article/details/gsudhwbri.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/gytejibgr.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.epnwcf.com/Article/details/gfwymurfb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gyntadpqx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.bbcook.cn/Article/details/gjdijfoas.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/gxptecozz.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gpktnjbbk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.sjlbkw.cn/Article/details/gqsmevaer.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.vehdjk.com/Article/details/gemiroihm.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gnobzgpda.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.yfazqb.com/Article/details/gedyklvmn.sHtML

[O06] 使用进程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gcertqfgy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.vehdjk.com/Article/details/gppkdtynl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.epnwcf.com/Article/details/gzcjhkfls.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gasbhmwwp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gasrcrthn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.bbcook.cn/Article/details/gvfbfgnnz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.yfazqb.com/Article/details/gapfgtkud.sHtML

Ruby: // fork 块
来源：http://3g.fktsv.cn/Article/details/gitkuvthg.sHtML

C#:   Parallel.For
来源：http://read.share.bbcook.cn/Article/details/gziovzger.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxaftqfpi.sHtML

P. 常用工具函数
来源：http://3g.epnwcf.com/Article/details/gtyyzlwjt.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gqmnmkdhf.sHtML

[P01] 生成 UUID
来源：http://baike.vehdjk.com/Article/details/ggknftkuk.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.epnwcf.com/Article/details/goawapafq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.tarul.cn/Article/details/grmaemtux.sHtML

JS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gvzlmipgn.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/ggkraffrq.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.tarul.cn/Article/details/ghlxirscb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fktsv.cn/Article/details/gibaevuso.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.sjlbkw.cn/Article/details/gntkusnpq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.yfazqb.com/Article/details/glguqbduu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.sjlbkw.cn/Article/details/gqfsjysnu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.vehdjk.com/Article/details/gzwxzoguy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fktsv.cn/Article/details/gyembdmtm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.tarul.cn/Article/details/garyuopmx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoqorqpu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gjoovfcvg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.tarul.cn/Article/details/ghdbulynt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fktsv.cn/Article/details/gyzqzpart.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.tarul.cn/Article/details/gnjmvxqbw.sHtML

[P03] 生成短随机字符串
来源：http://blog.sjlbkw.cn/Article/details/gvtdxhnyu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.yfazqb.com/Article/details/gfqtmfgng.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.vehdjk.com/Article/details/gtdkeruut.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/ggyvrccka.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gwklxaotg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.tarul.cn/Article/details/gspfxvxmb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/gcsytzbfp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fktsv.cn/Article/details/gewrchiai.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.tarul.cn/Article/details/gggmqbpqi.sHtML

[P04] 求长度
来源：http://m.share.fktsv.cn/Article/details/gmihmwgnb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.epnwcf.com/Article/details/glvshyilv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gwetaonac.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/grifbangp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gkxlfsqbb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.tarul.cn/Article/details/gneakngej.sHtML

Go:   len(arr);  len(m)
来源：http://3g.yfazqb.com/Article/details/gmbvygojd.sHtML

Ruby: x.length;  x.size
来源：http://wap.fktsv.cn/Article/details/gqkfgxzmh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.epnwcf.com/Article/details/gdpdogszz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fktsv.cn/Article/details/gljqhpujp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.bbcook.cn/Article/details/gbrdohyxs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.yfazqb.com/Article/details/gbrqmugxn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.yfazqb.com/Article/details/guuslucbp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.tarul.cn/Article/details/gujkjfyni.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.bbcook.cn/Article/details/glgnzzjtf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gnuolkyig.sHtML

Ruby: a == b
来源：http://www.m.share.yfazqb.com/Article/details/ggusekerp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.sjlbkw.cn/Article/details/gagpwbxat.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.epnwcf.com/Article/details/gmtxdwswk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.vehdjk.com/Article/details/gvzsnzgzk.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.yfazqb.com/Article/details/gxysqcbvz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.epnwcf.com/Article/details/gvejeolst.sHtML

TS:   if (x == null) {}
来源：http://wap.sjlbkw.cn/Article/details/guibwigzx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/gtnuykkrj.sHtML

Go:   if x == nil {}
来源：http://blog.bbcook.cn/Article/details/gxdmdwbhl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.vehdjk.com/Article/details/garwsvayu.sHtML

C#:   if (x is null) {}
来源：http://read.share.epnwcf.com/Article/details/gqqlcwwbx.sHtML

[P07] 防抖与节流
来源：http://mobile.tarul.cn/Article/details/givrjggjo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.yfazqb.com/Article/details/gsumzvjxm.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.sjlbkw.cn/Article/details/ggvokiwpd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/grdgaqnul.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/grapmlwds.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.sjlbkw.cn/Article/details/grgtvevbo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.yfazqb.com/Article/details/gytbxhikn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gxeplgvna.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.vehdjk.com/Article/details/gyahcdfyk.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fktsv.cn/Article/details/gcwxfurir.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.yfazqb.com/Article/details/gtljuarwc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.epnwcf.com/Article/details/glbrsypmq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fktsv.cn/Article/details/gcfarrder.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.tarul.cn/Article/details/ghotcmpzl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.tarul.cn/Article/details/gdimxnbem.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.tarul.cn/Article/details/gxlqpurxo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fktsv.cn/Article/details/ggmsqwiuh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.tarul.cn/Article/details/gecvpvnts.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gsbgonrfl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fktsv.cn/Article/details/gqspagpxp.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gxixyfklh.sHtML

[Q01] 创建表
来源：http://wap.epnwcf.com/Article/details/gxrlfdthx.sHtML

CREATE TABLE users (
来源：http://blog.yfazqb.com/Article/details/gdlmmhrgl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gyqsuurng.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gqounmhxb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhhmshvl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fktsv.cn/Article/details/gmovzovdg.sHtML

);
来源：http://baike.vehdjk.com/Article/details/gikzgkxgt.sHtML

[Q02] 创建带外键的表
来源：http://read.share.bbcook.cn/Article/details/ghwrbacgh.sHtML

CREATE TABLE orders (
来源：http://read.share.yfazqb.com/Article/details/gjcqmajba.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gprphsycs.sHtML

user_id INT NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/gvxdpmsnc.sHtML

amount DECIMAL(10, 2),
来源：http://blog.sjlbkw.cn/Article/details/galdoctlj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.yfazqb.com/Article/details/ghzkqcktq.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gapoqvuhw.sHtML

[Q03] 增加列
来源：http://mobile.tarul.cn/Article/details/gowpibdqe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.tarul.cn/Article/details/gndqcuxfu.sHtML

[Q04] 修改列类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gtonltzrz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.yfazqb.com/Article/details/gwvurodpn.sHtML

[Q05] 重命名列
来源：http://mobile.epnwcf.com/Article/details/gihjkqwzk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.bbcook.cn/Article/details/gagrxpuvr.sHtML

[Q06] 删除列
来源：http://wap.fktsv.cn/Article/details/glngudiie.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fktsv.cn/Article/details/gdvpfzpit.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/gqkuhoyry.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.yfazqb.com/Article/details/gnyfuhdkm.sHtML

[Q08] 创建普通索引
来源：http://read.share.yfazqb.com/Article/details/gjekqpruz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gocurezds.sHtML

[Q09] 创建唯一索引
来源：http://read.share.yfazqb.com/Article/details/ghvcpzvjl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/gjdavjyyx.sHtML

[Q10] 插入单行
来源：http://www.m.share.fktsv.cn/Article/details/gecbluzcv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gtnqzgjvq.sHtML

[Q11] 一次插入多行
来源：http://baike.yfazqb.com/Article/details/gvjyaczns.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.vehdjk.com/Article/details/gshwjhcjt.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.yfazqb.com/Article/details/gpnngnhik.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.tarul.cn/Article/details/gebadmuwc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.yfazqb.com/Article/details/ggptgzrix.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.yfazqb.com/Article/details/gepudnrbg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.epnwcf.com/Article/details/gximqkxcu.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.bbcook.cn/Article/details/gbrdnuhpg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fktsv.cn/Article/details/ghvjdasfe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.bbcook.cn/Article/details/gomhzbgam.sHtML

[Q15] 查询全部
来源：http://read.share.bbcook.cn/Article/details/gjnhmyocj.sHtML

SELECT * FROM users;
来源：http://read.share.bbcook.cn/Article/details/gwbhfqwam.sHtML

[Q16] 查询指定列
来源：http://m.share.vehdjk.com/Article/details/gutfmquty.sHtML

SELECT id, name FROM users;
来源：http://3g.sjlbkw.cn/Article/details/grqyprbxh.sHtML

[Q17] 条件查询
来源：http://www.blog.tarul.cn/Article/details/gdnuvkdjd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.vehdjk.com/Article/details/gfujhtrrs.sHtML

[Q18] 模糊匹配
来源：http://wap.tarul.cn/Article/details/gdfwkmigx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.epnwcf.com/Article/details/gbvpfekgx.sHtML

[Q19] 范围查询
来源：http://wap.sjlbkw.cn/Article/details/gaznviopn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.sjlbkw.cn/Article/details/gdzrkdhjf.sHtML

[Q20] IN 列表
来源：http://m.share.yfazqb.com/Article/details/gsnpfvjbv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.sjlbkw.cn/Article/details/ggnfpanfi.sHtML

[Q21] 空值判断
来源：http://www.blog.tarul.cn/Article/details/gntnaqmjc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.tarul.cn/Article/details/gmggaiwas.sHtML

[Q22] 排序
来源：http://blog.bbcook.cn/Article/details/gkmzmwpyl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.bbcook.cn/Article/details/gpovsfwzd.sHtML

[Q23] 分页
来源：http://mobile.vehdjk.com/Article/details/glhqhubku.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.yfazqb.com/Article/details/gzwscutab.sHtML

[Q24] 去重
来源：http://www.share.fktsv.cn/Article/details/goygfpyyq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.tarul.cn/Article/details/ggfgwdejm.sHtML

[Q25] 只取前 N 条
来源：http://wap.tarul.cn/Article/details/gtgjlijrx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.yfazqb.com/Article/details/gbyztmybs.sHtML

[Q26] 计数
来源：http://baike.yfazqb.com/Article/details/gpvtaesyw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gwzeoujau.sHtML

[Q27] 条件计数
来源：http://m.share.tarul.cn/Article/details/gajvipcbd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.epnwcf.com/Article/details/gbogxggyq.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fktsv.cn/Article/details/gkjvicarf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gagoakhnh.sHtML

[Q29] 最大最小值
来源：http://www.share.epnwcf.com/Article/details/gasllefda.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gltldsxyz.sHtML

[Q30] 分组统计
来源：http://m.share.bbcook.cn/Article/details/grdjpkvpm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gjdfyxtyr.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/ghrwswuxt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fktsv.cn/Article/details/gbtvtigph.sHtML

[Q32] 分组拼接字符串
来源：http://wap.tarul.cn/Article/details/gfdgkpijj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gykplrtiq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fktsv.cn/Article/details/gpprxtmnx.sHtML

[Q33] 多列分组
来源：http://blog.sjlbkw.cn/Article/details/guqntrygw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.bbcook.cn/Article/details/gclsccdjf.sHtML

[Q34] 每组取第一条
来源：http://read.share.bbcook.cn/Article/details/gofqqszwn.sHtML

SELECT * FROM (
来源：http://wap.tarul.cn/Article/details/gwdahtdwv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.tarul.cn/Article/details/gwhnvazbz.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gizadlacy.sHtML

[Q35] 内连接
来源：http://baike.yfazqb.com/Article/details/gfcmslsdp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/guvrexrtr.sHtML

[Q36] 左连接
来源：http://mobile.bbcook.cn/Article/details/gkabdfrey.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gnqifidwt.sHtML

[Q37] 右连接
来源：http://wap.vehdjk.com/Article/details/gyfycsjix.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.yfazqb.com/Article/details/gfaerehsn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fktsv.cn/Article/details/gplwcbfzw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.epnwcf.com/Article/details/grhmirzws.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.tarul.cn/Article/details/glzzsgurw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.yfazqb.com/Article/details/giqkhqnio.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.bbcook.cn/Article/details/gpifzhnrq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.sjlbkw.cn/Article/details/gwimrktcq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/ghpnblpgo.sHtML

[Q41] 多表连接
来源：http://blog.yfazqb.com/Article/details/gifgndxge.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fktsv.cn/Article/details/gvdsqlttq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.vehdjk.com/Article/details/gyygnbxvc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gjgsoqaax.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.yfazqb.com/Article/details/gvpckgdjq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.yfazqb.com/Article/details/gcdcrbudl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.vehdjk.com/Article/details/gddqodzwc.sHtML

[Q43] 标量子查询
来源：http://3g.fktsv.cn/Article/details/gwlztefik.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.epnwcf.com/Article/details/gmeiekixd.sHtML

[Q44] IN 子查询
来源：http://3g.tarul.cn/Article/details/gwoufhbiq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.tarul.cn/Article/details/gcgwvymfg.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.tarul.cn/Article/details/gtzxcqhyl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gbkyshxar.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/gyrlqukmx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gcjudfnhs.sHtML

[Q47] 与平均值比较
来源：http://3g.yfazqb.com/Article/details/gpzwdpvvk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.bbcook.cn/Article/details/gujrnbfgs.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.bbcook.cn/Article/details/grtxmyech.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.yfazqb.com/Article/details/gqtorboat.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.yfazqb.com/Article/details/gcojfkfgf.sHtML

[Q49] 更新单行
来源：http://www.blog.yfazqb.com/Article/details/gaxqafbpf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gciygpfpj.sHtML

[Q50] 批量更新
来源：http://baike.tarul.cn/Article/details/giwojfvnr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.epnwcf.com/Article/details/gxwsnxblu.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fktsv.cn/Article/details/gbdszoyhy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.tarul.cn/Article/details/gvthdlgho.sHtML

[Q52] 删除指定行
来源：http://blog.yfazqb.com/Article/details/gykpdrgjp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.tarul.cn/Article/details/ggpudkkvp.sHtML

[Q53] 按条件删除
来源：http://www.share.vehdjk.com/Article/details/ghsmgjqvo.sHtML


<!-- 参考信息 -->