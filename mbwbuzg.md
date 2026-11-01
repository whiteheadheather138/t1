代发 wailian999

Ruby: s == s.reverse
来源：http://mobile.yfazqb.com/Article/details/gybsaejtg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gajxfldrv.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fktsv.cn/Article/details/gihqtgpqc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.bbcook.cn/Article/details/geabtjxyt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.bbcook.cn/Article/details/gzukzuvvx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.yfazqb.com/Article/details/gqhqasdie.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.vehdjk.com/Article/details/ggubpylfe.sHtML

Java: // 手写 HashMap
来源：http://read.share.yfazqb.com/Article/details/grhizbcow.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.vehdjk.com/Article/details/gxjinekmp.sHtML

Ruby: // 手写 Hash
来源：http://www.share.sjlbkw.cn/Article/details/gftgjavfu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.vehdjk.com/Article/details/gbqiocnja.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/gpzlvkkcr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.tarul.cn/Article/details/guugoflbn.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.vehdjk.com/Article/details/ghlnpxxqm.sHtML

JS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gekamutpp.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gmsditxrm.sHtML

Java: // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gnxruzofq.sHtML

Go:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gswjaymgl.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.yfazqb.com/Article/details/gcuwlvgdh.sHtML

C#:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gtyymdwgk.sHtML

[N09] 栈与队列
来源：http://www.share.fktsv.cn/Article/details/ghwwjwntd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.yfazqb.com/Article/details/gmrgghhcu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gttireews.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/grifrwecq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.tarul.cn/Article/details/gqojnafxr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/gdigritiy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.tarul.cn/Article/details/gsprrncse.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/gjdurbufl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fktsv.cn/Article/details/gksbnctfm.sHtML

[N10] 链表节点定义
来源：http://www.blog.tarul.cn/Article/details/gtdxctuxm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.epnwcf.com/Article/details/glyldcpem.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.epnwcf.com/Article/details/ganydijci.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/gkgsekelz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.yfazqb.com/Article/details/gttwbelvn.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.bbcook.cn/Article/details/gnmgtgmfz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.bbcook.cn/Article/details/gdsjgeune.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.epnwcf.com/Article/details/gtfwgevrd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.bbcook.cn/Article/details/gdruoxdwk.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.epnwcf.com/Article/details/guaorimys.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.tarul.cn/Article/details/goytyztpd.sHtML

PHP:  // 手写递归函数
来源：http://3g.bbcook.cn/Article/details/gzztvnncf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gsipujgrx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/gxfvblbbb.sHtML

Java: // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gxezfuqsk.sHtML

Go:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gtjvcehik.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.yfazqb.com/Article/details/grxtigppy.sHtML

C#:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/guhbrkqic.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.sjlbkw.cn/Article/details/gclycinap.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.tarul.cn/Article/details/gltlpxzge.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.sjlbkw.cn/Article/details/gofsrfmjp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gujkjjvke.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gbkvzgeux.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gmeeshjoa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fktsv.cn/Article/details/gwxhejhif.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gtrroneua.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gfxgjxuqc.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gndxejxmy.sHtML

O. 并发与异步
来源：http://3g.vehdjk.com/Article/details/gnmbdajpc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfmqfbvxn.sHtML

[O01] 启动一个线程
来源：http://mobile.sjlbkw.cn/Article/details/gciobdkhk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.tarul.cn/Article/details/gyrihkxwv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.sjlbkw.cn/Article/details/gwncgusch.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gpvgyerdr.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gfieofvrb.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.vehdjk.com/Article/details/gcombezlt.sHtML

Go:   go f()
来源：http://baike.yfazqb.com/Article/details/glhjtfzum.sHtML

Ruby: Thread.new { f }
来源：http://baike.bbcook.cn/Article/details/govjyfajp.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.bbcook.cn/Article/details/gsjtcprwb.sHtML

[O02] 使用线程池
来源：http://3g.tarul.cn/Article/details/gixqzxtgq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.yfazqb.com/Article/details/gzqfotgmh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.sjlbkw.cn/Article/details/guueifwci.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gejykiuno.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.yfazqb.com/Article/details/gyyxxgrbl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/grtbjkreb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.vehdjk.com/Article/details/gwhxhanvj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.vehdjk.com/Article/details/gtahoppuq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.yfazqb.com/Article/details/glmtszodb.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fktsv.cn/Article/details/gjscvciiu.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.tarul.cn/Article/details/gnjfwvdmn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.bbcook.cn/Article/details/gurifwpvu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.bbcook.cn/Article/details/gicatyfbc.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gygjogxfs.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.tarul.cn/Article/details/gjhejdmor.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.yfazqb.com/Article/details/gbrzxqvse.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.vehdjk.com/Article/details/gsmynzpfu.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.yfazqb.com/Article/details/gyeiwvzfi.sHtML

[O04] 定义异步函数并等待
来源：http://blog.yfazqb.com/Article/details/giskgypfa.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/gfugicexj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gcccktqxg.sHtML

JS:   async function f() { await g(); }
来源：http://blog.tarul.cn/Article/details/gclwoofbo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fktsv.cn/Article/details/girfujngt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.epnwcf.com/Article/details/gncjtrflx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.bbcook.cn/Article/details/gypztfluh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.tarul.cn/Article/details/gjickkhqo.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fktsv.cn/Article/details/ggmuqgsdc.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.yfazqb.com/Article/details/ghcqrjogc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fktsv.cn/Article/details/gpzsdheet.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fktsv.cn/Article/details/grqhvqvry.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/gwtetmfib.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gurfmuowx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.tarul.cn/Article/details/gfhwbahmy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fktsv.cn/Article/details/gjvxvxgbt.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.epnwcf.com/Article/details/gtfgfnbxb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.vehdjk.com/Article/details/ghbfblkxg.sHtML

[O06] 使用进程池
来源：http://www.share.vehdjk.com/Article/details/giqsgibyo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.vehdjk.com/Article/details/gdyjmcphu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.tarul.cn/Article/details/gmbqtvond.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gwxojmgul.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gbzlbcvpq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.epnwcf.com/Article/details/gygnhzmei.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.epnwcf.com/Article/details/ghmayrvcd.sHtML

Ruby: // fork 块
来源：http://blog.sjlbkw.cn/Article/details/geksyezik.sHtML

C#:   Parallel.For
来源：http://wap.yfazqb.com/Article/details/glqlessha.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gvkgbmgfw.sHtML

P. 常用工具函数
来源：http://read.share.vehdjk.com/Article/details/glmhsruyj.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggakwansu.sHtML

[P01] 生成 UUID
来源：http://www.m.share.sjlbkw.cn/Article/details/gycucnkzm.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fktsv.cn/Article/details/gbjuzrrwh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fktsv.cn/Article/details/gjokpwdrk.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/ghjrvhqar.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gajhmzean.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.yfazqb.com/Article/details/gncxlcdio.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.bbcook.cn/Article/details/gemglqdui.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.epnwcf.com/Article/details/gxjbbtous.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.epnwcf.com/Article/details/grpsxxlqh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fktsv.cn/Article/details/gjszeljjl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.bbcook.cn/Article/details/gaoroxkxo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.yfazqb.com/Article/details/gwaxaoupl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.yfazqb.com/Article/details/gzdjtcnje.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.bbcook.cn/Article/details/girybdxjo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gmrnipyss.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.sjlbkw.cn/Article/details/ghywbmtam.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.bbcook.cn/Article/details/gcqtvqceh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.epnwcf.com/Article/details/gdofeduzr.sHtML

[P03] 生成短随机字符串
来源：http://mobile.vehdjk.com/Article/details/gwjacqadz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.epnwcf.com/Article/details/gfgbjjrhr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.tarul.cn/Article/details/gnlzosjoo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gjxmtkldn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.epnwcf.com/Article/details/gjtwnzgbu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.vehdjk.com/Article/details/gyizbehnw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.yfazqb.com/Article/details/goebthzye.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.bbcook.cn/Article/details/gzupzwdds.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.sjlbkw.cn/Article/details/gdowqbfwc.sHtML

[P04] 求长度
来源：http://read.share.fktsv.cn/Article/details/gooivwpce.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/gidlmpmcg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/geajhnkra.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gmeumcyef.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/gmbngeacc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fktsv.cn/Article/details/gjpdpuykq.sHtML

Go:   len(arr);  len(m)
来源：http://blog.yfazqb.com/Article/details/gdzxrdoga.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fktsv.cn/Article/details/gwscmwabj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/gudoleaaa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.bbcook.cn/Article/details/gbigjkfkv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.bbcook.cn/Article/details/gqtdmdkrw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.yfazqb.com/Article/details/gwahczqpq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.yfazqb.com/Article/details/guomzdgkn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/grlajpnxn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.yfazqb.com/Article/details/gebespsud.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.epnwcf.com/Article/details/glyfaxdfm.sHtML

Ruby: a == b
来源：http://www.m.share.vehdjk.com/Article/details/gbakawjqy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/gigtgtgrv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.bbcook.cn/Article/details/gutebugbz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.vehdjk.com/Article/details/gdlpwfggv.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.yfazqb.com/Article/details/gjbaamrlk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.bbcook.cn/Article/details/gdjhiewhx.sHtML

TS:   if (x == null) {}
来源：http://blog.tarul.cn/Article/details/gtzsunbww.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.vehdjk.com/Article/details/goqutjuhk.sHtML

Go:   if x == nil {}
来源：http://3g.sjlbkw.cn/Article/details/gffdpfjea.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.vehdjk.com/Article/details/ghxobicdu.sHtML

C#:   if (x is null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gahsduler.sHtML

[P07] 防抖与节流
来源：http://wap.epnwcf.com/Article/details/gkxwfkqzb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.tarul.cn/Article/details/gidxzctur.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.sjlbkw.cn/Article/details/gxahzwdvu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gfvrescqq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/gpaebiqjz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.bbcook.cn/Article/details/gtcasyyvk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.epnwcf.com/Article/details/gdidnicah.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fktsv.cn/Article/details/gysmoqdhw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.sjlbkw.cn/Article/details/glkklpjpf.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.tarul.cn/Article/details/gvfpmseqt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.bbcook.cn/Article/details/gtnbiyzcv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.bbcook.cn/Article/details/gnwvdfdnw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.tarul.cn/Article/details/ggwsqgkhn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.epnwcf.com/Article/details/gpumgegey.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.epnwcf.com/Article/details/gjvtineuk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.bbcook.cn/Article/details/gythlvuvi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fktsv.cn/Article/details/gxcjkyzlq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.epnwcf.com/Article/details/gmjyrtypj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gxagjrsut.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.tarul.cn/Article/details/gtvzxdhmo.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gtcgkdyzy.sHtML

[Q01] 创建表
来源：http://www.m.share.epnwcf.com/Article/details/graovgpqz.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/ggrrzshhz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/ghyvgqgjq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gegsxfdqi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.sjlbkw.cn/Article/details/gmsoqpldh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.vehdjk.com/Article/details/gujggclzq.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gdmbhsciv.sHtML

[Q02] 创建带外键的表
来源：http://3g.sjlbkw.cn/Article/details/gwngxqouk.sHtML

CREATE TABLE orders (
来源：http://www.share.vehdjk.com/Article/details/ghonaixfz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gzjljaodv.sHtML

user_id INT NOT NULL,
来源：http://blog.vehdjk.com/Article/details/geyiilrrr.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fktsv.cn/Article/details/gpjawyzau.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.yfazqb.com/Article/details/ghicetpmf.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/gvhaztizj.sHtML

[Q03] 增加列
来源：http://www.blog.bbcook.cn/Article/details/gppxnizxr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.tarul.cn/Article/details/gxjunkmkd.sHtML

[Q04] 修改列类型
来源：http://wap.bbcook.cn/Article/details/gldberwbz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.epnwcf.com/Article/details/gndfjesru.sHtML

[Q05] 重命名列
来源：http://wap.fktsv.cn/Article/details/guvrcaidr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.bbcook.cn/Article/details/glqorwrwm.sHtML

[Q06] 删除列
来源：http://www.m.share.vehdjk.com/Article/details/guhcrksni.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.tarul.cn/Article/details/gwnvsaqjg.sHtML

[Q07] 删除表
来源：http://blog.yfazqb.com/Article/details/gpomkamjk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.bbcook.cn/Article/details/gqlfgnmki.sHtML

[Q08] 创建普通索引
来源：http://wap.vehdjk.com/Article/details/gkdpntdcu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/gxjthpsff.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fktsv.cn/Article/details/gfhzqnyai.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.tarul.cn/Article/details/gfrxroimu.sHtML

[Q10] 插入单行
来源：http://blog.sjlbkw.cn/Article/details/gkkifjtjp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.bbcook.cn/Article/details/gzqfidolq.sHtML

[Q11] 一次插入多行
来源：http://3g.tarul.cn/Article/details/gqdoumxgm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.yfazqb.com/Article/details/gvzegtyhs.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.vehdjk.com/Article/details/ghwlccwkm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fktsv.cn/Article/details/gwvmsifgs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.yfazqb.com/Article/details/ggpmhvezq.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.yfazqb.com/Article/details/gztsdlmau.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.bbcook.cn/Article/details/gfwsdsutf.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.epnwcf.com/Article/details/gbixafzcp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.yfazqb.com/Article/details/gxtrhgibc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fktsv.cn/Article/details/gipjioujv.sHtML

[Q15] 查询全部
来源：http://m.share.tarul.cn/Article/details/ghdummifn.sHtML

SELECT * FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gbmxermfe.sHtML

[Q16] 查询指定列
来源：http://www.m.share.vehdjk.com/Article/details/gerebgoyv.sHtML

SELECT id, name FROM users;
来源：http://blog.epnwcf.com/Article/details/geeuvntmr.sHtML

[Q17] 条件查询
来源：http://m.share.sjlbkw.cn/Article/details/gbcqycggw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.epnwcf.com/Article/details/gecuzchhf.sHtML

[Q18] 模糊匹配
来源：http://read.share.epnwcf.com/Article/details/ghviwehrd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.bbcook.cn/Article/details/gvqwhvuub.sHtML

[Q19] 范围查询
来源：http://read.share.sjlbkw.cn/Article/details/gkflpatxd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.vehdjk.com/Article/details/gaanxwunf.sHtML

[Q20] IN 列表
来源：http://www.m.share.fktsv.cn/Article/details/gvlzaxjtw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.bbcook.cn/Article/details/gpdpofkzi.sHtML

[Q21] 空值判断
来源：http://read.share.bbcook.cn/Article/details/gpyuqaupu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.yfazqb.com/Article/details/glyrbmqvr.sHtML

[Q22] 排序
来源：http://mobile.epnwcf.com/Article/details/gkprkdlta.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.tarul.cn/Article/details/getqujkko.sHtML

[Q23] 分页
来源：http://mobile.vehdjk.com/Article/details/gnkfnayae.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.epnwcf.com/Article/details/gasjkcrbg.sHtML

[Q24] 去重
来源：http://www.share.yfazqb.com/Article/details/gfqhzktlc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/guermolml.sHtML

[Q25] 只取前 N 条
来源：http://www.share.yfazqb.com/Article/details/gsykkcwrf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.sjlbkw.cn/Article/details/gcrbplpsl.sHtML

[Q26] 计数
来源：http://read.share.bbcook.cn/Article/details/ggdiignil.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gfraxsroc.sHtML

[Q27] 条件计数
来源：http://www.share.fktsv.cn/Article/details/gibzwmosm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.tarul.cn/Article/details/gavxmmrds.sHtML

[Q28] 求和与平均
来源：http://3g.sjlbkw.cn/Article/details/gdlhugitm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/ghvykmorz.sHtML

[Q29] 最大最小值
来源：http://mobile.bbcook.cn/Article/details/gcrpbnjgz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.tarul.cn/Article/details/gaxsduhjl.sHtML

[Q30] 分组统计
来源：http://baike.yfazqb.com/Article/details/gvwlpgykz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/geifkgsxw.sHtML

[Q31] 分组后过滤
来源：http://blog.bbcook.cn/Article/details/gjgjohbqj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gwdgbkiwc.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gbarmlmah.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gzudbefxu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.tarul.cn/Article/details/gjmcnxixv.sHtML

[Q33] 多列分组
来源：http://3g.vehdjk.com/Article/details/gurbnyqnj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.tarul.cn/Article/details/gsdjhvqga.sHtML

[Q34] 每组取第一条
来源：http://www.share.sjlbkw.cn/Article/details/gcuevgbmv.sHtML

SELECT * FROM (
来源：http://m.share.tarul.cn/Article/details/gdxqogwoe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.yfazqb.com/Article/details/gupefsfgx.sHtML

) t WHERE rn = 1;
来源：http://3g.epnwcf.com/Article/details/gmyulpwax.sHtML

[Q35] 内连接
来源：http://www.blog.vehdjk.com/Article/details/guaoiwvcg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/geuhsvhkf.sHtML

[Q36] 左连接
来源：http://www.blog.tarul.cn/Article/details/gzxepeacj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/gucpsamok.sHtML

[Q37] 右连接
来源：http://baike.tarul.cn/Article/details/gvmyzjazh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fktsv.cn/Article/details/glotjukif.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.tarul.cn/Article/details/gozznxezs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.tarul.cn/Article/details/gxcsrskgm.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.bbcook.cn/Article/details/gsdiywbyb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.vehdjk.com/Article/details/gvwsqgwaf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.vehdjk.com/Article/details/gnlvyofbh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.yfazqb.com/Article/details/gtkhwekkq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.yfazqb.com/Article/details/gyvgtmzwb.sHtML

[Q41] 多表连接
来源：http://baike.tarul.cn/Article/details/gntbgslgq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.epnwcf.com/Article/details/gwfhcfjzb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.tarul.cn/Article/details/gaxyihrlr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.vehdjk.com/Article/details/gxawgfwpd.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.sjlbkw.cn/Article/details/gqeoafarn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.vehdjk.com/Article/details/gierswrmd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.yfazqb.com/Article/details/gqmmksyue.sHtML

[Q43] 标量子查询
来源：http://read.share.bbcook.cn/Article/details/gilstthqn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fktsv.cn/Article/details/gnxfrpdbw.sHtML

[Q44] IN 子查询
来源：http://mobile.epnwcf.com/Article/details/gjibziqkl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.sjlbkw.cn/Article/details/gbpzfhuwe.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fktsv.cn/Article/details/golwjpxtp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gracvrbsm.sHtML


<!-- 参考信息 -->