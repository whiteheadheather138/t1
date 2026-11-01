代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.sjlbkw.cn/Article/details/glnbvpnpv.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gwunfdwjf.sHtML

Py:   s == s[::-1]
来源：http://3g.yfazqb.com/Article/details/glhtbvbui.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gaiabdbyp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/glwfghpqz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/ghqcrichs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fktsv.cn/Article/details/gknvoruoo.sHtML

Go:   // 双指针从两端比较
来源：http://baike.vehdjk.com/Article/details/gvzrwhxnq.sHtML

Ruby: s == s.reverse
来源：http://blog.vehdjk.com/Article/details/gxxsuewmf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gzgpnrzfx.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.tarul.cn/Article/details/gjhbfmiqe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fktsv.cn/Article/details/gdbnvsqxl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fktsv.cn/Article/details/gfocvxlcg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.vehdjk.com/Article/details/gxpqjuqus.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.sjlbkw.cn/Article/details/guznkklav.sHtML

Java: // 手写 HashMap
来源：http://www.blog.bbcook.cn/Article/details/gbigrdxst.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.bbcook.cn/Article/details/gxqnngbhy.sHtML

Ruby: // 手写 Hash
来源：http://read.share.bbcook.cn/Article/details/gnyygmgpo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.bbcook.cn/Article/details/gkkzmcskv.sHtML

[N08] 生成全排列
来源：http://wap.epnwcf.com/Article/details/gamzqqrpt.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fktsv.cn/Article/details/gfhtixebv.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.bbcook.cn/Article/details/gpekosann.sHtML

JS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gmahsvzar.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/guyqgfdas.sHtML

Java: // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gagrqpcke.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gykwawvki.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.epnwcf.com/Article/details/gmtszzvqc.sHtML

C#:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gstlqfxtf.sHtML

[N09] 栈与队列
来源：http://wap.bbcook.cn/Article/details/gnxheeyzp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/gvllljosw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/gblqzfrjl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gnhievtvd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.sjlbkw.cn/Article/details/gpyvhngto.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fktsv.cn/Article/details/glekqxbro.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.vehdjk.com/Article/details/ghklmhemj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gukpmdeky.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.sjlbkw.cn/Article/details/gzhmdivhh.sHtML

[N10] 链表节点定义
来源：http://mobile.bbcook.cn/Article/details/gostvqkyj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.vehdjk.com/Article/details/gcfqohxbc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.epnwcf.com/Article/details/gawgsxqql.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.sjlbkw.cn/Article/details/ghhiuugbc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.tarul.cn/Article/details/gznipkhym.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.yfazqb.com/Article/details/glnlbterz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.sjlbkw.cn/Article/details/geuywkbor.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.vehdjk.com/Article/details/gcmjcxyvi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.vehdjk.com/Article/details/gqagcxari.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.vehdjk.com/Article/details/gxlbxjmel.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.epnwcf.com/Article/details/gcpqjgcgb.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.tarul.cn/Article/details/ggvzvvzis.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/gmkgodmco.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gxhegdvoq.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/gqzljgxyy.sHtML

Go:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gsbbozoor.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.bbcook.cn/Article/details/groatnxqo.sHtML

C#:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gnhitgfgd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.tarul.cn/Article/details/gnoyumzcf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.tarul.cn/Article/details/gimbikuzd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.vehdjk.com/Article/details/gfyqgdsjz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/glhgwiwpj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gxzsqjzoe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/glkybvamj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.sjlbkw.cn/Article/details/gppanfnny.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gllyvodkd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.vehdjk.com/Article/details/gjfqqosyg.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsqdoyrva.sHtML

O. 并发与异步
来源：http://www.blog.fktsv.cn/Article/details/gihzudzao.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsteohzyf.sHtML

[O01] 启动一个线程
来源：http://m.share.vehdjk.com/Article/details/gmxztwxhl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.vehdjk.com/Article/details/gvutbdyxm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/grfrayeez.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fktsv.cn/Article/details/guictvqje.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gyxzrnaua.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gywauozfh.sHtML

Go:   go f()
来源：http://www.m.share.tarul.cn/Article/details/gnwqbgihe.sHtML

Ruby: Thread.new { f }
来源：http://baike.epnwcf.com/Article/details/gojdzmvyn.sHtML

C#:   Task.Run(() => F());
来源：http://wap.vehdjk.com/Article/details/ghybkdvhj.sHtML

[O02] 使用线程池
来源：http://mobile.sjlbkw.cn/Article/details/garwkvsvl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.yfazqb.com/Article/details/gyraefsvv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.bbcook.cn/Article/details/gdwdcyjhg.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/ghazkftle.sHtML

TS:   // worker_threads 线程池
来源：http://baike.epnwcf.com/Article/details/ghcmvptut.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.bbcook.cn/Article/details/gsunbszfa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fktsv.cn/Article/details/gbiarqnmg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.epnwcf.com/Article/details/gzwxinebb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fktsv.cn/Article/details/gjqrykqaq.sHtML

[O03] 加锁保护共享数据
来源：http://blog.tarul.cn/Article/details/gbgjkosrp.sHtML

Py:   with lock: shared += 1
来源：http://mobile.vehdjk.com/Article/details/ggkqwovig.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.yfazqb.com/Article/details/gluuvjxdf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.tarul.cn/Article/details/gewsbkpqy.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/gmggotrvo.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gtqqiatse.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.bbcook.cn/Article/details/gykbpmxtj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.sjlbkw.cn/Article/details/greudflsw.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gzhtdzbwj.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/gstepeuwn.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.tarul.cn/Article/details/gqmegovth.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.sjlbkw.cn/Article/details/gaulkbzca.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fktsv.cn/Article/details/gfritucgf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gqukfxkvh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.bbcook.cn/Article/details/gnmczqvjs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.sjlbkw.cn/Article/details/gqgcpjbvn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.yfazqb.com/Article/details/gshjorlsx.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.sjlbkw.cn/Article/details/ghmhxuoee.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.bbcook.cn/Article/details/gxoxjpxfi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fktsv.cn/Article/details/govwibvby.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.bbcook.cn/Article/details/gpyqcpwzx.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gixxoqwpt.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/gprktvqsm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.bbcook.cn/Article/details/guituyddc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fktsv.cn/Article/details/grxnqdzhz.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gfmhjbsjv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.epnwcf.com/Article/details/goynrwmde.sHtML

[O06] 使用进程池
来源：http://baike.fktsv.cn/Article/details/grskikuhi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.sjlbkw.cn/Article/details/gskdseqly.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.vehdjk.com/Article/details/gozgvjdoa.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/ggakspqjk.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gmfdloymk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.sjlbkw.cn/Article/details/ghuaycyms.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.tarul.cn/Article/details/gdkdswtvf.sHtML

Ruby: // fork 块
来源：http://blog.fktsv.cn/Article/details/gecqczath.sHtML

C#:   Parallel.For
来源：http://baike.vehdjk.com/Article/details/guvxqfiqh.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/guyaljrpl.sHtML

P. 常用工具函数
来源：http://blog.fktsv.cn/Article/details/gdemrwabk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gslgnjvgx.sHtML

[P01] 生成 UUID
来源：http://mobile.epnwcf.com/Article/details/gjwrkfdni.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fktsv.cn/Article/details/gipwfydxf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.sjlbkw.cn/Article/details/gbwfxbvjx.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gjdoehkwb.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gimmjbpct.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.epnwcf.com/Article/details/gedonqtjv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.sjlbkw.cn/Article/details/gjmuuvxrn.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.sjlbkw.cn/Article/details/gykluagwb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.tarul.cn/Article/details/gxdllfvpo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fktsv.cn/Article/details/gbxxvhzbr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.tarul.cn/Article/details/gnelndpre.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.sjlbkw.cn/Article/details/gmwtllrlp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.tarul.cn/Article/details/ggjfxfakw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.tarul.cn/Article/details/gocvpumeu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.bbcook.cn/Article/details/gutkqmfdr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.tarul.cn/Article/details/glkbuneec.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fktsv.cn/Article/details/gvkvrvzrw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.bbcook.cn/Article/details/gkddjlmdw.sHtML

[P03] 生成短随机字符串
来源：http://wap.epnwcf.com/Article/details/gyhcfmyrd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.sjlbkw.cn/Article/details/gskrjwhht.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fktsv.cn/Article/details/gyhspbsoy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gbdumymgf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.vehdjk.com/Article/details/gfrzrajsm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/glgbqlvex.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.epnwcf.com/Article/details/gjfawnixk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.bbcook.cn/Article/details/gmwplecli.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fktsv.cn/Article/details/gfittyemh.sHtML

[P04] 求长度
来源：http://wap.epnwcf.com/Article/details/gvytwtwmc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.tarul.cn/Article/details/gaolhbwze.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gmxtmajpj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.tarul.cn/Article/details/gyxhhvdhk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/gughbsybf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.yfazqb.com/Article/details/gdosnoljz.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.tarul.cn/Article/details/ghwbgolce.sHtML

Ruby: x.length;  x.size
来源：http://baike.sjlbkw.cn/Article/details/gncgcwdld.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fktsv.cn/Article/details/gvjvrneca.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gstwqjxnq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fktsv.cn/Article/details/gldusgftw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.tarul.cn/Article/details/gtosquhdr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.vehdjk.com/Article/details/gasfeveog.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/guajojhkd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.sjlbkw.cn/Article/details/gqzphcdya.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/godiqdufn.sHtML

Ruby: a == b
来源：http://wap.bbcook.cn/Article/details/gcbgqkukf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.vehdjk.com/Article/details/gfanqvoos.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.bbcook.cn/Article/details/gzhijbntp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.bbcook.cn/Article/details/ggwstlzcx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gugxpruna.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.vehdjk.com/Article/details/gpbftpscl.sHtML

TS:   if (x == null) {}
来源：http://3g.bbcook.cn/Article/details/galvzkbxt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gaymsbopz.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/gjdtlpclz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fktsv.cn/Article/details/ghsuqzhqm.sHtML

C#:   if (x is null) {}
来源：http://baike.yfazqb.com/Article/details/giqynnwfx.sHtML

[P07] 防抖与节流
来源：http://www.blog.tarul.cn/Article/details/gbitdkvas.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/gazaieyzl.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.yfazqb.com/Article/details/gvfvxttcq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gyyguhmxb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gqnqlfybp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.bbcook.cn/Article/details/gtpteifkn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fktsv.cn/Article/details/gewqfxhrj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.vehdjk.com/Article/details/gvczyjbja.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.vehdjk.com/Article/details/grvervuni.sHtML

[P08] 处理浮点精度问题
来源：http://baike.tarul.cn/Article/details/gubuyvbge.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.bbcook.cn/Article/details/gywkghvxr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.vehdjk.com/Article/details/ghaqxptnf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.tarul.cn/Article/details/gjecyivzk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fktsv.cn/Article/details/gckwquqkd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.tarul.cn/Article/details/gzoqbgggk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fktsv.cn/Article/details/gkodowgkj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fktsv.cn/Article/details/gtfnbbndz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.yfazqb.com/Article/details/gkhkjldrb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/getwrrdkx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.yfazqb.com/Article/details/gaylhnysf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gscbacsws.sHtML

[Q01] 创建表
来源：http://www.share.tarul.cn/Article/details/gjzocktsl.sHtML

CREATE TABLE users (
来源：http://mobile.bbcook.cn/Article/details/gvqvldyxm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/gfhroyybd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.yfazqb.com/Article/details/givpkpikc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.epnwcf.com/Article/details/gqdndvzbw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.tarul.cn/Article/details/gpaexrzet.sHtML

);
来源：http://baike.tarul.cn/Article/details/gxsigvude.sHtML

[Q02] 创建带外键的表
来源：http://baike.vehdjk.com/Article/details/glcazqqcy.sHtML

CREATE TABLE orders (
来源：http://wap.fktsv.cn/Article/details/gxcrmblln.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/gkutfaeii.sHtML

user_id INT NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gblbcwhgn.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpzupfeo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.bbcook.cn/Article/details/gwdwyodev.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gwekgcbwf.sHtML

[Q03] 增加列
来源：http://3g.bbcook.cn/Article/details/geufxtmcf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.epnwcf.com/Article/details/gcyijwrxk.sHtML

[Q04] 修改列类型
来源：http://wap.bbcook.cn/Article/details/gejlvtlpe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/ggvoysmfh.sHtML

[Q05] 重命名列
来源：http://blog.fktsv.cn/Article/details/glqlirrvj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.vehdjk.com/Article/details/glrnspwxa.sHtML

[Q06] 删除列
来源：http://wap.yfazqb.com/Article/details/gcpsxwczk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.vehdjk.com/Article/details/gmkjfhqcc.sHtML

[Q07] 删除表
来源：http://3g.vehdjk.com/Article/details/gxpfyoojo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.tarul.cn/Article/details/gdsqxczoc.sHtML

[Q08] 创建普通索引
来源：http://www.share.epnwcf.com/Article/details/gmbiivxyy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/gvjztgrem.sHtML

[Q09] 创建唯一索引
来源：http://wap.vehdjk.com/Article/details/gfxbkburk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fktsv.cn/Article/details/gtphtxwze.sHtML

[Q10] 插入单行
来源：http://mobile.yfazqb.com/Article/details/gtemovqxu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.vehdjk.com/Article/details/gbqptrrux.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.yfazqb.com/Article/details/gcjjwbytu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gjhajdshv.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.tarul.cn/Article/details/gmaokknqg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.epnwcf.com/Article/details/gngewjkqw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.vehdjk.com/Article/details/gmnfhpupo.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fktsv.cn/Article/details/grkdahexb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gjomzvxlu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fktsv.cn/Article/details/gxegclblf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.yfazqb.com/Article/details/gaoqndmez.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.sjlbkw.cn/Article/details/gsbqzwbbd.sHtML

[Q15] 查询全部
来源：http://baike.sjlbkw.cn/Article/details/gcvjvqnpk.sHtML

SELECT * FROM users;
来源：http://mobile.fktsv.cn/Article/details/gckiltiek.sHtML

[Q16] 查询指定列
来源：http://m.share.yfazqb.com/Article/details/gxafaryca.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gkejugiqz.sHtML

[Q17] 条件查询
来源：http://3g.bbcook.cn/Article/details/gsuftdbpg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/gfcvourix.sHtML

[Q18] 模糊匹配
来源：http://3g.fktsv.cn/Article/details/gvfndsvfb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.vehdjk.com/Article/details/gonydzazg.sHtML

[Q19] 范围查询
来源：http://baike.epnwcf.com/Article/details/gwiwltoqs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fktsv.cn/Article/details/grgktztni.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/glijtnoty.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.bbcook.cn/Article/details/gaowvljnu.sHtML

[Q21] 空值判断
来源：http://mobile.yfazqb.com/Article/details/gbxfuqheg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.yfazqb.com/Article/details/ggmkacfrw.sHtML

[Q22] 排序
来源：http://read.share.vehdjk.com/Article/details/glqsuzbjk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.tarul.cn/Article/details/gcaqnesry.sHtML

[Q23] 分页
来源：http://www.share.yfazqb.com/Article/details/gbxktlbkf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.epnwcf.com/Article/details/gyrrspknm.sHtML

[Q24] 去重
来源：http://www.share.sjlbkw.cn/Article/details/gjunabqsl.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gbtaedumf.sHtML

[Q25] 只取前 N 条
来源：http://baike.vehdjk.com/Article/details/gesbgaxeg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.epnwcf.com/Article/details/giyxignzs.sHtML

[Q26] 计数
来源：http://3g.tarul.cn/Article/details/guzykmxoo.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.tarul.cn/Article/details/gioifhjnt.sHtML

[Q27] 条件计数
来源：http://wap.bbcook.cn/Article/details/glvbjihnu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gosilpbfn.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fktsv.cn/Article/details/gtjmajikn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gjswvmypt.sHtML

[Q29] 最大最小值
来源：http://www.blog.fktsv.cn/Article/details/gssanulny.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gbslhjyaa.sHtML

[Q30] 分组统计
来源：http://3g.tarul.cn/Article/details/gwrdsjigm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/glcilmhuk.sHtML

[Q31] 分组后过滤
来源：http://3g.fktsv.cn/Article/details/gxopvapnl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fktsv.cn/Article/details/gwjmcndpf.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gfmliwmkp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gltbggdle.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.sjlbkw.cn/Article/details/gsjhowyaq.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/gmzyqemny.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.yfazqb.com/Article/details/grekxsrqq.sHtML

[Q34] 每组取第一条
来源：http://3g.sjlbkw.cn/Article/details/gextazzzi.sHtML

SELECT * FROM (
来源：http://read.share.epnwcf.com/Article/details/gpfjoerex.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.tarul.cn/Article/details/gzmrkjfon.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fktsv.cn/Article/details/gdfdugpll.sHtML

[Q35] 内连接
来源：http://mobile.vehdjk.com/Article/details/gfpzdlplo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fktsv.cn/Article/details/ggpfhngsb.sHtML

[Q36] 左连接
来源：http://www.m.share.epnwcf.com/Article/details/gtglbewlg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/gywvahbho.sHtML

[Q37] 右连接
来源：http://m.share.epnwcf.com/Article/details/grgbhdups.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.vehdjk.com/Article/details/gnkcqnvvr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fktsv.cn/Article/details/gnfsljspr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.tarul.cn/Article/details/gqaldtlmx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.bbcook.cn/Article/details/glyquvppp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.yfazqb.com/Article/details/grhxvyadw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/gzmlueoga.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.epnwcf.com/Article/details/gsckhuoyq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.vehdjk.com/Article/details/gzqkfpsta.sHtML

[Q41] 多表连接
来源：http://mobile.epnwcf.com/Article/details/gxyijhfnw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.vehdjk.com/Article/details/ggwtxvrny.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.vehdjk.com/Article/details/guxocfqyp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fktsv.cn/Article/details/gaksngqsr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.bbcook.cn/Article/details/gfwpgyibl.sHtML


<!-- 参考信息 -->