代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.epnwcf.com/Article/details/glgjjqfgs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.epnwcf.com/Article/details/gwcykxung.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.yfazqb.com/Article/details/gqtcwkurn.sHtML

Java: // 手写 HashMap
来源：http://www.share.yfazqb.com/Article/details/gbicknpna.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fktsv.cn/Article/details/gjdzmpcck.sHtML

Ruby: // 手写 Hash
来源：http://blog.tarul.cn/Article/details/gjbsooyim.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.sjlbkw.cn/Article/details/gohsinbyd.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/gnpjdjuqs.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/gehjjogah.sHtML

PHP:  // 手写递归交换
来源：http://m.share.tarul.cn/Article/details/ghzhzsoud.sHtML

JS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/glzebduwx.sHtML

TS:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/ghyaaieli.sHtML

Java: // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gkytjqnip.sHtML

Go:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/goaiskfwo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fktsv.cn/Article/details/gyfclrlat.sHtML

C#:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/grahisquj.sHtML

[N09] 栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gdanmtmqm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.tarul.cn/Article/details/ggltxjqpp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.tarul.cn/Article/details/gbczxlwog.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gnfghcnus.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.vehdjk.com/Article/details/gxmkdbmzu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.epnwcf.com/Article/details/gfknubdlw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.bbcook.cn/Article/details/geckzzlts.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gpxcmopkv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.vehdjk.com/Article/details/gfzgbwcxe.sHtML

[N10] 链表节点定义
来源：http://m.share.tarul.cn/Article/details/gjamwpvid.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.bbcook.cn/Article/details/gpsoqjvys.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.bbcook.cn/Article/details/gbhbvbizq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/gtucgrvfx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.bbcook.cn/Article/details/gdodzlazv.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.bbcook.cn/Article/details/gcpmcfuow.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.yfazqb.com/Article/details/gvxvbawkc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.epnwcf.com/Article/details/gzupojwtk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.bbcook.cn/Article/details/gkutjaxtq.sHtML

[N11] 二叉树中序遍历
来源：http://baike.yfazqb.com/Article/details/ghszjaszu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.bbcook.cn/Article/details/gquxyooho.sHtML

PHP:  // 手写递归函数
来源：http://baike.epnwcf.com/Article/details/glpvycsui.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/giwumucbj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gdgiskmlg.sHtML

Java: // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gysjpwkwi.sHtML

Go:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gbrlwqndd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.epnwcf.com/Article/details/gnzyogjll.sHtML

C#:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/gaqbajmzf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.sjlbkw.cn/Article/details/gyljyfnbh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.bbcook.cn/Article/details/ggdihxiah.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.epnwcf.com/Article/details/gbvelybvf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.tarul.cn/Article/details/gvehlrkov.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/gjprktsfd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/gzzgugwsz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.epnwcf.com/Article/details/gmsviqdgh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.epnwcf.com/Article/details/gkshwmydw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.tarul.cn/Article/details/grcsxliih.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzvibjwdj.sHtML

O. 并发与异步
来源：http://www.blog.bbcook.cn/Article/details/gpbqojuot.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ganitjpkc.sHtML

[O01] 启动一个线程
来源：http://www.share.epnwcf.com/Article/details/gjqijxsaq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fktsv.cn/Article/details/glxomiidt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/gpmgdhfol.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fktsv.cn/Article/details/gkvjqcdub.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gskcaanpl.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.sjlbkw.cn/Article/details/gfyobzpif.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/gmnvvwhsc.sHtML

Ruby: Thread.new { f }
来源：http://baike.bbcook.cn/Article/details/gcjuwhwls.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fktsv.cn/Article/details/gxljnluxo.sHtML

[O02] 使用线程池
来源：http://www.blog.vehdjk.com/Article/details/gjaqmddnq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fktsv.cn/Article/details/gvxkzqlxe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fktsv.cn/Article/details/guunylqyw.sHtML

JS:   // worker_threads 线程池
来源：http://baike.epnwcf.com/Article/details/ggnwfkpqi.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gbmmmuiki.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.bbcook.cn/Article/details/gpzjzffpt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.bbcook.cn/Article/details/gtfrxyfnj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.epnwcf.com/Article/details/guqnkyskk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.vehdjk.com/Article/details/gvtkegfso.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/gynmnuteu.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.bbcook.cn/Article/details/gjalzrqmq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.tarul.cn/Article/details/gugfmqame.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.sjlbkw.cn/Article/details/gopqvfevi.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/gswwltbhk.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.yfazqb.com/Article/details/gogldwpto.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.sjlbkw.cn/Article/details/ghwdmmmcn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.yfazqb.com/Article/details/giqkiujim.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/gbifgecfy.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.yfazqb.com/Article/details/gaksoomyk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.epnwcf.com/Article/details/gltbqjkgr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.epnwcf.com/Article/details/gmjwqkxpk.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gqvhvuzgt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gmtnvqofs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.sjlbkw.cn/Article/details/gzmgzcjzf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.epnwcf.com/Article/details/gpkblocra.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.vehdjk.com/Article/details/gazxxhhpy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.tarul.cn/Article/details/gjxjyiltu.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.epnwcf.com/Article/details/gnuxaivgz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.tarul.cn/Article/details/gmzsqsram.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.yfazqb.com/Article/details/gqnfxkmfr.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.epnwcf.com/Article/details/gdvjfwcfs.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gsgpmyskt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.vehdjk.com/Article/details/gbhkxkhaf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.vehdjk.com/Article/details/gpdalcres.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gwydmypdo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.sjlbkw.cn/Article/details/gvskbgmtk.sHtML

[O06] 使用进程池
来源：http://read.share.epnwcf.com/Article/details/gsrgwxzxd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.tarul.cn/Article/details/gqlhmjdji.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.tarul.cn/Article/details/gnzpiwbui.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/govykgono.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/ghjwozfbj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.bbcook.cn/Article/details/gygmygpfe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fktsv.cn/Article/details/gzigxxgln.sHtML

Ruby: // fork 块
来源：http://mobile.fktsv.cn/Article/details/gisgwlbvl.sHtML

C#:   Parallel.For
来源：http://mobile.tarul.cn/Article/details/gznybieyc.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gruulriqx.sHtML

P. 常用工具函数
来源：http://read.share.tarul.cn/Article/details/gbzmfcazc.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkjbzqcqr.sHtML

[P01] 生成 UUID
来源：http://blog.vehdjk.com/Article/details/gpfirvxnn.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.sjlbkw.cn/Article/details/gfvdmykot.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fktsv.cn/Article/details/gmfxojmgf.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gfsgvzyqe.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gbtvcugzg.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.bbcook.cn/Article/details/gofrbfcxl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.vehdjk.com/Article/details/gcplsydsq.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.yfazqb.com/Article/details/gittttlri.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.epnwcf.com/Article/details/ggvnszvpn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.epnwcf.com/Article/details/gvkhxzthz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/gztvxomkc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.tarul.cn/Article/details/gfjzrjsem.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fktsv.cn/Article/details/gglhgbhbf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.vehdjk.com/Article/details/gnficxtam.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fktsv.cn/Article/details/givtzgfuk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.epnwcf.com/Article/details/guxmajmpa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.vehdjk.com/Article/details/guhtxnety.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.yfazqb.com/Article/details/gqxladmhp.sHtML

[P03] 生成短随机字符串
来源：http://wap.tarul.cn/Article/details/greruoipq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.yfazqb.com/Article/details/gxgaafcno.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.yfazqb.com/Article/details/gzlgyzjwe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fktsv.cn/Article/details/gekqvfcic.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/guomwszly.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.bbcook.cn/Article/details/gvamvekxa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.tarul.cn/Article/details/gclwwtnzf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.vehdjk.com/Article/details/gemdstvlk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gqdqoyihc.sHtML

[P04] 求长度
来源：http://m.share.tarul.cn/Article/details/gocjgpioy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fktsv.cn/Article/details/gcuxqfyos.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gxssvbbjp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gobopdaly.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gsdpcqeif.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.epnwcf.com/Article/details/gydjdgljq.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fktsv.cn/Article/details/gfyowmmhy.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gwhlhjknq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gaqcarnym.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.sjlbkw.cn/Article/details/gshenyvka.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.sjlbkw.cn/Article/details/giitcgmst.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.sjlbkw.cn/Article/details/gfttfxlan.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.yfazqb.com/Article/details/gzeqraamr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.vehdjk.com/Article/details/gtdzyhaaz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fktsv.cn/Article/details/gjyxmephd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fktsv.cn/Article/details/gzwedzeqm.sHtML

Ruby: a == b
来源：http://mobile.sjlbkw.cn/Article/details/gvplekehb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.bbcook.cn/Article/details/goftjfgsp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.tarul.cn/Article/details/gqcryprza.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fktsv.cn/Article/details/gsxpdmgeo.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.epnwcf.com/Article/details/ghgnfmnwt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.vehdjk.com/Article/details/gjynmvpjg.sHtML

TS:   if (x == null) {}
来源：http://baike.bbcook.cn/Article/details/gqsjkakci.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gsybonhuj.sHtML

Go:   if x == nil {}
来源：http://read.share.vehdjk.com/Article/details/gdfoxgqpz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fktsv.cn/Article/details/gnfndxodn.sHtML

C#:   if (x is null) {}
来源：http://www.blog.yfazqb.com/Article/details/grpfrgxvm.sHtML

[P07] 防抖与节流
来源：http://www.blog.epnwcf.com/Article/details/ggpykgbnv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.bbcook.cn/Article/details/gsqchpkem.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.yfazqb.com/Article/details/giuxvducb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gkadalnth.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gytfzjlxo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/goglqwonr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.yfazqb.com/Article/details/gcohcbeuh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.bbcook.cn/Article/details/gyohixhyt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.yfazqb.com/Article/details/gdpyyqfcj.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.bbcook.cn/Article/details/gevmsxttr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.epnwcf.com/Article/details/gqxeaikfa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fktsv.cn/Article/details/gxzkfhifw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.tarul.cn/Article/details/gthoanynf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fktsv.cn/Article/details/gcwgxsctj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.yfazqb.com/Article/details/glwgbyrsh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.vehdjk.com/Article/details/guhzscoad.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.sjlbkw.cn/Article/details/gjxwcwayy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fktsv.cn/Article/details/ggdcwkyre.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gabvboymr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.bbcook.cn/Article/details/gwfzqrqcf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gsdihixnh.sHtML

[Q01] 创建表
来源：http://www.share.epnwcf.com/Article/details/gbslyapxr.sHtML

CREATE TABLE users (
来源：http://www.m.share.epnwcf.com/Article/details/gwyeeceqv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gfymgloeg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gompxjsaa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.sjlbkw.cn/Article/details/grbyyvidx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.epnwcf.com/Article/details/gcrdhndfw.sHtML

);
来源：http://3g.tarul.cn/Article/details/gxhrwueke.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fktsv.cn/Article/details/ghxyfjvgh.sHtML

CREATE TABLE orders (
来源：http://mobile.yfazqb.com/Article/details/gqluuhzbg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.tarul.cn/Article/details/gumaawogs.sHtML

user_id INT NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/gmzejnvcx.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.yfazqb.com/Article/details/gkudfrcyl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.bbcook.cn/Article/details/gotfulmcp.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/gwkellntu.sHtML

[Q03] 增加列
来源：http://3g.fktsv.cn/Article/details/gunkqqaoo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.bbcook.cn/Article/details/guphwrwqa.sHtML

[Q04] 修改列类型
来源：http://3g.tarul.cn/Article/details/givqihctk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.sjlbkw.cn/Article/details/gzdakjgmm.sHtML

[Q05] 重命名列
来源：http://3g.fktsv.cn/Article/details/glbstcbtg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.tarul.cn/Article/details/gbzyhadht.sHtML

[Q06] 删除列
来源：http://www.m.share.fktsv.cn/Article/details/gpidbidrk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.vehdjk.com/Article/details/goxuguben.sHtML

[Q07] 删除表
来源：http://www.share.vehdjk.com/Article/details/gscnpgxeb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fktsv.cn/Article/details/gxfwnytoe.sHtML

[Q08] 创建普通索引
来源：http://wap.vehdjk.com/Article/details/gtcbghpie.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gfifftoki.sHtML

[Q09] 创建唯一索引
来源：http://read.share.tarul.cn/Article/details/gespxsszs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/ghifedrmk.sHtML

[Q10] 插入单行
来源：http://www.m.share.sjlbkw.cn/Article/details/ggoxccjff.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gqrvclixm.sHtML

[Q11] 一次插入多行
来源：http://m.share.fktsv.cn/Article/details/gwqxzifqw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/gyfhkwmmx.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fktsv.cn/Article/details/guykysdmg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fktsv.cn/Article/details/gcldwyqpn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.sjlbkw.cn/Article/details/goujtabvh.sHtML

[Q13] 忽略重复插入
来源：http://blog.tarul.cn/Article/details/gldlxvzwj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fktsv.cn/Article/details/gyltdyxaw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fktsv.cn/Article/details/gkrvbsktu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.yfazqb.com/Article/details/godfledoc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.sjlbkw.cn/Article/details/gixmxixth.sHtML

[Q15] 查询全部
来源：http://wap.fktsv.cn/Article/details/gevwhqzzg.sHtML

SELECT * FROM users;
来源：http://www.share.yfazqb.com/Article/details/ggeqclmlz.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/gbriolhmb.sHtML

SELECT id, name FROM users;
来源：http://wap.bbcook.cn/Article/details/gzhlkzspy.sHtML

[Q17] 条件查询
来源：http://www.share.epnwcf.com/Article/details/ggvuoiepv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fktsv.cn/Article/details/gpokauejo.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.epnwcf.com/Article/details/gkmbewnyl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.epnwcf.com/Article/details/gbzmpclie.sHtML

[Q19] 范围查询
来源：http://www.share.fktsv.cn/Article/details/grgyaubai.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.yfazqb.com/Article/details/gfdldlopu.sHtML

[Q20] IN 列表
来源：http://3g.bbcook.cn/Article/details/gphlqjdzl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.vehdjk.com/Article/details/gkpdfluqe.sHtML

[Q21] 空值判断
来源：http://www.blog.epnwcf.com/Article/details/gnvblkdzg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fktsv.cn/Article/details/ggbpaecso.sHtML

[Q22] 排序
来源：http://baike.vehdjk.com/Article/details/gtevwjxpy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.tarul.cn/Article/details/ghillmwhy.sHtML

[Q23] 分页
来源：http://wap.vehdjk.com/Article/details/gbbjevdjx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.yfazqb.com/Article/details/gbwyjrsaw.sHtML

[Q24] 去重
来源：http://baike.sjlbkw.cn/Article/details/galvmtgzd.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.yfazqb.com/Article/details/gdlrfabtk.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fktsv.cn/Article/details/gyrlmwybj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.epnwcf.com/Article/details/gmpgquyqa.sHtML

[Q26] 计数
来源：http://read.share.epnwcf.com/Article/details/gpvasndzo.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gebsrqjxt.sHtML

[Q27] 条件计数
来源：http://www.blog.sjlbkw.cn/Article/details/gdksrzdfl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gimdskcuc.sHtML

[Q28] 求和与平均
来源：http://www.share.vehdjk.com/Article/details/gpsxkkvxr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.tarul.cn/Article/details/grryajiko.sHtML

[Q29] 最大最小值
来源：http://mobile.vehdjk.com/Article/details/govywmybp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlhkxfrt.sHtML

[Q30] 分组统计
来源：http://baike.tarul.cn/Article/details/gbtcspnzp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gosplrbbu.sHtML

[Q31] 分组后过滤
来源：http://www.share.fktsv.cn/Article/details/gtfvwxmhq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.sjlbkw.cn/Article/details/gpomyhsvj.sHtML

[Q32] 分组拼接字符串
来源：http://blog.vehdjk.com/Article/details/gsfajkmqg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gbqcwtsbm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.sjlbkw.cn/Article/details/goztehwmt.sHtML

[Q33] 多列分组
来源：http://wap.tarul.cn/Article/details/ghewkhjts.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.bbcook.cn/Article/details/gsjomibpi.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.tarul.cn/Article/details/getxmfhrf.sHtML

SELECT * FROM (
来源：http://blog.fktsv.cn/Article/details/gliwaqmci.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.bbcook.cn/Article/details/gdtbjruca.sHtML

) t WHERE rn = 1;
来源：http://www.blog.epnwcf.com/Article/details/gumkllktl.sHtML

[Q35] 内连接
来源：http://wap.fktsv.cn/Article/details/gjwnfbxlq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gqjddvbzv.sHtML

[Q36] 左连接
来源：http://3g.fktsv.cn/Article/details/gtzoofrmi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/gtoowopfm.sHtML

[Q37] 右连接
来源：http://read.share.sjlbkw.cn/Article/details/gdwttsxet.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.vehdjk.com/Article/details/grctjyufy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fktsv.cn/Article/details/gcdmqghot.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.sjlbkw.cn/Article/details/gosowyobt.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.epnwcf.com/Article/details/glrpfkhpx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fktsv.cn/Article/details/gfstybxwj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.yfazqb.com/Article/details/gxwzquwkv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.epnwcf.com/Article/details/gpsfmxztm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/grtomogok.sHtML

[Q41] 多表连接
来源：http://wap.yfazqb.com/Article/details/gscqddgno.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.bbcook.cn/Article/details/gmdpqffic.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.yfazqb.com/Article/details/gctboenyx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/gdoqpdqxq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.epnwcf.com/Article/details/giicylagw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.tarul.cn/Article/details/ghbqeixch.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.sjlbkw.cn/Article/details/gylwltfmo.sHtML

[Q43] 标量子查询
来源：http://3g.tarul.cn/Article/details/gxkvsflql.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fktsv.cn/Article/details/gejpircjz.sHtML

[Q44] IN 子查询
来源：http://www.m.share.tarul.cn/Article/details/gpzsavcdc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.bbcook.cn/Article/details/gqsqggyob.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.bbcook.cn/Article/details/ggpwlmfxd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/ghxdtqhdq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.sjlbkw.cn/Article/details/gbzmmyknd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.vehdjk.com/Article/details/gcnqrbltz.sHtML

[Q47] 与平均值比较
来源：http://read.share.bbcook.cn/Article/details/gyhqmsalh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.tarul.cn/Article/details/gpuknvbxy.sHtML


<!-- 参考信息 -->