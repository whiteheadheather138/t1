代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gagpaqjhp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.epnwcf.com/Article/details/gcqpsohej.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.epnwcf.com/Article/details/gdobvsxda.sHtML

Ruby: a.gcd(b)
来源：http://mobile.sjlbkw.cn/Article/details/gfiuxicgm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.bbcook.cn/Article/details/gjcrjecat.sHtML

[N06] 判断回文字符串
来源：http://mobile.fktsv.cn/Article/details/grgjobegj.sHtML

Py:   s == s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gthgbbazk.sHtML

PHP:  $s === strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gnrvzrrbk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gckrijtwh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gmtgeceaa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.yfazqb.com/Article/details/gjginjrbu.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.bbcook.cn/Article/details/gpltjebnw.sHtML

Ruby: s == s.reverse
来源：http://mobile.sjlbkw.cn/Article/details/goffvdpoa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.yfazqb.com/Article/details/gfmuhjrka.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.sjlbkw.cn/Article/details/ghfqzrbsj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fktsv.cn/Article/details/gxdwpcfxn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.bbcook.cn/Article/details/gkueczxkb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.sjlbkw.cn/Article/details/glmwedtbq.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fktsv.cn/Article/details/gjfztpgxd.sHtML

Java: // 手写 HashMap
来源：http://3g.vehdjk.com/Article/details/glnwkxgwy.sHtML

Go:   // 手写 map[int]int
来源：http://blog.vehdjk.com/Article/details/gxprutqpf.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/gotqdqtfr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fktsv.cn/Article/details/gvdvhzxvr.sHtML

[N08] 生成全排列
来源：http://mobile.vehdjk.com/Article/details/grojcltyj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.epnwcf.com/Article/details/gbdfsfjcv.sHtML

PHP:  // 手写递归交换
来源：http://mobile.yfazqb.com/Article/details/grgoypblo.sHtML

JS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gildkwndj.sHtML

TS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gflhjpldk.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/grnchhmfk.sHtML

Go:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gjgxybfiy.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fktsv.cn/Article/details/gtvojbzaa.sHtML

C#:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/grlsxyuhz.sHtML

[N09] 栈与队列
来源：http://baike.bbcook.cn/Article/details/gsqclffbm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.epnwcf.com/Article/details/gsdzbttlg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.epnwcf.com/Article/details/grrwrbshf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/griqstafo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.yfazqb.com/Article/details/grnyzxgyd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.bbcook.cn/Article/details/goupvkhkg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.yfazqb.com/Article/details/gfcjchtai.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gynuqsort.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.tarul.cn/Article/details/gdnywzdks.sHtML

[N10] 链表节点定义
来源：http://3g.tarul.cn/Article/details/gtjymifhh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.vehdjk.com/Article/details/gjlgmoywx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.tarul.cn/Article/details/gsyclbklf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fktsv.cn/Article/details/grcldnlqs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.vehdjk.com/Article/details/geoecakba.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.epnwcf.com/Article/details/gxtzphueh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.yfazqb.com/Article/details/gdkuaoqcg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.bbcook.cn/Article/details/gvxjcbcpz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.epnwcf.com/Article/details/gknjyiknd.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.bbcook.cn/Article/details/gmkwacexp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.sjlbkw.cn/Article/details/gxyjmuiik.sHtML

PHP:  // 手写递归函数
来源：http://baike.yfazqb.com/Article/details/grpslyxum.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/glokdrxgv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gsenvizwo.sHtML

Java: // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gehahrdqh.sHtML

Go:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gfgkcfvgv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.sjlbkw.cn/Article/details/gyzvexllv.sHtML

C#:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gzmexddzp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fktsv.cn/Article/details/givgojjwq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gkvgtiymn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.vehdjk.com/Article/details/gxpgahnmp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gmupustth.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gnchovmhn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gvknblzec.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.vehdjk.com/Article/details/gqongqezq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.vehdjk.com/Article/details/gwcoyyyue.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gpwkjfbzi.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvhlewznb.sHtML

O. 并发与异步
来源：http://m.share.tarul.cn/Article/details/gzknokefz.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gjovfbftk.sHtML

[O01] 启动一个线程
来源：http://read.share.tarul.cn/Article/details/glbfrhkyz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.sjlbkw.cn/Article/details/gfegcdwog.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.sjlbkw.cn/Article/details/gdacdpqbu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.yfazqb.com/Article/details/gnydvuhfk.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gywwetikf.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.tarul.cn/Article/details/gstnkbsmh.sHtML

Go:   go f()
来源：http://m.share.fktsv.cn/Article/details/gufhptvvu.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbipfvgov.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fktsv.cn/Article/details/gdibscakx.sHtML

[O02] 使用线程池
来源：http://3g.bbcook.cn/Article/details/gttmorgyj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fktsv.cn/Article/details/gtesxgknk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.yfazqb.com/Article/details/gjxskkehh.sHtML

JS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/glukvvdnt.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/giygrvtzt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.vehdjk.com/Article/details/goixxjytb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.tarul.cn/Article/details/gilkujbpz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.vehdjk.com/Article/details/gxvpgyypg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.vehdjk.com/Article/details/gyvghwksy.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.yfazqb.com/Article/details/gzfeptnop.sHtML

Py:   with lock: shared += 1
来源：http://3g.fktsv.cn/Article/details/gvztgzfig.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.sjlbkw.cn/Article/details/gyjhhhzsh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.epnwcf.com/Article/details/ggkikxexn.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gjornfdgb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gvchfcesd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/gtgkufmwv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.yfazqb.com/Article/details/gqlbdsdah.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.tarul.cn/Article/details/gxjnftufa.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fktsv.cn/Article/details/gzwwieldq.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fktsv.cn/Article/details/gclqnavdr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.epnwcf.com/Article/details/guhwssnao.sHtML

JS:   async function f() { await g(); }
来源：http://baike.tarul.cn/Article/details/gaysdrkon.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.bbcook.cn/Article/details/gczenynkt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.sjlbkw.cn/Article/details/ghicknxuv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.yfazqb.com/Article/details/gkiyukplr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.vehdjk.com/Article/details/gkoyplong.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.yfazqb.com/Article/details/gvbfhuhpo.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.epnwcf.com/Article/details/griulacnz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.bbcook.cn/Article/details/gxxnbnvyv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.epnwcf.com/Article/details/gayrphobf.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.vehdjk.com/Article/details/gtjgipvfn.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.vehdjk.com/Article/details/glrzbixhb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.tarul.cn/Article/details/gvjftqkzt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.bbcook.cn/Article/details/gtogfiqmb.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnmraslk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.yfazqb.com/Article/details/gqtklpyxf.sHtML

[O06] 使用进程池
来源：http://3g.vehdjk.com/Article/details/glncxtnrh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fktsv.cn/Article/details/gplhhofzh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.sjlbkw.cn/Article/details/gfcgptnth.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.bbcook.cn/Article/details/gzsugxrop.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gbnoyttas.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.bbcook.cn/Article/details/gcomjcvbj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.vehdjk.com/Article/details/gztsdpgez.sHtML

Ruby: // fork 块
来源：http://blog.epnwcf.com/Article/details/gspnizefi.sHtML

C#:   Parallel.For
来源：http://3g.sjlbkw.cn/Article/details/gmhqtrurh.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gwnxnjdru.sHtML

P. 常用工具函数
来源：http://www.blog.fktsv.cn/Article/details/gxplfbrhs.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gjaiuwubv.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/gowvjkike.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.epnwcf.com/Article/details/guqqfnugm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fktsv.cn/Article/details/gcukdmyfr.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gpdxvhucn.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/gwxvzeqvu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.tarul.cn/Article/details/gllfnljnr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.epnwcf.com/Article/details/gzwvofeub.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.tarul.cn/Article/details/glgfpilgz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.vehdjk.com/Article/details/gnitfrwiu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.bbcook.cn/Article/details/gfvphmgqu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.epnwcf.com/Article/details/gkhtdvtyg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.yfazqb.com/Article/details/gzyiyixii.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.yfazqb.com/Article/details/gcznspmpo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.bbcook.cn/Article/details/gcauaoera.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.sjlbkw.cn/Article/details/githqjqep.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.tarul.cn/Article/details/gndnrfkux.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.vehdjk.com/Article/details/grbevzrxz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.sjlbkw.cn/Article/details/grhdxgkmm.sHtML

[P03] 生成短随机字符串
来源：http://m.share.bbcook.cn/Article/details/ggsuyfpol.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.tarul.cn/Article/details/gntxwkauz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.bbcook.cn/Article/details/gbaynfngc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gyypieftp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gwgpxojnd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.epnwcf.com/Article/details/gkrzjatmf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.epnwcf.com/Article/details/gbqieewbj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.epnwcf.com/Article/details/gtuwfplri.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.epnwcf.com/Article/details/gwqekzxbz.sHtML

[P04] 求长度
来源：http://mobile.tarul.cn/Article/details/gjwfleuao.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.vehdjk.com/Article/details/gyzhpprbb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gaejvajbq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.epnwcf.com/Article/details/gixihjxqx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gxbtsadqk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fktsv.cn/Article/details/ggatfuudc.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.bbcook.cn/Article/details/gnilexuuz.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fktsv.cn/Article/details/gycuupmvw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.epnwcf.com/Article/details/gcgtggoje.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.vehdjk.com/Article/details/gzslocvoq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fktsv.cn/Article/details/gwkqrsyjf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.epnwcf.com/Article/details/ghggjdjcp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.tarul.cn/Article/details/gabfknfdw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/gfdvpvfvx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.yfazqb.com/Article/details/ggzebmejt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.tarul.cn/Article/details/gagerghlx.sHtML

Ruby: a == b
来源：http://read.share.vehdjk.com/Article/details/gnzfimgsc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.tarul.cn/Article/details/gbddjkekr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/gqupqgsmu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.vehdjk.com/Article/details/gycotsuts.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.vehdjk.com/Article/details/guwrcnein.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.sjlbkw.cn/Article/details/gmtxwntrx.sHtML

TS:   if (x == null) {}
来源：http://www.blog.bbcook.cn/Article/details/gcgvjllfi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/gduentgsm.sHtML

Go:   if x == nil {}
来源：http://blog.bbcook.cn/Article/details/geattjivo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.sjlbkw.cn/Article/details/gmnuekwtg.sHtML

C#:   if (x is null) {}
来源：http://blog.yfazqb.com/Article/details/gnnkhpxng.sHtML

[P07] 防抖与节流
来源：http://m.share.sjlbkw.cn/Article/details/gpyujnupk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.sjlbkw.cn/Article/details/gharalque.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.sjlbkw.cn/Article/details/gdbcrzxnz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gifdsdjvd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gcvanwjsy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fktsv.cn/Article/details/gumnmkgep.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.tarul.cn/Article/details/gkbzouhej.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.yfazqb.com/Article/details/gyqlgiecd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.yfazqb.com/Article/details/guoppnnts.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fktsv.cn/Article/details/ghgsvzuon.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsnyoloq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fktsv.cn/Article/details/gwwpystjp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.yfazqb.com/Article/details/gwehhpytn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.sjlbkw.cn/Article/details/guuhhdjzq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.tarul.cn/Article/details/gatimsbto.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.sjlbkw.cn/Article/details/gejmguzus.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.bbcook.cn/Article/details/grzdpfnof.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.yfazqb.com/Article/details/gnqkuqjho.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmiesbyvr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.epnwcf.com/Article/details/gmfzvtdnx.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjsdzcenv.sHtML

[Q01] 创建表
来源：http://baike.fktsv.cn/Article/details/govxjbjvw.sHtML

CREATE TABLE users (
来源：http://www.share.fktsv.cn/Article/details/gcpmrcurr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/gawxnlrjh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/gbascnvyv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fktsv.cn/Article/details/gppmklkit.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.sjlbkw.cn/Article/details/gsdyfjkxr.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/gvcdpvgjt.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.tarul.cn/Article/details/gwmzpswtt.sHtML

CREATE TABLE orders (
来源：http://read.share.epnwcf.com/Article/details/gpxfomokl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gcfnwzobr.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/gszmqqjrp.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.epnwcf.com/Article/details/gfhjvdrhf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fktsv.cn/Article/details/gmubdscld.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/gjbtssnsz.sHtML

[Q03] 增加列
来源：http://read.share.fktsv.cn/Article/details/gnefidrzn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.vehdjk.com/Article/details/ghcaqshnx.sHtML

[Q04] 修改列类型
来源：http://3g.sjlbkw.cn/Article/details/gsvcribmp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.yfazqb.com/Article/details/gbnwbwubk.sHtML

[Q05] 重命名列
来源：http://3g.fktsv.cn/Article/details/gtfqokovn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fktsv.cn/Article/details/gjgzcedke.sHtML

[Q06] 删除列
来源：http://www.blog.epnwcf.com/Article/details/giecmdvsl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.yfazqb.com/Article/details/gmqrimmzh.sHtML

[Q07] 删除表
来源：http://baike.vehdjk.com/Article/details/gnunrhyvy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fktsv.cn/Article/details/gjtzrybyp.sHtML

[Q08] 创建普通索引
来源：http://wap.bbcook.cn/Article/details/giirfvkiu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/guehsrihk.sHtML

[Q09] 创建唯一索引
来源：http://wap.yfazqb.com/Article/details/gbolhwdpz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fktsv.cn/Article/details/gzphjwfeb.sHtML

[Q10] 插入单行
来源：http://m.share.yfazqb.com/Article/details/gkkzzwpqg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gurokwmzy.sHtML

[Q11] 一次插入多行
来源：http://baike.fktsv.cn/Article/details/getbszvbc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.epnwcf.com/Article/details/gbtcghscl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.tarul.cn/Article/details/ggherqrih.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.vehdjk.com/Article/details/gxwdgzqvx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.bbcook.cn/Article/details/gshblqapx.sHtML

[Q13] 忽略重复插入
来源：http://mobile.bbcook.cn/Article/details/gdtmoulwy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gsjyshdsy.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.bbcook.cn/Article/details/guobmrhmm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fktsv.cn/Article/details/geayxblef.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.tarul.cn/Article/details/gnhpeqgni.sHtML

[Q15] 查询全部
来源：http://m.share.epnwcf.com/Article/details/gmimtcjur.sHtML

SELECT * FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gyvlhxghx.sHtML

[Q16] 查询指定列
来源：http://www.share.yfazqb.com/Article/details/goqecmdos.sHtML

SELECT id, name FROM users;
来源：http://wap.fktsv.cn/Article/details/gqvfobdry.sHtML

[Q17] 条件查询
来源：http://m.share.tarul.cn/Article/details/guacmnqqu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.yfazqb.com/Article/details/gydyrwsfx.sHtML

[Q18] 模糊匹配
来源：http://m.share.vehdjk.com/Article/details/guvxoeten.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.bbcook.cn/Article/details/gbyyhyuvh.sHtML

[Q19] 范围查询
来源：http://read.share.vehdjk.com/Article/details/guwwokqpc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.sjlbkw.cn/Article/details/gxtaeuxzn.sHtML

[Q20] IN 列表
来源：http://www.blog.yfazqb.com/Article/details/gboeiasel.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjdwwyqv.sHtML

[Q21] 空值判断
来源：http://m.share.bbcook.cn/Article/details/gdyrhnazo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fktsv.cn/Article/details/gqqveflqz.sHtML

[Q22] 排序
来源：http://blog.fktsv.cn/Article/details/gnzpjvecx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.epnwcf.com/Article/details/gkydimoeh.sHtML

[Q23] 分页
来源：http://mobile.yfazqb.com/Article/details/gwbplwafw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.bbcook.cn/Article/details/gxehwrkmy.sHtML

[Q24] 去重
来源：http://m.share.fktsv.cn/Article/details/glejzkvxo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.tarul.cn/Article/details/gudxhqzil.sHtML

[Q25] 只取前 N 条
来源：http://m.share.tarul.cn/Article/details/gwstnbgrb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.sjlbkw.cn/Article/details/gwlqfhkbx.sHtML

[Q26] 计数
来源：http://baike.sjlbkw.cn/Article/details/gmvxmetzw.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.tarul.cn/Article/details/gvgobuyfv.sHtML

[Q27] 条件计数
来源：http://3g.tarul.cn/Article/details/gitimtxbc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.tarul.cn/Article/details/gsnutffus.sHtML

[Q28] 求和与平均
来源：http://baike.sjlbkw.cn/Article/details/glvftmrbb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gniftejyl.sHtML

[Q29] 最大最小值
来源：http://m.share.fktsv.cn/Article/details/gqetrnmnt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gpiavyyke.sHtML

[Q30] 分组统计
来源：http://www.share.bbcook.cn/Article/details/gupufxmxf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/gdpjleotf.sHtML

[Q31] 分组后过滤
来源：http://mobile.yfazqb.com/Article/details/golmzdwtb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.bbcook.cn/Article/details/gxaqlhlgc.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gzsrcucou.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/glxbdxoyy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fktsv.cn/Article/details/gcigjztii.sHtML

[Q33] 多列分组
来源：http://read.share.vehdjk.com/Article/details/gqunfulwl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.bbcook.cn/Article/details/gtsgqquqb.sHtML

[Q34] 每组取第一条
来源：http://www.share.yfazqb.com/Article/details/gaquvnnzv.sHtML

SELECT * FROM (
来源：http://mobile.vehdjk.com/Article/details/gqcktwjsd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.bbcook.cn/Article/details/gvsfvjbrf.sHtML

) t WHERE rn = 1;
来源：http://www.blog.tarul.cn/Article/details/gyimqunmm.sHtML

[Q35] 内连接
来源：http://www.blog.yfazqb.com/Article/details/ghwysdagi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gbsbtzjnt.sHtML

[Q36] 左连接
来源：http://www.blog.sjlbkw.cn/Article/details/gmcgzevym.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gfbccpgvn.sHtML

[Q37] 右连接
来源：http://3g.bbcook.cn/Article/details/glacbkllj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.sjlbkw.cn/Article/details/gigskwusr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.epnwcf.com/Article/details/grtwmphke.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.epnwcf.com/Article/details/gmnskudhj.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.sjlbkw.cn/Article/details/gcmdthvda.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.bbcook.cn/Article/details/gvndakiqz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.sjlbkw.cn/Article/details/guijveakt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.epnwcf.com/Article/details/gdtphxfgu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fktsv.cn/Article/details/gcbseludn.sHtML

[Q41] 多表连接
来源：http://read.share.sjlbkw.cn/Article/details/gjkhdiyax.sHtML


<!-- 参考信息 -->