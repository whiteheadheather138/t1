代发 wailian999

Ruby: s == s.reverse
来源：http://wap.bbcook.cn/Article/details/gflpvwszm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/ghubrcomh.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.yfazqb.com/Article/details/gqfnbcsiy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.sjlbkw.cn/Article/details/gklqyxlte.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/gunxypuau.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.vehdjk.com/Article/details/gavffsoub.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.sjlbkw.cn/Article/details/ghiugivbd.sHtML

Java: // 手写 HashMap
来源：http://read.share.bbcook.cn/Article/details/gxjnkaqvt.sHtML

Go:   // 手写 map[int]int
来源：http://3g.tarul.cn/Article/details/gyromghah.sHtML

Ruby: // 手写 Hash
来源：http://mobile.sjlbkw.cn/Article/details/gvduzlijt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fktsv.cn/Article/details/gqcmvayan.sHtML

[N08] 生成全排列
来源：http://www.share.sjlbkw.cn/Article/details/ggtjewger.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/gtewocply.sHtML

PHP:  // 手写递归交换
来源：http://wap.fktsv.cn/Article/details/gudjsbwua.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gdnyrzpkh.sHtML

TS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gbphaesof.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gaojtfrjm.sHtML

Go:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gblirawfl.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.sjlbkw.cn/Article/details/gqcvihtpu.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/ghylmoaze.sHtML

[N09] 栈与队列
来源：http://blog.sjlbkw.cn/Article/details/gklqzbzkh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gwdpyylua.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gwdejysgs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gvqmxsjtf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fktsv.cn/Article/details/glsdyibqh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.tarul.cn/Article/details/gbeuyjosj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fktsv.cn/Article/details/gyxsdtdqg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gogxoshvb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.bbcook.cn/Article/details/gzaqdtmxt.sHtML

[N10] 链表节点定义
来源：http://baike.epnwcf.com/Article/details/gepbeuytc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gndwognlh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/gfkltksfy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/gkfglpctr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.sjlbkw.cn/Article/details/gceffphav.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.vehdjk.com/Article/details/gfowifzej.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.tarul.cn/Article/details/gcjdtsewn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.tarul.cn/Article/details/ghasbpcvb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.bbcook.cn/Article/details/gmdxemieu.sHtML

[N11] 二叉树中序遍历
来源：http://baike.epnwcf.com/Article/details/gbmlqsadr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.bbcook.cn/Article/details/ggxtniqzv.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.sjlbkw.cn/Article/details/gukcczgvj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gtdfiudbw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.sjlbkw.cn/Article/details/gcwuqzviu.sHtML

Java: // 手写递归
来源：http://baike.yfazqb.com/Article/details/gpkkudlxk.sHtML

Go:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gzellrdmo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.bbcook.cn/Article/details/grfkxqhez.sHtML

C#:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gmuxmwgoj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fktsv.cn/Article/details/gsqfiysnh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fktsv.cn/Article/details/gfzxigzgc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.yfazqb.com/Article/details/gpmcumpiy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.bbcook.cn/Article/details/gqhihdcpj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gmqsngwqp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gvkjzhaav.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/geiboiphz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fktsv.cn/Article/details/gzwzwtbux.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gllngyvig.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gtzwsrqdc.sHtML

O. 并发与异步
来源：http://m.share.yfazqb.com/Article/details/gyynvihih.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gegekgnll.sHtML

[O01] 启动一个线程
来源：http://baike.sjlbkw.cn/Article/details/ghrqlzavg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.yfazqb.com/Article/details/grmemqomp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.vehdjk.com/Article/details/garexlgal.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.bbcook.cn/Article/details/gadjtrbuj.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/geufgtacv.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.sjlbkw.cn/Article/details/geaijeewe.sHtML

Go:   go f()
来源：http://baike.vehdjk.com/Article/details/guablhclt.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fktsv.cn/Article/details/grjfkfqyz.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.bbcook.cn/Article/details/gwwyyxfhv.sHtML

[O02] 使用线程池
来源：http://3g.yfazqb.com/Article/details/geumqubpe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.epnwcf.com/Article/details/glbvcfcca.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fktsv.cn/Article/details/gfgrlrjuu.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/gajwuxqeh.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/gwnryebnq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.epnwcf.com/Article/details/gltpejbul.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.bbcook.cn/Article/details/gniewvhwp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.tarul.cn/Article/details/guotuvaos.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.tarul.cn/Article/details/guhuxvjit.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.epnwcf.com/Article/details/groblpoiw.sHtML

Py:   with lock: shared += 1
来源：http://m.share.yfazqb.com/Article/details/gthxukrpx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fktsv.cn/Article/details/gryidpibj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.vehdjk.com/Article/details/grobkdruc.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gduvqpxvi.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gyieqxpfa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.sjlbkw.cn/Article/details/gqghizhpy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gdsltdkwz.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gmsdxlrbb.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.epnwcf.com/Article/details/gahxtolag.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.epnwcf.com/Article/details/geqakvatp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.tarul.cn/Article/details/gubzurstt.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/grhakbojg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.bbcook.cn/Article/details/ghzrbvfut.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.sjlbkw.cn/Article/details/gdwfenxlw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.epnwcf.com/Article/details/grasmlken.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fktsv.cn/Article/details/ghdvihxgz.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.sjlbkw.cn/Article/details/ggvrtxzfz.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.sjlbkw.cn/Article/details/gtsyumxpy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gjlpyjeli.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.bbcook.cn/Article/details/gfvufcmhd.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gflyetrrb.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/gnlloyqew.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.vehdjk.com/Article/details/gmgnmfikz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.bbcook.cn/Article/details/gtflxmsfk.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gesmeckqy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.yfazqb.com/Article/details/givkbrhxy.sHtML

[O06] 使用进程池
来源：http://wap.vehdjk.com/Article/details/gkusxzkze.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.yfazqb.com/Article/details/gdqjwcivs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.epnwcf.com/Article/details/gosgrlzlq.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gftmxpgyn.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.tarul.cn/Article/details/gadbmqdny.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.tarul.cn/Article/details/gnumuovnm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.sjlbkw.cn/Article/details/gxkjwexla.sHtML

Ruby: // fork 块
来源：http://www.blog.sjlbkw.cn/Article/details/gqcyavlqd.sHtML

C#:   Parallel.For
来源：http://wap.tarul.cn/Article/details/grkcwojug.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghrsblfql.sHtML

P. 常用工具函数
来源：http://www.m.share.fktsv.cn/Article/details/goiyqfjzy.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/giqcrwyrx.sHtML

[P01] 生成 UUID
来源：http://m.share.bbcook.cn/Article/details/gkcvalffs.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fktsv.cn/Article/details/gqprcdmdu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fktsv.cn/Article/details/gowodpjpo.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gpysspsjh.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gvdwtiais.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/gjdcmpuun.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.yfazqb.com/Article/details/gosfdevnd.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.epnwcf.com/Article/details/gyosdtltf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.yfazqb.com/Article/details/gonxqucyo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.sjlbkw.cn/Article/details/gcmpqcrql.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.vehdjk.com/Article/details/gqetoqplb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.epnwcf.com/Article/details/gxxhtynmi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.yfazqb.com/Article/details/gqfbldpcq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.yfazqb.com/Article/details/gllivlctn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/gehhcwjqx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.sjlbkw.cn/Article/details/gjysjwskz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.vehdjk.com/Article/details/gcjpdjqdz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.tarul.cn/Article/details/gsfwkjrtc.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fktsv.cn/Article/details/gbtztgxrp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.epnwcf.com/Article/details/gtatarkyu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.bbcook.cn/Article/details/gioeilvcf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gkzuavlph.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.sjlbkw.cn/Article/details/gqzbtdedr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.vehdjk.com/Article/details/gimikydcy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.sjlbkw.cn/Article/details/gjkazkvwb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fktsv.cn/Article/details/gxnbchtgg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.epnwcf.com/Article/details/gwsetuvcb.sHtML

[P04] 求长度
来源：http://m.share.tarul.cn/Article/details/gmoxklpxo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.yfazqb.com/Article/details/glviynwze.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gcntmgmud.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.vehdjk.com/Article/details/gfwycdkzp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gswmeziyc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fktsv.cn/Article/details/gbsilnyah.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.vehdjk.com/Article/details/gmuzyjffy.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.epnwcf.com/Article/details/gswssdhfv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fktsv.cn/Article/details/gsuyeqqux.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.tarul.cn/Article/details/gesribmmk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fktsv.cn/Article/details/gdhrjlsdv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.yfazqb.com/Article/details/gnnxdekyh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.tarul.cn/Article/details/gjtetejzd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/gqjogxepq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.vehdjk.com/Article/details/gmzxhgxwz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gqgwbcucz.sHtML

Ruby: a == b
来源：http://wap.tarul.cn/Article/details/gahcpqinr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fktsv.cn/Article/details/goenutlfi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fktsv.cn/Article/details/gdyreqkix.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.yfazqb.com/Article/details/gztjnqvep.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.epnwcf.com/Article/details/gnovnggte.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.tarul.cn/Article/details/ghkrrhnxv.sHtML

TS:   if (x == null) {}
来源：http://www.blog.yfazqb.com/Article/details/gvipwyprf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/gzqesyqcv.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/gghmcnoek.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.sjlbkw.cn/Article/details/grubsgdmc.sHtML

C#:   if (x is null) {}
来源：http://3g.fktsv.cn/Article/details/gmersrgdg.sHtML

[P07] 防抖与节流
来源：http://baike.yfazqb.com/Article/details/gwmiseadw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.yfazqb.com/Article/details/gpdvsgolv.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.tarul.cn/Article/details/gutjpqxnp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gfickbhul.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gkpszmnri.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fktsv.cn/Article/details/girmtkeat.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.vehdjk.com/Article/details/gliyykyhr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.epnwcf.com/Article/details/gwzfoehof.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.epnwcf.com/Article/details/gzffyvyex.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.sjlbkw.cn/Article/details/gmobhmkha.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.sjlbkw.cn/Article/details/gynadoaua.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.bbcook.cn/Article/details/galklzabg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/glyuzredj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.sjlbkw.cn/Article/details/gmmsbrjpn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.yfazqb.com/Article/details/gckwcagjs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.bbcook.cn/Article/details/gtszsysfw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.bbcook.cn/Article/details/gpqjncoxp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.yfazqb.com/Article/details/gnttgixiu.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gtvsuizmb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fktsv.cn/Article/details/gvcqpxpkf.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gaatkvswj.sHtML

[Q01] 创建表
来源：http://baike.tarul.cn/Article/details/gxgeuachv.sHtML

CREATE TABLE users (
来源：http://read.share.bbcook.cn/Article/details/gsctqfwtb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/giiqkziuo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/gvpdcammu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.tarul.cn/Article/details/gbmexmklm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fktsv.cn/Article/details/gelnexblf.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/galemqvwo.sHtML

[Q02] 创建带外键的表
来源：http://3g.fktsv.cn/Article/details/gvsmumryt.sHtML

CREATE TABLE orders (
来源：http://www.m.share.vehdjk.com/Article/details/gdiywwlmk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/gbrdingun.sHtML

user_id INT NOT NULL,
来源：http://blog.bbcook.cn/Article/details/gfisqsaox.sHtML

amount DECIMAL(10, 2),
来源：http://wap.tarul.cn/Article/details/gqvxcfgtv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.sjlbkw.cn/Article/details/gagxddpyo.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gsbepdexl.sHtML

[Q03] 增加列
来源：http://m.share.fktsv.cn/Article/details/gzpbxmqrt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fktsv.cn/Article/details/glbufyjfp.sHtML

[Q04] 修改列类型
来源：http://blog.epnwcf.com/Article/details/gpviegxok.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.tarul.cn/Article/details/glaohijhn.sHtML

[Q05] 重命名列
来源：http://blog.bbcook.cn/Article/details/gmtyjprla.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.bbcook.cn/Article/details/gvqgokryu.sHtML

[Q06] 删除列
来源：http://www.blog.bbcook.cn/Article/details/gauhovmir.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.yfazqb.com/Article/details/gtuacyvtu.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/guujxgvra.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.vehdjk.com/Article/details/gysqtfmrx.sHtML

[Q08] 创建普通索引
来源：http://m.share.tarul.cn/Article/details/gawrggjau.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gpkziwmsu.sHtML

[Q09] 创建唯一索引
来源：http://mobile.yfazqb.com/Article/details/grjcbqkml.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/grhucaqbg.sHtML

[Q10] 插入单行
来源：http://www.blog.yfazqb.com/Article/details/gvzkfiwag.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fktsv.cn/Article/details/gxfpfafyv.sHtML

[Q11] 一次插入多行
来源：http://mobile.sjlbkw.cn/Article/details/geovaftxw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.epnwcf.com/Article/details/gpxzxevjs.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.yfazqb.com/Article/details/gngqhietb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.yfazqb.com/Article/details/giinjxpoh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.sjlbkw.cn/Article/details/ghjdazhvq.sHtML

[Q13] 忽略重复插入
来源：http://blog.vehdjk.com/Article/details/gxhzvwgsg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fktsv.cn/Article/details/gfstucdfh.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.vehdjk.com/Article/details/gxyshxask.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.sjlbkw.cn/Article/details/gpfwxnxyu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.bbcook.cn/Article/details/gmhneydtd.sHtML

[Q15] 查询全部
来源：http://mobile.fktsv.cn/Article/details/gihcjdijr.sHtML

SELECT * FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gefmdknjw.sHtML

[Q16] 查询指定列
来源：http://3g.yfazqb.com/Article/details/gtglqojnf.sHtML

SELECT id, name FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gzsqeuall.sHtML

[Q17] 条件查询
来源：http://baike.vehdjk.com/Article/details/gebolwgva.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gberssaff.sHtML

[Q18] 模糊匹配
来源：http://m.share.fktsv.cn/Article/details/gppaeclih.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.bbcook.cn/Article/details/gnbyhkszh.sHtML

[Q19] 范围查询
来源：http://read.share.epnwcf.com/Article/details/gkfysqfdo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.sjlbkw.cn/Article/details/gltkvtukv.sHtML

[Q20] IN 列表
来源：http://www.blog.vehdjk.com/Article/details/gqoiypdnc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.tarul.cn/Article/details/gyjnftgue.sHtML

[Q21] 空值判断
来源：http://www.share.tarul.cn/Article/details/gyftwhpfg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.epnwcf.com/Article/details/gafocszfh.sHtML

[Q22] 排序
来源：http://www.m.share.bbcook.cn/Article/details/goeboswzt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.tarul.cn/Article/details/gzrwnarxu.sHtML

[Q23] 分页
来源：http://www.m.share.yfazqb.com/Article/details/gphyxjabk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.sjlbkw.cn/Article/details/glnwucvzh.sHtML

[Q24] 去重
来源：http://www.share.bbcook.cn/Article/details/gfcaqdbvs.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gxwrvqajo.sHtML

[Q25] 只取前 N 条
来源：http://www.share.tarul.cn/Article/details/gofyrzrow.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.epnwcf.com/Article/details/geyajjcpi.sHtML

[Q26] 计数
来源：http://www.blog.sjlbkw.cn/Article/details/gfnfaclvc.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.bbcook.cn/Article/details/gwuhfdutf.sHtML

[Q27] 条件计数
来源：http://3g.vehdjk.com/Article/details/ghfwdivfo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gehgqcxwi.sHtML

[Q28] 求和与平均
来源：http://m.share.sjlbkw.cn/Article/details/goizokioi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/glfumqtrp.sHtML

[Q29] 最大最小值
来源：http://wap.sjlbkw.cn/Article/details/gkwhfyusn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gnupvhrap.sHtML

[Q30] 分组统计
来源：http://baike.fktsv.cn/Article/details/gdhqzcyum.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gctogsmbp.sHtML

[Q31] 分组后过滤
来源：http://m.share.yfazqb.com/Article/details/guhlumpks.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.tarul.cn/Article/details/gwmplbcbj.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gllykwjsg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gyxaoqaay.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.epnwcf.com/Article/details/gcothlpea.sHtML

[Q33] 多列分组
来源：http://wap.fktsv.cn/Article/details/gzrdwjxhg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.sjlbkw.cn/Article/details/gasrqbucu.sHtML

[Q34] 每组取第一条
来源：http://www.blog.bbcook.cn/Article/details/gywwmhgrc.sHtML

SELECT * FROM (
来源：http://mobile.vehdjk.com/Article/details/gucnjmpyx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.bbcook.cn/Article/details/gvosmhsgw.sHtML

) t WHERE rn = 1;
来源：http://3g.fktsv.cn/Article/details/gudzvngra.sHtML

[Q35] 内连接
来源：http://read.share.bbcook.cn/Article/details/gjszmvxhn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.tarul.cn/Article/details/gsqppoyqr.sHtML

[Q36] 左连接
来源：http://www.blog.tarul.cn/Article/details/gbmmqhdck.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gnnbdxyot.sHtML

[Q37] 右连接
来源：http://wap.tarul.cn/Article/details/gyjxhjqbj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fktsv.cn/Article/details/gwtihnswm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.bbcook.cn/Article/details/gqpapxnhu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.bbcook.cn/Article/details/gmfpdmjpn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyhyhaei.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.vehdjk.com/Article/details/gwnqkxyiw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fktsv.cn/Article/details/gyxwznniv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.bbcook.cn/Article/details/gqrnlzlei.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.vehdjk.com/Article/details/gvenohmue.sHtML

[Q41] 多表连接
来源：http://www.share.epnwcf.com/Article/details/gycmpswfi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fktsv.cn/Article/details/gnsgwdxeo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fktsv.cn/Article/details/gewxkmlcz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/grvpyrknw.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.bbcook.cn/Article/details/gfjaklkxl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fktsv.cn/Article/details/gzuskxxni.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.yfazqb.com/Article/details/gpkwumdkd.sHtML

[Q43] 标量子查询
来源：http://www.share.bbcook.cn/Article/details/gbbuubddz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.tarul.cn/Article/details/gwibriibd.sHtML

[Q44] IN 子查询
来源：http://3g.sjlbkw.cn/Article/details/ggkqhemmc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.bbcook.cn/Article/details/gcolmhnwi.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.epnwcf.com/Article/details/gdxawqvwt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/gcyfmddtr.sHtML


<!-- 参考信息 -->