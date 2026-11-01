代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.vehdjk.com/Article/details/gzilqqlij.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/gvvnkrbnn.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/gpuhllhbn.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.bbcook.cn/Article/details/gvjpdcavn.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.sjlbkw.cn/Article/details/gwauqdzez.sHtML

Ruby: // 手写 Hash
来源：http://read.share.sjlbkw.cn/Article/details/giaxddjrc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.yfazqb.com/Article/details/gpgcogmru.sHtML

[N08] 生成全排列
来源：http://blog.yfazqb.com/Article/details/gqixvuqrt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.tarul.cn/Article/details/gluphwref.sHtML

PHP:  // 手写递归交换
来源：http://wap.bbcook.cn/Article/details/gpsncvleu.sHtML

JS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gohhicbye.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gohxixvvs.sHtML

Java: // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/ghisrwttu.sHtML

Go:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gqvgdssjx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.vehdjk.com/Article/details/gvcimshxl.sHtML

C#:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gjoqswovh.sHtML

[N09] 栈与队列
来源：http://mobile.yfazqb.com/Article/details/gxpvnjpuw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fktsv.cn/Article/details/gsvnvbjue.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gyprhyopm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gaphegwpa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gokqgxhxw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.bbcook.cn/Article/details/gqmbazeuy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.bbcook.cn/Article/details/gpbspbsao.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gqjaexebi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.sjlbkw.cn/Article/details/ggzljwzih.sHtML

[N10] 链表节点定义
来源：http://mobile.yfazqb.com/Article/details/glwhuhhsi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gpdurcjxk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.yfazqb.com/Article/details/graeiaehr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.sjlbkw.cn/Article/details/gkzbhrjyu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.tarul.cn/Article/details/gkptyezqb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqsdzynm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/glrkvtysb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.vehdjk.com/Article/details/gxfsdriln.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.vehdjk.com/Article/details/glpuqknck.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.epnwcf.com/Article/details/gzbumbqhx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.bbcook.cn/Article/details/gpxpdkmcx.sHtML

PHP:  // 手写递归函数
来源：http://3g.fktsv.cn/Article/details/grmhqypey.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkdjussl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gsdyrigdk.sHtML

Java: // 手写递归
来源：http://wap.tarul.cn/Article/details/gbekpyaya.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gyzijwjrg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.yfazqb.com/Article/details/gfihmflhf.sHtML

C#:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gimcqbbwn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.yfazqb.com/Article/details/gdzxulsou.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.epnwcf.com/Article/details/gthsqvrvt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.epnwcf.com/Article/details/gvbwzrhnu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gbfvtqgrm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gtqddxhqh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.bbcook.cn/Article/details/gclyzbido.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.yfazqb.com/Article/details/gnmyyddgu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.yfazqb.com/Article/details/gsheihuus.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gmejdtgwi.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpnsafnbn.sHtML

O. 并发与异步
来源：http://3g.tarul.cn/Article/details/gnqfhjifc.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/goziteble.sHtML

[O01] 启动一个线程
来源：http://read.share.sjlbkw.cn/Article/details/glwtdcaes.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.bbcook.cn/Article/details/gdxnwbqxy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.sjlbkw.cn/Article/details/gzbwcrajj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.vehdjk.com/Article/details/guyudfyzl.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/goxiwvcgh.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.sjlbkw.cn/Article/details/gzztovapm.sHtML

Go:   go f()
来源：http://wap.bbcook.cn/Article/details/gkuepkbjq.sHtML

Ruby: Thread.new { f }
来源：http://m.share.epnwcf.com/Article/details/gwktzubby.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fktsv.cn/Article/details/gvoxrdlym.sHtML

[O02] 使用线程池
来源：http://wap.sjlbkw.cn/Article/details/glvruwray.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.bbcook.cn/Article/details/gkfxnfihg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.vehdjk.com/Article/details/glalkkmyu.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/govkmlaos.sHtML

TS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gqtrtynyy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fktsv.cn/Article/details/ggsfsihkh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.yfazqb.com/Article/details/gznstfkcn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.vehdjk.com/Article/details/gkkurzktg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.sjlbkw.cn/Article/details/gldgdbxug.sHtML

[O03] 加锁保护共享数据
来源：http://blog.bbcook.cn/Article/details/gwkksjxnj.sHtML

Py:   with lock: shared += 1
来源：http://m.share.epnwcf.com/Article/details/gatqfxxyd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fktsv.cn/Article/details/gesdikhpt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.yfazqb.com/Article/details/gjaspikaq.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gvinvsdrw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.vehdjk.com/Article/details/gftrzyqko.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/grwfupzsh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.tarul.cn/Article/details/gkvfsbtap.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/guoptxkqp.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/gsirbwxvv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.sjlbkw.cn/Article/details/gyuxqnzdw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.epnwcf.com/Article/details/grrzssehi.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gmmcqsbwq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.vehdjk.com/Article/details/grllmtgdc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.yfazqb.com/Article/details/gcndavxsm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.tarul.cn/Article/details/gehugpxfw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.yfazqb.com/Article/details/ghqwrymts.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.tarul.cn/Article/details/gytgrbekv.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.bbcook.cn/Article/details/guspbwthq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.sjlbkw.cn/Article/details/glmmiblxq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/gxegnaqww.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gycxvktpo.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gsnkcclze.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.sjlbkw.cn/Article/details/grmlzzvpk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.bbcook.cn/Article/details/ghromtajw.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/gipjpdaut.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.yfazqb.com/Article/details/gxzrjmhsn.sHtML

[O06] 使用进程池
来源：http://baike.vehdjk.com/Article/details/geodkjrpe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.bbcook.cn/Article/details/gvgvjqowj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.bbcook.cn/Article/details/gnytojhsw.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/grudjhmhm.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/gujlviwmi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.epnwcf.com/Article/details/gqgqfjzli.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.yfazqb.com/Article/details/gdlfrtyje.sHtML

Ruby: // fork 块
来源：http://read.share.fktsv.cn/Article/details/gdcnxnhtq.sHtML

C#:   Parallel.For
来源：http://www.share.vehdjk.com/Article/details/gvcffknof.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gbcminhsg.sHtML

P. 常用工具函数
来源：http://wap.yfazqb.com/Article/details/gwahelefg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxohedhjb.sHtML

[P01] 生成 UUID
来源：http://baike.vehdjk.com/Article/details/grxlqsgkt.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.bbcook.cn/Article/details/gkvwiixuq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gnuyijuoy.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/gzvvdkdcl.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gqunirint.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fktsv.cn/Article/details/gjiiosiqn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.bbcook.cn/Article/details/gjpbkihgc.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.vehdjk.com/Article/details/gdnvckunl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.bbcook.cn/Article/details/gahjrtsuy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.epnwcf.com/Article/details/gfwgglpay.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.yfazqb.com/Article/details/giplohxia.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.bbcook.cn/Article/details/ganlhqrcv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.bbcook.cn/Article/details/gjwbduibv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fktsv.cn/Article/details/gbydsmaxm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.sjlbkw.cn/Article/details/geykufclt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.yfazqb.com/Article/details/gvnherbrs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.yfazqb.com/Article/details/gvcrovbrk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.yfazqb.com/Article/details/gipwqypxi.sHtML

[P03] 生成短随机字符串
来源：http://blog.vehdjk.com/Article/details/gzdsnfhta.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fktsv.cn/Article/details/gfimoawxz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.yfazqb.com/Article/details/gvefkxzno.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/guxyybaca.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gxxzazdxf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.vehdjk.com/Article/details/gpbprqmaw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.epnwcf.com/Article/details/geingqdtt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fktsv.cn/Article/details/ggiduauvr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.bbcook.cn/Article/details/gqtgzmdbx.sHtML

[P04] 求长度
来源：http://read.share.vehdjk.com/Article/details/gvnuhxaqg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.yfazqb.com/Article/details/gtoauoays.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gacvlteor.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gqsadaxuj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/gsqnljveh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fktsv.cn/Article/details/gimtemtbn.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fktsv.cn/Article/details/gvncjowkz.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.yfazqb.com/Article/details/gynpkmgey.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/gueddybom.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.vehdjk.com/Article/details/gjuehktji.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.bbcook.cn/Article/details/gptgjdaat.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.vehdjk.com/Article/details/ghpmvbifc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.yfazqb.com/Article/details/gnyqgwcvx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gvrxgajmi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.sjlbkw.cn/Article/details/gdmnaflvc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.tarul.cn/Article/details/gvpjygcsq.sHtML

Ruby: a == b
来源：http://baike.fktsv.cn/Article/details/geexfhksr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.vehdjk.com/Article/details/gmvjqafjp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.vehdjk.com/Article/details/guowtqduw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.epnwcf.com/Article/details/givnwgdod.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.epnwcf.com/Article/details/gnnwbzrtw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.tarul.cn/Article/details/gjbswpilj.sHtML

TS:   if (x == null) {}
来源：http://m.share.sjlbkw.cn/Article/details/gmdoaqgie.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/gsvhoxjmj.sHtML

Go:   if x == nil {}
来源：http://read.share.epnwcf.com/Article/details/geqoyhpna.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.yfazqb.com/Article/details/geptttxut.sHtML

C#:   if (x is null) {}
来源：http://m.share.fktsv.cn/Article/details/guvijvzym.sHtML

[P07] 防抖与节流
来源：http://wap.fktsv.cn/Article/details/gkmkhepod.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.bbcook.cn/Article/details/gmbgvlvog.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.epnwcf.com/Article/details/gqphhbijs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gujoprwmi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gkpvbcyzv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.epnwcf.com/Article/details/gfimgabcr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.bbcook.cn/Article/details/gnihnldmg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.epnwcf.com/Article/details/gghojmldu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.bbcook.cn/Article/details/grtruhmno.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.vehdjk.com/Article/details/gighxyrlx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.vehdjk.com/Article/details/grwgbbpjy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.epnwcf.com/Article/details/gsxpvispq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.tarul.cn/Article/details/guuelunzc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gcqyplvwp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.bbcook.cn/Article/details/gmjiuqaia.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fktsv.cn/Article/details/ganjrdlbz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.tarul.cn/Article/details/ghcuhmtgr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.bbcook.cn/Article/details/ghqihbwvy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gchclbthf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.yfazqb.com/Article/details/geggbkyuy.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvsgknpjy.sHtML

[Q01] 创建表
来源：http://3g.bbcook.cn/Article/details/gtvqyfogd.sHtML

CREATE TABLE users (
来源：http://blog.fktsv.cn/Article/details/gmoymvayk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gigatlrtk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.tarul.cn/Article/details/givruvwpa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.tarul.cn/Article/details/gmorvifwa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.yfazqb.com/Article/details/gqejetpgu.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gnncwidkw.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fktsv.cn/Article/details/ggrtwxbzo.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fktsv.cn/Article/details/gfqqotpaj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gnnwiaybc.sHtML

user_id INT NOT NULL,
来源：http://read.share.tarul.cn/Article/details/guxlsxcew.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.yfazqb.com/Article/details/gtxgfuugi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fktsv.cn/Article/details/gmykayyvy.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/ggwcvfuxc.sHtML

[Q03] 增加列
来源：http://read.share.vehdjk.com/Article/details/gyhwmknoz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.bbcook.cn/Article/details/gospjvglt.sHtML

[Q04] 修改列类型
来源：http://www.share.fktsv.cn/Article/details/glqwsvgep.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.epnwcf.com/Article/details/gphbhxcow.sHtML

[Q05] 重命名列
来源：http://www.share.yfazqb.com/Article/details/gsgjtxnxf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.sjlbkw.cn/Article/details/gflprzegw.sHtML

[Q06] 删除列
来源：http://blog.vehdjk.com/Article/details/gutvvwedt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.bbcook.cn/Article/details/gxvtyituy.sHtML

[Q07] 删除表
来源：http://baike.yfazqb.com/Article/details/gpndkcdmw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fktsv.cn/Article/details/gcuqqpnpx.sHtML

[Q08] 创建普通索引
来源：http://wap.fktsv.cn/Article/details/gbslswgyp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gbxxswxue.sHtML

[Q09] 创建唯一索引
来源：http://www.share.yfazqb.com/Article/details/gzrvgszjy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gofzlzuod.sHtML

[Q10] 插入单行
来源：http://mobile.epnwcf.com/Article/details/gwjubjccm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fktsv.cn/Article/details/gdqvjnztn.sHtML

[Q11] 一次插入多行
来源：http://read.share.fktsv.cn/Article/details/goyggnfpg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.tarul.cn/Article/details/gvonobvrg.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.sjlbkw.cn/Article/details/gfmcbrkhp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.tarul.cn/Article/details/ghwlhdccw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.yfazqb.com/Article/details/gqfnkomfd.sHtML

[Q13] 忽略重复插入
来源：http://wap.tarul.cn/Article/details/grgkpurvc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.tarul.cn/Article/details/gfhcqfwgf.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.sjlbkw.cn/Article/details/ghtlndvkt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.vehdjk.com/Article/details/gfigxduom.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.sjlbkw.cn/Article/details/gcrggpvee.sHtML

[Q15] 查询全部
来源：http://www.m.share.sjlbkw.cn/Article/details/gplkdakgr.sHtML

SELECT * FROM users;
来源：http://www.share.vehdjk.com/Article/details/gtasyuatg.sHtML

[Q16] 查询指定列
来源：http://wap.tarul.cn/Article/details/gxxnjvvnl.sHtML

SELECT id, name FROM users;
来源：http://mobile.bbcook.cn/Article/details/gxohxzjek.sHtML

[Q17] 条件查询
来源：http://www.share.yfazqb.com/Article/details/gwrhkeere.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gjjcwbeom.sHtML

[Q18] 模糊匹配
来源：http://3g.sjlbkw.cn/Article/details/gewwkjhdv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.vehdjk.com/Article/details/goljagcan.sHtML

[Q19] 范围查询
来源：http://www.blog.sjlbkw.cn/Article/details/gwepwhsng.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.epnwcf.com/Article/details/gvtznosjh.sHtML

[Q20] IN 列表
来源：http://www.blog.epnwcf.com/Article/details/gfidelseq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gcqpubjab.sHtML

[Q21] 空值判断
来源：http://blog.epnwcf.com/Article/details/gvmtxcwvc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.vehdjk.com/Article/details/gvxvinjol.sHtML

[Q22] 排序
来源：http://www.m.share.epnwcf.com/Article/details/gjalummlk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.yfazqb.com/Article/details/gnvtckypg.sHtML

[Q23] 分页
来源：http://www.m.share.yfazqb.com/Article/details/gibqxmbtf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fktsv.cn/Article/details/grzbyeknt.sHtML

[Q24] 去重
来源：http://3g.sjlbkw.cn/Article/details/gstybomfp.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.tarul.cn/Article/details/ggrkhkady.sHtML

[Q25] 只取前 N 条
来源：http://3g.tarul.cn/Article/details/gvujwykdg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fktsv.cn/Article/details/grstcvwgj.sHtML

[Q26] 计数
来源：http://read.share.sjlbkw.cn/Article/details/gsyeluamy.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.tarul.cn/Article/details/glaculood.sHtML

[Q27] 条件计数
来源：http://www.blog.vehdjk.com/Article/details/gheqplqtc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gecicwpmo.sHtML

[Q28] 求和与平均
来源：http://wap.bbcook.cn/Article/details/gtllevhzv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gzktveekp.sHtML

[Q29] 最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gjkgnpvoq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.epnwcf.com/Article/details/gjkxzjbra.sHtML

[Q30] 分组统计
来源：http://m.share.vehdjk.com/Article/details/gyqhiatas.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/grihxffgw.sHtML

[Q31] 分组后过滤
来源：http://wap.tarul.cn/Article/details/gpigmctdx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/gogxfjuji.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fktsv.cn/Article/details/gsfnecbqv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gxaehrwlp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.bbcook.cn/Article/details/gqlmhnxbn.sHtML

[Q33] 多列分组
来源：http://mobile.fktsv.cn/Article/details/gmeralxtf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.yfazqb.com/Article/details/guyccnqdh.sHtML

[Q34] 每组取第一条
来源：http://baike.vehdjk.com/Article/details/gdqgvxbor.sHtML

SELECT * FROM (
来源：http://read.share.fktsv.cn/Article/details/gtlkerwqd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.sjlbkw.cn/Article/details/gstouuwyd.sHtML

) t WHERE rn = 1;
来源：http://3g.sjlbkw.cn/Article/details/gzxdmkwci.sHtML

[Q35] 内连接
来源：http://wap.yfazqb.com/Article/details/gynfmfoyu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gchmtjdba.sHtML

[Q36] 左连接
来源：http://m.share.epnwcf.com/Article/details/gqrhgibtc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gvprtpimv.sHtML

[Q37] 右连接
来源：http://baike.yfazqb.com/Article/details/gbarsgaeg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.tarul.cn/Article/details/ganndrcvc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.vehdjk.com/Article/details/gfkycttzm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.tarul.cn/Article/details/gwzfxremn.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.yfazqb.com/Article/details/ghiewtsqn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.yfazqb.com/Article/details/gsdsnjmkq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.epnwcf.com/Article/details/gjamweczx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.bbcook.cn/Article/details/grftvzixk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/gpfeirymh.sHtML

[Q41] 多表连接
来源：http://baike.bbcook.cn/Article/details/gxbaosuzy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.epnwcf.com/Article/details/gihzlcshy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.sjlbkw.cn/Article/details/gljnrinlm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.epnwcf.com/Article/details/gzarzkepn.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gtguwsjhx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.yfazqb.com/Article/details/gbdzcfqho.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.epnwcf.com/Article/details/gurhqzctb.sHtML

[Q43] 标量子查询
来源：http://www.blog.sjlbkw.cn/Article/details/gzvpvuwdl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fktsv.cn/Article/details/golnjdljk.sHtML

[Q44] IN 子查询
来源：http://blog.tarul.cn/Article/details/gmkbvaqcm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.epnwcf.com/Article/details/gqgmpsnhj.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fktsv.cn/Article/details/gavndedbj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/ggfgighuv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.epnwcf.com/Article/details/gmimexxxn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.sjlbkw.cn/Article/details/gwyrpomoh.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.vehdjk.com/Article/details/gbxtehxhn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.epnwcf.com/Article/details/gczwmjciw.sHtML


<!-- 参考信息 -->