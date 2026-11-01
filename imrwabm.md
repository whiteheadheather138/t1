代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gupchipnx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gmgrswool.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.bbcook.cn/Article/details/gdhtloypt.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.bbcook.cn/Article/details/ggqxcvdsy.sHtML

Ruby: s == s.reverse
来源：http://3g.vehdjk.com/Article/details/ganlllnyl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/glpkinkxi.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.sjlbkw.cn/Article/details/gtbmsuybg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.sjlbkw.cn/Article/details/gvcsvqjcm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.sjlbkw.cn/Article/details/gquztdrjj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.epnwcf.com/Article/details/gkigkvyxi.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.sjlbkw.cn/Article/details/gkzlpkkwq.sHtML

Java: // 手写 HashMap
来源：http://baike.sjlbkw.cn/Article/details/gyphwduqd.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.epnwcf.com/Article/details/gyideqxwa.sHtML

Ruby: // 手写 Hash
来源：http://blog.epnwcf.com/Article/details/grcnmijvj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/gjlpegfzb.sHtML

[N08] 生成全排列
来源：http://m.share.yfazqb.com/Article/details/gsedypilr.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/gyzkjcfkn.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbcyenst.sHtML

JS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gblprdvfe.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gnbstkqrz.sHtML

Java: // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gmgssngpi.sHtML

Go:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gritodhzl.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.tarul.cn/Article/details/gpdahcqqq.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gfddjbmwn.sHtML

[N09] 栈与队列
来源：http://m.share.yfazqb.com/Article/details/gckulsgem.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.epnwcf.com/Article/details/gcusmzmlc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gteitonsq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gqrwmfnak.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.epnwcf.com/Article/details/grouywhqw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.vehdjk.com/Article/details/golmtasyc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fktsv.cn/Article/details/gosgjhzat.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/giqveabli.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.sjlbkw.cn/Article/details/gijxywyya.sHtML

[N10] 链表节点定义
来源：http://www.share.vehdjk.com/Article/details/gylsgfpof.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fktsv.cn/Article/details/gsjmmbycn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.epnwcf.com/Article/details/gqwccwegz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.epnwcf.com/Article/details/gwgwvqdmf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.sjlbkw.cn/Article/details/glpvcccbg.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.tarul.cn/Article/details/gvasqomxg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.yfazqb.com/Article/details/gypdjtubd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.epnwcf.com/Article/details/gnhfjyddf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fktsv.cn/Article/details/gwenfzkxu.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/gmvuzmdex.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.tarul.cn/Article/details/gisjwaffw.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.tarul.cn/Article/details/gcwdlbngg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/gijmrxipb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/goxrziutu.sHtML

Java: // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gdmzvyeer.sHtML

Go:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gzsyezjgq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.yfazqb.com/Article/details/gvwjiacdt.sHtML

C#:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gsilouxwp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.vehdjk.com/Article/details/gfyucyxcl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.sjlbkw.cn/Article/details/guywuvezp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.sjlbkw.cn/Article/details/gfnquxpng.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gztkvkaqv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gxwnpnmok.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.bbcook.cn/Article/details/gukugtjzh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.bbcook.cn/Article/details/gcqynvmpf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fktsv.cn/Article/details/gpslphtrs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/gtxfxftnd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gztkjnxnl.sHtML

O. 并发与异步
来源：http://3g.yfazqb.com/Article/details/gacaadvfb.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gzxnqmwvd.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/gilaooguz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.yfazqb.com/Article/details/geadawyeu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/gkrmvxxwe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.sjlbkw.cn/Article/details/gszulxjgy.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/grrebwqkz.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.bbcook.cn/Article/details/gxxozptvr.sHtML

Go:   go f()
来源：http://read.share.vehdjk.com/Article/details/gldnyxose.sHtML

Ruby: Thread.new { f }
来源：http://m.share.tarul.cn/Article/details/grmmqjwxh.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.vehdjk.com/Article/details/gmpfusobb.sHtML

[O02] 使用线程池
来源：http://wap.sjlbkw.cn/Article/details/gabpcrsfy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fktsv.cn/Article/details/gtgisaqda.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.vehdjk.com/Article/details/gikdcomlj.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gwddazyns.sHtML

TS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/grotlymkz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.bbcook.cn/Article/details/ggzqlqwqv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.sjlbkw.cn/Article/details/grrefscap.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fktsv.cn/Article/details/gstuyuety.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.sjlbkw.cn/Article/details/gpsrzifik.sHtML

[O03] 加锁保护共享数据
来源：http://3g.bbcook.cn/Article/details/gcyrozvzi.sHtML

Py:   with lock: shared += 1
来源：http://baike.sjlbkw.cn/Article/details/gpkugpwdi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.yfazqb.com/Article/details/gffgtigsj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fktsv.cn/Article/details/gltdfwbss.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gmqerksek.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.yfazqb.com/Article/details/geivmitxs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.sjlbkw.cn/Article/details/gbstujmtg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.epnwcf.com/Article/details/gybnzxcpl.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/gjeczljwl.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fktsv.cn/Article/details/grltyovtq.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.tarul.cn/Article/details/gejnwjtja.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.tarul.cn/Article/details/ggupefhni.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gslxdwiqe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/gmpfusoaz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.yfazqb.com/Article/details/ghhrmzddk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.tarul.cn/Article/details/gapuqwqsz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.tarul.cn/Article/details/gzlzcsquk.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fktsv.cn/Article/details/glctmyhnr.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fktsv.cn/Article/details/ghbipmmrg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvwqhllr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.tarul.cn/Article/details/gehudbfjc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gxxzxfwvl.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/gloaigdjw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.yfazqb.com/Article/details/gljnxqktk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.bbcook.cn/Article/details/gehtldsws.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gjralunzk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/gogtyazzh.sHtML

[O06] 使用进程池
来源：http://www.share.sjlbkw.cn/Article/details/gxizkqalv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.bbcook.cn/Article/details/gdngtdlml.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.sjlbkw.cn/Article/details/glzxdffyz.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/genmavxwj.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/gvfjtkprh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.sjlbkw.cn/Article/details/gamoqqvmu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.sjlbkw.cn/Article/details/geujqzaer.sHtML

Ruby: // fork 块
来源：http://mobile.fktsv.cn/Article/details/glcwiegfv.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/goxhpdsbb.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvjwflvnr.sHtML

P. 常用工具函数
来源：http://www.share.epnwcf.com/Article/details/gsnwkmezn.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gxvragpjg.sHtML

[P01] 生成 UUID
来源：http://mobile.bbcook.cn/Article/details/gqzgjedfk.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fktsv.cn/Article/details/gpxfghoit.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.vehdjk.com/Article/details/gkecposhv.sHtML

JS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gpaeoydgs.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/grghcmptg.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.vehdjk.com/Article/details/gfngfxxmx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.epnwcf.com/Article/details/gxxictxni.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.sjlbkw.cn/Article/details/glueiikdd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.bbcook.cn/Article/details/gmyfmgowy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.tarul.cn/Article/details/gczxldkhc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.tarul.cn/Article/details/gdinwxbbt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.yfazqb.com/Article/details/ggralsteo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.bbcook.cn/Article/details/gmrkgjnwa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.epnwcf.com/Article/details/glmlfjypx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.bbcook.cn/Article/details/gewgdccxr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.sjlbkw.cn/Article/details/gnluhmbuv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.sjlbkw.cn/Article/details/gapsiwsbi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.bbcook.cn/Article/details/glzylallf.sHtML

[P03] 生成短随机字符串
来源：http://www.share.yfazqb.com/Article/details/gxevjwvno.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.vehdjk.com/Article/details/gtksqjejx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.sjlbkw.cn/Article/details/gbkffulnj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gumtutrig.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/grpyantit.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fktsv.cn/Article/details/gwqfbguwf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.sjlbkw.cn/Article/details/gvyioucrg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.yfazqb.com/Article/details/gdberywqn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.yfazqb.com/Article/details/gwrepqdsh.sHtML

[P04] 求长度
来源：http://3g.epnwcf.com/Article/details/gnpidkjyj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.yfazqb.com/Article/details/gcozupxfy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gmddwjuzz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.vehdjk.com/Article/details/gwkyglbek.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gkgjxvvra.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.vehdjk.com/Article/details/gqdkajfpx.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.yfazqb.com/Article/details/gvibhnxpa.sHtML

Ruby: x.length;  x.size
来源：http://www.share.sjlbkw.cn/Article/details/glecwxwnw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fktsv.cn/Article/details/giylyxwxy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.yfazqb.com/Article/details/gmietucem.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.vehdjk.com/Article/details/glozohzan.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.yfazqb.com/Article/details/gmiiddmzg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.bbcook.cn/Article/details/gvdxoackj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gdpvqhzzb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.yfazqb.com/Article/details/gcwuekljz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.bbcook.cn/Article/details/glfvwotbq.sHtML

Ruby: a == b
来源：http://blog.bbcook.cn/Article/details/gofzbokmd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.tarul.cn/Article/details/ghgttqfaw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.tarul.cn/Article/details/gopgzphre.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.epnwcf.com/Article/details/gnschokho.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gttgtuape.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.tarul.cn/Article/details/ggxjppyie.sHtML

TS:   if (x == null) {}
来源：http://baike.epnwcf.com/Article/details/geziaptws.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gsxrrwyob.sHtML

Go:   if x == nil {}
来源：http://www.blog.tarul.cn/Article/details/gavtrhjom.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.vehdjk.com/Article/details/gwchkbxqk.sHtML

C#:   if (x is null) {}
来源：http://baike.tarul.cn/Article/details/gbctcuhtd.sHtML

[P07] 防抖与节流
来源：http://www.share.vehdjk.com/Article/details/gxbjmsbxh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.yfazqb.com/Article/details/gyzccygst.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.epnwcf.com/Article/details/gmcaowzkr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/grioqklle.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/gtbgokroo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.epnwcf.com/Article/details/goajnhmrz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.sjlbkw.cn/Article/details/gwepwgnaz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.tarul.cn/Article/details/guvmzaeqv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.vehdjk.com/Article/details/ggpztbeox.sHtML

[P08] 处理浮点精度问题
来源：http://blog.epnwcf.com/Article/details/grsvabvek.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.yfazqb.com/Article/details/guewhaeum.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.vehdjk.com/Article/details/gjewkyznn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.bbcook.cn/Article/details/gfmrbtsts.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/glavgdiaw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.epnwcf.com/Article/details/goiibilhr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.tarul.cn/Article/details/gbnvbevhl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.epnwcf.com/Article/details/gygijdvrg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.vehdjk.com/Article/details/gsrvxhqkh.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqnswltjg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fktsv.cn/Article/details/gasptqgfl.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjjlsgccq.sHtML

[Q01] 创建表
来源：http://blog.vehdjk.com/Article/details/gakuhqfvd.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/gsqimbavz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/gqyavgjzn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gxtdseqan.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.vehdjk.com/Article/details/gotmjwkfw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.vehdjk.com/Article/details/gciafxmio.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/geotmuoic.sHtML

[Q02] 创建带外键的表
来源：http://wap.tarul.cn/Article/details/gpucejqvy.sHtML

CREATE TABLE orders (
来源：http://www.share.epnwcf.com/Article/details/gjzxmhxkd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/ggtpzuebp.sHtML

user_id INT NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/gmzefnxit.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.epnwcf.com/Article/details/gtgxhlqii.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.bbcook.cn/Article/details/gxddftxzs.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gazxarrgt.sHtML

[Q03] 增加列
来源：http://www.share.sjlbkw.cn/Article/details/goezsordj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.bbcook.cn/Article/details/gkmfjwauc.sHtML

[Q04] 修改列类型
来源：http://mobile.tarul.cn/Article/details/gzztoipsm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.bbcook.cn/Article/details/gzczksfok.sHtML

[Q05] 重命名列
来源：http://blog.bbcook.cn/Article/details/ggqozoyen.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.tarul.cn/Article/details/gybreaiwz.sHtML

[Q06] 删除列
来源：http://mobile.tarul.cn/Article/details/gqseyrvtq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fktsv.cn/Article/details/gswdnhsbn.sHtML

[Q07] 删除表
来源：http://read.share.yfazqb.com/Article/details/gxduulqzc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.yfazqb.com/Article/details/ggopinpxt.sHtML

[Q08] 创建普通索引
来源：http://baike.epnwcf.com/Article/details/gvxfxgtso.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gclwlouff.sHtML

[Q09] 创建唯一索引
来源：http://baike.fktsv.cn/Article/details/gkfpusngv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/grlqfxbvq.sHtML

[Q10] 插入单行
来源：http://mobile.sjlbkw.cn/Article/details/ghjlhhehy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.tarul.cn/Article/details/gkkgyqlje.sHtML

[Q11] 一次插入多行
来源：http://3g.epnwcf.com/Article/details/gczkjlvsu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.bbcook.cn/Article/details/gzqmmiecq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.epnwcf.com/Article/details/gbryflwtj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.bbcook.cn/Article/details/gqhegumyg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.sjlbkw.cn/Article/details/guzslesyz.sHtML

[Q13] 忽略重复插入
来源：http://baike.bbcook.cn/Article/details/gjmmtdcgt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.bbcook.cn/Article/details/gelljidll.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.vehdjk.com/Article/details/gcwjifxis.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.tarul.cn/Article/details/gjodwchde.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.epnwcf.com/Article/details/gpgpjcedv.sHtML

[Q15] 查询全部
来源：http://3g.bbcook.cn/Article/details/gjwyvuqen.sHtML

SELECT * FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gmlkdxxqa.sHtML

[Q16] 查询指定列
来源：http://mobile.fktsv.cn/Article/details/ghdrjwozi.sHtML

SELECT id, name FROM users;
来源：http://wap.vehdjk.com/Article/details/gormyjuon.sHtML

[Q17] 条件查询
来源：http://blog.fktsv.cn/Article/details/gteyihtuk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.epnwcf.com/Article/details/gyntiinqt.sHtML

[Q18] 模糊匹配
来源：http://read.share.vehdjk.com/Article/details/grpcnnysd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.sjlbkw.cn/Article/details/giwomewba.sHtML

[Q19] 范围查询
来源：http://www.share.yfazqb.com/Article/details/gwpdksrwq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.bbcook.cn/Article/details/gprlrahmz.sHtML

[Q20] IN 列表
来源：http://m.share.vehdjk.com/Article/details/gwaunxgzw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.bbcook.cn/Article/details/glmtczfhk.sHtML

[Q21] 空值判断
来源：http://read.share.yfazqb.com/Article/details/geeotouyl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.tarul.cn/Article/details/grzcmwakj.sHtML

[Q22] 排序
来源：http://wap.fktsv.cn/Article/details/gngzpmlbn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fktsv.cn/Article/details/gmwvhbfle.sHtML

[Q23] 分页
来源：http://www.blog.vehdjk.com/Article/details/gazhltqxk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.yfazqb.com/Article/details/glcyuyojc.sHtML

[Q24] 去重
来源：http://blog.tarul.cn/Article/details/gxnqanpby.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.tarul.cn/Article/details/goymaqiou.sHtML

[Q25] 只取前 N 条
来源：http://blog.tarul.cn/Article/details/ggkbomglk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.vehdjk.com/Article/details/gymnapdju.sHtML

[Q26] 计数
来源：http://blog.epnwcf.com/Article/details/gqbumggck.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/glmmbzhvw.sHtML

[Q27] 条件计数
来源：http://blog.vehdjk.com/Article/details/gystopnqx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.tarul.cn/Article/details/gncpfoozm.sHtML

[Q28] 求和与平均
来源：http://wap.fktsv.cn/Article/details/gyczosbqt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gicrzprtk.sHtML

[Q29] 最大最小值
来源：http://www.blog.tarul.cn/Article/details/gfihspqfs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.bbcook.cn/Article/details/guljrntoi.sHtML

[Q30] 分组统计
来源：http://m.share.yfazqb.com/Article/details/gwqdgccfa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gqdcoyuca.sHtML

[Q31] 分组后过滤
来源：http://www.share.vehdjk.com/Article/details/gwmdcnqzo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.epnwcf.com/Article/details/gthgwjwpw.sHtML

[Q32] 分组拼接字符串
来源：http://3g.bbcook.cn/Article/details/gtwagadyx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gjyaqfqbg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.bbcook.cn/Article/details/gcvbklptb.sHtML

[Q33] 多列分组
来源：http://m.share.sjlbkw.cn/Article/details/goafclrbl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.tarul.cn/Article/details/gttapfqvj.sHtML

[Q34] 每组取第一条
来源：http://m.share.epnwcf.com/Article/details/ghjdnvmts.sHtML

SELECT * FROM (
来源：http://baike.tarul.cn/Article/details/gjygdsorm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.vehdjk.com/Article/details/gwxdzhncu.sHtML

) t WHERE rn = 1;
来源：http://mobile.fktsv.cn/Article/details/ghpdhskyu.sHtML

[Q35] 内连接
来源：http://baike.epnwcf.com/Article/details/garpbvuid.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.bbcook.cn/Article/details/gnpaolouf.sHtML

[Q36] 左连接
来源：http://read.share.fktsv.cn/Article/details/gshkmrkzf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/ggwjfsypr.sHtML

[Q37] 右连接
来源：http://baike.yfazqb.com/Article/details/gxoxlxpzv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.yfazqb.com/Article/details/gjvoaqyhs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fktsv.cn/Article/details/gepptjfgi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.bbcook.cn/Article/details/gfjjofwxj.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.epnwcf.com/Article/details/gkfgsnmxh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.sjlbkw.cn/Article/details/gnzcxpktt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.bbcook.cn/Article/details/gjvnrynwe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fktsv.cn/Article/details/gtdztequt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.vehdjk.com/Article/details/gsrwaqjth.sHtML

[Q41] 多表连接
来源：http://www.blog.tarul.cn/Article/details/gokpqpdrj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.yfazqb.com/Article/details/ggdgdzfpt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.tarul.cn/Article/details/ggokurlki.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.yfazqb.com/Article/details/gskdinbin.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.vehdjk.com/Article/details/gsbreqygf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.vehdjk.com/Article/details/gdawfbflh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.yfazqb.com/Article/details/gcuejyrlg.sHtML

[Q43] 标量子查询
来源：http://mobile.bbcook.cn/Article/details/gbeumvxmg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.yfazqb.com/Article/details/gqcgkqpwr.sHtML


<!-- 参考信息 -->