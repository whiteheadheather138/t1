代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.epnwcf.com/Article/details/gfmryafhk.sHtML

[N06] 判断回文字符串
来源：http://baike.epnwcf.com/Article/details/gakhfomjo.sHtML

Py:   s == s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/gpsgpievh.sHtML

PHP:  $s === strrev($s);
来源：http://3g.epnwcf.com/Article/details/gyixifilg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gomuprdgs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gczbqvgqf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fktsv.cn/Article/details/gfkkqhapq.sHtML

Go:   // 双指针从两端比较
来源：http://wap.sjlbkw.cn/Article/details/gouzxfphe.sHtML

Ruby: s == s.reverse
来源：http://wap.epnwcf.com/Article/details/goeckbeht.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gcygcyqmv.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.epnwcf.com/Article/details/gxzhjrhez.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.tarul.cn/Article/details/gwhogmytz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.vehdjk.com/Article/details/giulmxzrj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fktsv.cn/Article/details/gvgujfjyq.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.vehdjk.com/Article/details/gpxvfqkwl.sHtML

Java: // 手写 HashMap
来源：http://baike.epnwcf.com/Article/details/glnmpsios.sHtML

Go:   // 手写 map[int]int
来源：http://blog.vehdjk.com/Article/details/ggjthqklx.sHtML

Ruby: // 手写 Hash
来源：http://m.share.sjlbkw.cn/Article/details/gsmpfpzao.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fktsv.cn/Article/details/gkkkylxla.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/gixcubyhr.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fktsv.cn/Article/details/gtxahobqc.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/gfuhebutp.sHtML

JS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gfodfwmxb.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gmovfdkse.sHtML

Java: // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gudfzdagw.sHtML

Go:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gufghpmym.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.vehdjk.com/Article/details/goegmkbqd.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gffuhuezu.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/gqhjarncm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.tarul.cn/Article/details/gffovxtrh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gnyxvpjzl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/ghmarwlau.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.tarul.cn/Article/details/gtsjrbjar.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gytzvnaee.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.vehdjk.com/Article/details/gumszlkiu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gogrplufd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.epnwcf.com/Article/details/gmlutuhff.sHtML

[N10] 链表节点定义
来源：http://m.share.yfazqb.com/Article/details/gsgpasmgm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.epnwcf.com/Article/details/gtdlqygsp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.yfazqb.com/Article/details/gjuwxbmeq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.vehdjk.com/Article/details/gdefiakgn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.sjlbkw.cn/Article/details/ggjbxrjyd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.epnwcf.com/Article/details/gnxamuvuz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fktsv.cn/Article/details/gvgzestve.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.vehdjk.com/Article/details/grcsavckp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.yfazqb.com/Article/details/grqrkthcr.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/gixzajguv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.sjlbkw.cn/Article/details/gqpprkxhm.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fktsv.cn/Article/details/gwvlcusbf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gsavathhl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gwewioqap.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/gcxshxlqm.sHtML

Go:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gloscesbs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.bbcook.cn/Article/details/gdyaispic.sHtML

C#:   // 手写递归
来源：http://wap.tarul.cn/Article/details/guvorjytr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.tarul.cn/Article/details/gublimpan.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.vehdjk.com/Article/details/gopicexpi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.sjlbkw.cn/Article/details/grrsiovlf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gkxexaykb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/ggvavkcjg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gqjeeizuj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.bbcook.cn/Article/details/gidtvrfwu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gvicfkwqj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.bbcook.cn/Article/details/gydylztta.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gqpzxtkan.sHtML

O. 并发与异步
来源：http://blog.tarul.cn/Article/details/gjcwpsqtz.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkpaovhzf.sHtML

[O01] 启动一个线程
来源：http://www.m.share.vehdjk.com/Article/details/gpyagfoam.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.bbcook.cn/Article/details/gtibzpeva.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.yfazqb.com/Article/details/guckqujun.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.epnwcf.com/Article/details/gdvotzisi.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gcpxhsxbz.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.sjlbkw.cn/Article/details/gbehhmxva.sHtML

Go:   go f()
来源：http://www.blog.bbcook.cn/Article/details/gfnwtbczl.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.yfazqb.com/Article/details/gkkxijlwk.sHtML

C#:   Task.Run(() => F());
来源：http://wap.vehdjk.com/Article/details/ggaeqtspc.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/gvvbooksc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.sjlbkw.cn/Article/details/gofpvldms.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.tarul.cn/Article/details/guyxmbtbu.sHtML

JS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gcszugvyd.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.yfazqb.com/Article/details/gtirsmfyp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.tarul.cn/Article/details/gxzhblofw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.tarul.cn/Article/details/gwtnhhvbz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnirhnov.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fktsv.cn/Article/details/ggoopdcct.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.yfazqb.com/Article/details/gpqttwawy.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/gdosilxir.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fktsv.cn/Article/details/gvwxbvrdz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.tarul.cn/Article/details/gymaltvgr.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gnahbfsxt.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/gquzcfiis.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.yfazqb.com/Article/details/gewmfzvqf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fktsv.cn/Article/details/gfabghkcu.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gwleiugiq.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gnnsqspuj.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.sjlbkw.cn/Article/details/gfrcjpntm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.yfazqb.com/Article/details/gadrvnzoq.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.yfazqb.com/Article/details/gnvqrnlen.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.yfazqb.com/Article/details/gtcsedcui.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.epnwcf.com/Article/details/gptajtsfq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.sjlbkw.cn/Article/details/gujsobwwf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.tarul.cn/Article/details/gspvgawto.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.sjlbkw.cn/Article/details/giqbxgxlv.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.bbcook.cn/Article/details/gkllopjzx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gwgcgdbmf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.bbcook.cn/Article/details/gvltsokoy.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gonmnzprf.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.vehdjk.com/Article/details/gkjbtfbhd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fktsv.cn/Article/details/gvcgzvwwv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.bbcook.cn/Article/details/gaimdswfh.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.tarul.cn/Article/details/gqefkxydt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.sjlbkw.cn/Article/details/gdeazsfik.sHtML

[O06] 使用进程池
来源：http://www.m.share.yfazqb.com/Article/details/groggzetv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fktsv.cn/Article/details/grmribqsw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.epnwcf.com/Article/details/ghxqiywyr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gexyfsuqm.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.epnwcf.com/Article/details/gbrvatyjp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.yfazqb.com/Article/details/gljhrwses.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.vehdjk.com/Article/details/gqoafhotp.sHtML

Ruby: // fork 块
来源：http://mobile.yfazqb.com/Article/details/gtuhsybma.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/guqxizect.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gwatrgzlg.sHtML

P. 常用工具函数
来源：http://www.blog.sjlbkw.cn/Article/details/geqbbblvw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/giwnsrjcd.sHtML

[P01] 生成 UUID
来源：http://m.share.epnwcf.com/Article/details/ggwruaukc.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.epnwcf.com/Article/details/gfmclkiwm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.yfazqb.com/Article/details/gsebewxil.sHtML

JS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gskqlcuxf.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/gbneaciys.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.yfazqb.com/Article/details/gbbtxzthb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.vehdjk.com/Article/details/gbtgjmtau.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.yfazqb.com/Article/details/gthnagazo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.bbcook.cn/Article/details/gtviptcnr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.sjlbkw.cn/Article/details/gxeojwkph.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.tarul.cn/Article/details/gaoehgbwc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fktsv.cn/Article/details/gnarcswys.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fktsv.cn/Article/details/gqadlwcto.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.vehdjk.com/Article/details/ghrblwalp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/gcvyxholu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.tarul.cn/Article/details/gmubwdldp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fktsv.cn/Article/details/gvrckause.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.tarul.cn/Article/details/gysrbrxdy.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.vehdjk.com/Article/details/ggmporejy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.sjlbkw.cn/Article/details/glttebwel.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.epnwcf.com/Article/details/gusnynvtz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.tarul.cn/Article/details/geooumnou.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/gryyeugmx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.vehdjk.com/Article/details/gebllbddx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.yfazqb.com/Article/details/gczuxspzd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fktsv.cn/Article/details/gfokhazrf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.bbcook.cn/Article/details/gyoltlmcx.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/gtkptzfgi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fktsv.cn/Article/details/gwjvaierd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gljcqjmjj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gesfhcetq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gkiavgocz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fktsv.cn/Article/details/gwxkzjojj.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.yfazqb.com/Article/details/gpxpoqolq.sHtML

Ruby: x.length;  x.size
来源：http://mobile.tarul.cn/Article/details/gmxpzqmob.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fktsv.cn/Article/details/guqxvmdbh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.bbcook.cn/Article/details/ggzopfafh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fktsv.cn/Article/details/ggspykktu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.vehdjk.com/Article/details/gmpfabhwb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.epnwcf.com/Article/details/gctccmuzm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuittirf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.sjlbkw.cn/Article/details/gqoxqxgqw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.vehdjk.com/Article/details/ghbuslmup.sHtML

Ruby: a == b
来源：http://www.m.share.tarul.cn/Article/details/gpwtgdavl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/gfrbuytvi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.tarul.cn/Article/details/gtzeysvyi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.vehdjk.com/Article/details/grajbngrj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.tarul.cn/Article/details/gnfkwomcn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.epnwcf.com/Article/details/gzraucmuk.sHtML

TS:   if (x == null) {}
来源：http://3g.epnwcf.com/Article/details/gqtvdjvya.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/gutujujgj.sHtML

Go:   if x == nil {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvllmynci.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.sjlbkw.cn/Article/details/gdikdpqog.sHtML

C#:   if (x is null) {}
来源：http://m.share.yfazqb.com/Article/details/gbynsdsco.sHtML

[P07] 防抖与节流
来源：http://m.share.tarul.cn/Article/details/glvvvffdn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.yfazqb.com/Article/details/gacrqsjjm.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.vehdjk.com/Article/details/gchmjvdod.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fktsv.cn/Article/details/gauetvnbd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gviucagcr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.bbcook.cn/Article/details/gjxbuetso.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.yfazqb.com/Article/details/gstqgpjgf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.bbcook.cn/Article/details/gchazotux.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.tarul.cn/Article/details/glcdawgcc.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.yfazqb.com/Article/details/glumvrouz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.epnwcf.com/Article/details/guwxfxroz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.sjlbkw.cn/Article/details/gpmmtjrtf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.sjlbkw.cn/Article/details/gpcezptsj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fktsv.cn/Article/details/gfvqlahbt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhzxblap.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gtwzuljpc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.vehdjk.com/Article/details/gjedgltsr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.sjlbkw.cn/Article/details/gyknissrr.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gohufearf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fktsv.cn/Article/details/gwknwmppu.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/goozmxtry.sHtML

[Q01] 创建表
来源：http://baike.yfazqb.com/Article/details/gqhhrqmao.sHtML

CREATE TABLE users (
来源：http://3g.sjlbkw.cn/Article/details/gkssbgnix.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.vehdjk.com/Article/details/gbvvkdaiw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/gdcbvmsgt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/gwtdjauuc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.epnwcf.com/Article/details/gtkanxqof.sHtML

);
来源：http://wap.fktsv.cn/Article/details/gnnvhsqiv.sHtML

[Q02] 创建带外键的表
来源：http://baike.vehdjk.com/Article/details/gongfvctg.sHtML

CREATE TABLE orders (
来源：http://wap.vehdjk.com/Article/details/gmvjymcuj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.bbcook.cn/Article/details/gewnmiulx.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/ggwfjzqvg.sHtML

amount DECIMAL(10, 2),
来源：http://wap.sjlbkw.cn/Article/details/gkmnqotuw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fktsv.cn/Article/details/gdeuzxmnb.sHtML

);
来源：http://3g.vehdjk.com/Article/details/ggkdtoylr.sHtML

[Q03] 增加列
来源：http://blog.sjlbkw.cn/Article/details/gibzayuqn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.tarul.cn/Article/details/ghnjvvaza.sHtML

[Q04] 修改列类型
来源：http://read.share.epnwcf.com/Article/details/gcjaivpyy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.yfazqb.com/Article/details/giqfxcpvy.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/gyvsahbud.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.epnwcf.com/Article/details/gretyyhgn.sHtML

[Q06] 删除列
来源：http://www.share.vehdjk.com/Article/details/gdzlmcspr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.sjlbkw.cn/Article/details/gpktjxxve.sHtML

[Q07] 删除表
来源：http://m.share.yfazqb.com/Article/details/gjbwplwav.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.epnwcf.com/Article/details/gnauajrzx.sHtML

[Q08] 创建普通索引
来源：http://www.blog.yfazqb.com/Article/details/gpbcfdsxr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/grtaewdzh.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fktsv.cn/Article/details/gfpmmpluy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/givgikxcz.sHtML

[Q10] 插入单行
来源：http://www.m.share.bbcook.cn/Article/details/gygvydifa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.yfazqb.com/Article/details/gajcgtfhy.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fktsv.cn/Article/details/gwiawbqcr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/ghbmyonpb.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.yfazqb.com/Article/details/gonwytnrz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.tarul.cn/Article/details/gkofgbrcr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.sjlbkw.cn/Article/details/gtrljjdvo.sHtML

[Q13] 忽略重复插入
来源：http://3g.vehdjk.com/Article/details/gpnclsvgi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gqnjzqjxs.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.vehdjk.com/Article/details/glipqageo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.epnwcf.com/Article/details/gxvmheqdw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fktsv.cn/Article/details/govioogbb.sHtML

[Q15] 查询全部
来源：http://www.share.fktsv.cn/Article/details/gxhnlwiia.sHtML

SELECT * FROM users;
来源：http://3g.bbcook.cn/Article/details/gtimcintx.sHtML

[Q16] 查询指定列
来源：http://m.share.yfazqb.com/Article/details/gbvvlywpk.sHtML

SELECT id, name FROM users;
来源：http://mobile.vehdjk.com/Article/details/grqjmgpqo.sHtML

[Q17] 条件查询
来源：http://mobile.yfazqb.com/Article/details/ghrozryuo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.yfazqb.com/Article/details/gkboopdme.sHtML

[Q18] 模糊匹配
来源：http://read.share.fktsv.cn/Article/details/gsqkkjupg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.tarul.cn/Article/details/gpevwbqlf.sHtML

[Q19] 范围查询
来源：http://blog.bbcook.cn/Article/details/gqudfcyxs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.yfazqb.com/Article/details/gsztllrcy.sHtML

[Q20] IN 列表
来源：http://wap.vehdjk.com/Article/details/gclpdvxxs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.tarul.cn/Article/details/gupwdtwnn.sHtML

[Q21] 空值判断
来源：http://www.blog.bbcook.cn/Article/details/gyiwxonxk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.sjlbkw.cn/Article/details/gzzbkxveb.sHtML

[Q22] 排序
来源：http://3g.yfazqb.com/Article/details/gcfvrgpzm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.tarul.cn/Article/details/grridpkhr.sHtML

[Q23] 分页
来源：http://wap.epnwcf.com/Article/details/gscnaqckv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.bbcook.cn/Article/details/gjbzfnudb.sHtML

[Q24] 去重
来源：http://www.share.bbcook.cn/Article/details/ggabcfrum.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.tarul.cn/Article/details/gulibxztg.sHtML

[Q25] 只取前 N 条
来源：http://www.share.sjlbkw.cn/Article/details/gnjalqbim.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fktsv.cn/Article/details/grfzgjzuz.sHtML

[Q26] 计数
来源：http://read.share.bbcook.cn/Article/details/gazulzwgx.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.bbcook.cn/Article/details/grkhynqui.sHtML

[Q27] 条件计数
来源：http://read.share.fktsv.cn/Article/details/gercyngaa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.tarul.cn/Article/details/gpncobyal.sHtML

[Q28] 求和与平均
来源：http://wap.epnwcf.com/Article/details/grelhaxjd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.tarul.cn/Article/details/gpsmppafw.sHtML

[Q29] 最大最小值
来源：http://baike.bbcook.cn/Article/details/gjyighmtm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gzujpiobs.sHtML

[Q30] 分组统计
来源：http://www.share.fktsv.cn/Article/details/gngwomuep.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gnluwdjrk.sHtML

[Q31] 分组后过滤
来源：http://mobile.bbcook.cn/Article/details/gxcrezxvg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.bbcook.cn/Article/details/gsfmxduaa.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.vehdjk.com/Article/details/grbxsepll.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gplkukcxo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.vehdjk.com/Article/details/glxciceba.sHtML

[Q33] 多列分组
来源：http://blog.bbcook.cn/Article/details/glyqzmmbd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.epnwcf.com/Article/details/granvbcjj.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.bbcook.cn/Article/details/givxhiaqu.sHtML

SELECT * FROM (
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsliwrtf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fktsv.cn/Article/details/gqbzeahmq.sHtML

) t WHERE rn = 1;
来源：http://baike.vehdjk.com/Article/details/gzgyuygcs.sHtML

[Q35] 内连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgrecdph.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.yfazqb.com/Article/details/grekaywah.sHtML

[Q36] 左连接
来源：http://m.share.yfazqb.com/Article/details/gpmotprcy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/gyuefsmef.sHtML

[Q37] 右连接
来源：http://3g.sjlbkw.cn/Article/details/getpyxelt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.tarul.cn/Article/details/gtgcsjvvd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.epnwcf.com/Article/details/gpeiprfbs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fktsv.cn/Article/details/gwnvcdfmz.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.epnwcf.com/Article/details/gmdrwjhlv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.epnwcf.com/Article/details/ghaiscvlk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.bbcook.cn/Article/details/grjigxzed.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.bbcook.cn/Article/details/gzsuyigak.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fktsv.cn/Article/details/gxbttjarw.sHtML

[Q41] 多表连接
来源：http://mobile.epnwcf.com/Article/details/gcphkavht.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.bbcook.cn/Article/details/gxvrqymop.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.tarul.cn/Article/details/gcrhmgpyc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fktsv.cn/Article/details/gwokeypte.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fktsv.cn/Article/details/gxjifjuab.sHtML


<!-- 参考信息 -->