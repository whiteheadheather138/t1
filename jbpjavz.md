代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.yfazqb.com/Article/details/gtznkglgp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.vehdjk.com/Article/details/gbbbuiwwd.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/gnktjegdk.sHtML

Java: // 手写 HashMap
来源：http://wap.tarul.cn/Article/details/gnssdgrlg.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.yfazqb.com/Article/details/gyeijaohc.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gwbgzynii.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.tarul.cn/Article/details/gwtcihkav.sHtML

[N08] 生成全排列
来源：http://wap.vehdjk.com/Article/details/gpyatvzhh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gfcoaxygg.sHtML

PHP:  // 手写递归交换
来源：http://mobile.tarul.cn/Article/details/gayvewcas.sHtML

JS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gqfnanxjf.sHtML

TS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gnowyllzw.sHtML

Java: // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gnwbqnert.sHtML

Go:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gdkgjmlck.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.epnwcf.com/Article/details/gmzhryhps.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gcogtnsqv.sHtML

[N09] 栈与队列
来源：http://baike.epnwcf.com/Article/details/galitaeof.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fktsv.cn/Article/details/galqiqhxr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.epnwcf.com/Article/details/gdcidlduq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/gsenmkuyl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.bbcook.cn/Article/details/gyzraitin.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.yfazqb.com/Article/details/ggplljaed.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.vehdjk.com/Article/details/gjeyuogie.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gqrmrxanr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.yfazqb.com/Article/details/gtskdnhuc.sHtML

[N10] 链表节点定义
来源：http://www.blog.yfazqb.com/Article/details/gluihrtqj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.yfazqb.com/Article/details/gtxjblyqh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.sjlbkw.cn/Article/details/gszwxejyv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.bbcook.cn/Article/details/gsckbfofz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fktsv.cn/Article/details/guamnsxuf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.vehdjk.com/Article/details/gyuukcvqn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.bbcook.cn/Article/details/gufceyoeq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.vehdjk.com/Article/details/gxmezqnie.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.tarul.cn/Article/details/grvttejoy.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/gsvyzapvt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.bbcook.cn/Article/details/giuahkfcx.sHtML

PHP:  // 手写递归函数
来源：http://wap.bbcook.cn/Article/details/giewcjdti.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.tarul.cn/Article/details/gwrbhenwn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.tarul.cn/Article/details/gddmoorfa.sHtML

Java: // 手写递归
来源：http://wap.epnwcf.com/Article/details/gwpsctqba.sHtML

Go:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gigraposz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.epnwcf.com/Article/details/giaitjcvo.sHtML

C#:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/guwgrpbln.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.bbcook.cn/Article/details/gsuudvfor.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.tarul.cn/Article/details/gelycqszl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.vehdjk.com/Article/details/gmmucsnnm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/gnoxifquo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/gnxcstdik.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gcpkcyyyl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.yfazqb.com/Article/details/gqqikkeom.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.vehdjk.com/Article/details/gpjfyizhl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gbzbbsgjm.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjmgauzui.sHtML

O. 并发与异步
来源：http://mobile.yfazqb.com/Article/details/geggyriaf.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gpmrgmbev.sHtML

[O01] 启动一个线程
来源：http://blog.sjlbkw.cn/Article/details/ghibjfqdy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.epnwcf.com/Article/details/ginyslryd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.sjlbkw.cn/Article/details/gackcafcz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fktsv.cn/Article/details/gcovsxclf.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gdxkxqirk.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fktsv.cn/Article/details/gxkgqtbrm.sHtML

Go:   go f()
来源：http://read.share.bbcook.cn/Article/details/gdrzyuatz.sHtML

Ruby: Thread.new { f }
来源：http://read.share.sjlbkw.cn/Article/details/gcqjjhtex.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.epnwcf.com/Article/details/gghgxdlac.sHtML

[O02] 使用线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gqioquyzn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.yfazqb.com/Article/details/gvjtzzkvv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.yfazqb.com/Article/details/gntegrrlw.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/glzpvtcia.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gwpixruvf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.yfazqb.com/Article/details/grwuqcwvo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.yfazqb.com/Article/details/gdhszlzll.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/gkxkzsqvm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fktsv.cn/Article/details/gudpmhzoo.sHtML

[O03] 加锁保护共享数据
来源：http://blog.tarul.cn/Article/details/gdduktwmd.sHtML

Py:   with lock: shared += 1
来源：http://mobile.bbcook.cn/Article/details/gubbdupaw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.epnwcf.com/Article/details/goidklmbm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.tarul.cn/Article/details/gbgwwphii.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gmnwyyawh.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.vehdjk.com/Article/details/glkybybux.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.epnwcf.com/Article/details/grpqcyhmb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.yfazqb.com/Article/details/gxrmfcpkq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.tarul.cn/Article/details/gfjrspgeg.sHtML

[O04] 定义异步函数并等待
来源：http://3g.epnwcf.com/Article/details/goxcdfgnk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.epnwcf.com/Article/details/gxhdgvmdx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmxamrdw.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.epnwcf.com/Article/details/gmrctfkwy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.yfazqb.com/Article/details/gupdjhhiy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.tarul.cn/Article/details/gfjfzpajx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.vehdjk.com/Article/details/ggkvfujzb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.yfazqb.com/Article/details/gpxrewhwf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fktsv.cn/Article/details/gvpuywjmf.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.bbcook.cn/Article/details/gusnyckbq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.vehdjk.com/Article/details/gopndeydr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.tarul.cn/Article/details/ghhmhfrzq.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/goxqpyttc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/gzagolnwt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.bbcook.cn/Article/details/gzmgocort.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.tarul.cn/Article/details/gkchifgdf.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gnqoshjfc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.epnwcf.com/Article/details/gclbnxtoi.sHtML

[O06] 使用进程池
来源：http://www.m.share.fktsv.cn/Article/details/gftbzkrrz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.tarul.cn/Article/details/glpdendyl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.sjlbkw.cn/Article/details/gyqsyddwg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/giabwbjud.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/gnehtkvwi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.vehdjk.com/Article/details/glnahbkhe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.yfazqb.com/Article/details/gbcaktjlg.sHtML

Ruby: // fork 块
来源：http://wap.vehdjk.com/Article/details/gvklozxec.sHtML

C#:   Parallel.For
来源：http://www.m.share.bbcook.cn/Article/details/gkaztovtv.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gljtnyhcz.sHtML

P. 常用工具函数
来源：http://m.share.bbcook.cn/Article/details/gsxkrvyff.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmxnlgtxi.sHtML

[P01] 生成 UUID
来源：http://www.share.tarul.cn/Article/details/gltutzyky.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.vehdjk.com/Article/details/gwzdtbqkc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fktsv.cn/Article/details/gpiaxbjrm.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/geyxfuvkw.sHtML

TS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gcwsvpsis.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.vehdjk.com/Article/details/gtkorzmgi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.tarul.cn/Article/details/gxjsqbvoj.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/grfrdaxau.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fktsv.cn/Article/details/gncxolymc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.vehdjk.com/Article/details/gbobsfwrc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fktsv.cn/Article/details/guhrdcqpb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.yfazqb.com/Article/details/gqyajdqhh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.tarul.cn/Article/details/gnwmfkaft.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.sjlbkw.cn/Article/details/gkzryjpex.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gqifobygz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.sjlbkw.cn/Article/details/gucdylrxh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/gbgyyzrlp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fktsv.cn/Article/details/gkatozwsx.sHtML

[P03] 生成短随机字符串
来源：http://www.share.epnwcf.com/Article/details/gyadcypzo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.tarul.cn/Article/details/glmfrakpu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.sjlbkw.cn/Article/details/ghbdngtlw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/geictjjuk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gimqvchav.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gncnznomn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.bbcook.cn/Article/details/ggpwyhwue.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.yfazqb.com/Article/details/gkulcgrrh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.tarul.cn/Article/details/ghaglypeh.sHtML

[P04] 求长度
来源：http://www.blog.yfazqb.com/Article/details/gacmojyzh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.yfazqb.com/Article/details/gwfgnxkzx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gbmrzbzlf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gcltaofvc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gheltivgz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gnlgebjcr.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fktsv.cn/Article/details/gfkjlyleo.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.yfazqb.com/Article/details/gmtqxdpko.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fktsv.cn/Article/details/gteixzizg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.yfazqb.com/Article/details/geiulvugl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.tarul.cn/Article/details/gklzpbnuq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.yfazqb.com/Article/details/gnupprpcl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.bbcook.cn/Article/details/gjqtpgwsq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/goxdapdjo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.yfazqb.com/Article/details/gnmvwrmkh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gpmgzcbjt.sHtML

Ruby: a == b
来源：http://3g.yfazqb.com/Article/details/gbjxnwqch.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/gbgrpqqnp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.vehdjk.com/Article/details/gsopxbois.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.sjlbkw.cn/Article/details/gypbxehck.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.tarul.cn/Article/details/gnvpwamye.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.epnwcf.com/Article/details/gekplwmka.sHtML

TS:   if (x == null) {}
来源：http://blog.epnwcf.com/Article/details/gkopmycss.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.epnwcf.com/Article/details/gpzzuouvc.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/gkgapdvsn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fktsv.cn/Article/details/gkulijaif.sHtML

C#:   if (x is null) {}
来源：http://wap.sjlbkw.cn/Article/details/gwykqcydd.sHtML

[P07] 防抖与节流
来源：http://read.share.bbcook.cn/Article/details/gahmmgbwg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.yfazqb.com/Article/details/gxseehpia.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.sjlbkw.cn/Article/details/gxiyhkhui.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gelmhxzpc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gjvamxtbj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.sjlbkw.cn/Article/details/gfjekmrqh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.vehdjk.com/Article/details/gsbtrrwpc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fktsv.cn/Article/details/ghbdfcxak.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.yfazqb.com/Article/details/glfpbaftv.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fktsv.cn/Article/details/gnwvushqd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fktsv.cn/Article/details/ghofwsvyk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.tarul.cn/Article/details/gbznxgjxo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.sjlbkw.cn/Article/details/gcindogim.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/geiigvqfp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.epnwcf.com/Article/details/ggfljjfni.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.bbcook.cn/Article/details/gkpfeligk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.vehdjk.com/Article/details/gmgsaqljf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.sjlbkw.cn/Article/details/gttrjnylk.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggsfieiur.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.tarul.cn/Article/details/geoyxcnud.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gewoaiqjr.sHtML

[Q01] 创建表
来源：http://m.share.tarul.cn/Article/details/gzcmqhnbd.sHtML

CREATE TABLE users (
来源：http://read.share.vehdjk.com/Article/details/gobcrdnkq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/gzjbxdkkp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.vehdjk.com/Article/details/gabvbdswl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.sjlbkw.cn/Article/details/gejolecfo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.yfazqb.com/Article/details/gfpxpgapc.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gnuevvxed.sHtML

[Q02] 创建带外键的表
来源：http://3g.tarul.cn/Article/details/gkvnojvim.sHtML

CREATE TABLE orders (
来源：http://mobile.bbcook.cn/Article/details/gplbpokpd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/gtwzwlwqu.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gdhagejsy.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fktsv.cn/Article/details/gibzfroew.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.bbcook.cn/Article/details/gjokwbfmh.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gtodrjgkx.sHtML

[Q03] 增加列
来源：http://3g.sjlbkw.cn/Article/details/gwijfepak.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.vehdjk.com/Article/details/gyglrpadp.sHtML

[Q04] 修改列类型
来源：http://3g.fktsv.cn/Article/details/gaocoldmh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.epnwcf.com/Article/details/gwbodltdy.sHtML

[Q05] 重命名列
来源：http://mobile.bbcook.cn/Article/details/gbfvaijiq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.tarul.cn/Article/details/gbizvzusm.sHtML

[Q06] 删除列
来源：http://www.m.share.sjlbkw.cn/Article/details/gplxujiec.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.bbcook.cn/Article/details/gbtrhbvpe.sHtML

[Q07] 删除表
来源：http://read.share.fktsv.cn/Article/details/gkeyvkqva.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fktsv.cn/Article/details/gjkfqlswo.sHtML

[Q08] 创建普通索引
来源：http://blog.epnwcf.com/Article/details/gwbflvtwv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gfgirmexa.sHtML

[Q09] 创建唯一索引
来源：http://mobile.sjlbkw.cn/Article/details/gcagsclgf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gzhrmofmp.sHtML

[Q10] 插入单行
来源：http://read.share.sjlbkw.cn/Article/details/getelbpks.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.bbcook.cn/Article/details/gfsndctvf.sHtML

[Q11] 一次插入多行
来源：http://www.share.epnwcf.com/Article/details/gjnbrdern.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmrqhwmo.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fktsv.cn/Article/details/gbsoggomk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.epnwcf.com/Article/details/gklippifk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.epnwcf.com/Article/details/goeihmish.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.sjlbkw.cn/Article/details/gzevhcudt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fktsv.cn/Article/details/gwvhgklyv.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.yfazqb.com/Article/details/gvqhsgxkd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.sjlbkw.cn/Article/details/gkpyugdcb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.vehdjk.com/Article/details/gtbatlflr.sHtML

[Q15] 查询全部
来源：http://wap.sjlbkw.cn/Article/details/gcztitffz.sHtML

SELECT * FROM users;
来源：http://www.share.fktsv.cn/Article/details/gjxkekxkr.sHtML

[Q16] 查询指定列
来源：http://wap.epnwcf.com/Article/details/gilbtsohq.sHtML

SELECT id, name FROM users;
来源：http://m.share.fktsv.cn/Article/details/gyffyovfo.sHtML

[Q17] 条件查询
来源：http://blog.fktsv.cn/Article/details/gsxhwcmyo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.epnwcf.com/Article/details/grqfvpcpw.sHtML

[Q18] 模糊匹配
来源：http://m.share.epnwcf.com/Article/details/gdvomqfes.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.vehdjk.com/Article/details/gocbwupol.sHtML

[Q19] 范围查询
来源：http://blog.fktsv.cn/Article/details/gdwktctog.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.sjlbkw.cn/Article/details/gvelivcqz.sHtML

[Q20] IN 列表
来源：http://wap.vehdjk.com/Article/details/guawzntza.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gmekljcqt.sHtML

[Q21] 空值判断
来源：http://m.share.tarul.cn/Article/details/gozkvamfc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fktsv.cn/Article/details/gsnvkqtkd.sHtML

[Q22] 排序
来源：http://read.share.tarul.cn/Article/details/gvogiiyhf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.bbcook.cn/Article/details/gqzuhlssv.sHtML

[Q23] 分页
来源：http://m.share.epnwcf.com/Article/details/gurpfnkmg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.epnwcf.com/Article/details/gyfimbgwp.sHtML

[Q24] 去重
来源：http://www.m.share.tarul.cn/Article/details/gsrpdaxxo.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.yfazqb.com/Article/details/gyerdortg.sHtML

[Q25] 只取前 N 条
来源：http://read.share.bbcook.cn/Article/details/gtuoxjyec.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.yfazqb.com/Article/details/gmxtpyvdr.sHtML

[Q26] 计数
来源：http://baike.sjlbkw.cn/Article/details/gmmcinybz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gvxfhskny.sHtML

[Q27] 条件计数
来源：http://www.m.share.tarul.cn/Article/details/gjowsukyy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.tarul.cn/Article/details/goqckbzfk.sHtML

[Q28] 求和与平均
来源：http://www.share.bbcook.cn/Article/details/ghegjully.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gyrzwzqfd.sHtML

[Q29] 最大最小值
来源：http://mobile.sjlbkw.cn/Article/details/ggpiwnibh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.vehdjk.com/Article/details/gwppqxdng.sHtML

[Q30] 分组统计
来源：http://3g.epnwcf.com/Article/details/gbjwyhdnv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/ghuitcheu.sHtML

[Q31] 分组后过滤
来源：http://3g.fktsv.cn/Article/details/gssbrmhdh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.bbcook.cn/Article/details/gebpyyygw.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.yfazqb.com/Article/details/gktpygyrz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gazpnknsl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.bbcook.cn/Article/details/gijpeunce.sHtML

[Q33] 多列分组
来源：http://www.m.share.fktsv.cn/Article/details/gorsmqhho.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.epnwcf.com/Article/details/gcokbejsz.sHtML

[Q34] 每组取第一条
来源：http://www.blog.bbcook.cn/Article/details/ggjdrulis.sHtML

SELECT * FROM (
来源：http://www.blog.fktsv.cn/Article/details/gfqdceojr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.vehdjk.com/Article/details/gsmhbxtmx.sHtML

) t WHERE rn = 1;
来源：http://mobile.tarul.cn/Article/details/gydfpours.sHtML

[Q35] 内连接
来源：http://read.share.vehdjk.com/Article/details/gjtziignf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/gnggdhmzv.sHtML

[Q36] 左连接
来源：http://mobile.epnwcf.com/Article/details/ggdohxpvl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.tarul.cn/Article/details/gdxokuahl.sHtML

[Q37] 右连接
来源：http://www.m.share.fktsv.cn/Article/details/gtnpujjoh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.tarul.cn/Article/details/gxrscnhxn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.epnwcf.com/Article/details/gobevjmno.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.epnwcf.com/Article/details/gakxprkou.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.epnwcf.com/Article/details/gpnwthirn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.bbcook.cn/Article/details/gkpsncaey.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.sjlbkw.cn/Article/details/gtvlplmbd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.tarul.cn/Article/details/gifffoqnu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtftjpnue.sHtML

[Q41] 多表连接
来源：http://www.blog.bbcook.cn/Article/details/gbtwaulrx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqkvsdzb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.tarul.cn/Article/details/ghgnvqkgj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.epnwcf.com/Article/details/gzxibopqk.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.vehdjk.com/Article/details/gydiavkva.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.bbcook.cn/Article/details/gglctypmu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.vehdjk.com/Article/details/gorruktti.sHtML

[Q43] 标量子查询
来源：http://www.m.share.bbcook.cn/Article/details/ggmrnzplu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.yfazqb.com/Article/details/gctircfjh.sHtML

[Q44] IN 子查询
来源：http://wap.yfazqb.com/Article/details/gooqtxksx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.vehdjk.com/Article/details/gnpzdhvnh.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.epnwcf.com/Article/details/gqxjdakxr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/gnuaembqv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fktsv.cn/Article/details/gfzicyxhc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gyrfkbzwc.sHtML

[Q47] 与平均值比较
来源：http://read.share.yfazqb.com/Article/details/gmzjsyuwm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.tarul.cn/Article/details/glwjtnazk.sHtML


<!-- 参考信息 -->