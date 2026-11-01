代发 wailian999

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/gfmyndzmv.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gtotmxleh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.epnwcf.com/Article/details/gkusyyqva.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gjacnznjd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/gkflwcjcw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/gbnzsoybz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.bbcook.cn/Article/details/gkrakiurn.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/glicxpkcj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.sjlbkw.cn/Article/details/gnghueauw.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fktsv.cn/Article/details/girlzzuzn.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/gegiwubsf.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/gohxvvouj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/glgdtxwfm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gnvqdgyzs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.vehdjk.com/Article/details/gxdzasrpo.sHtML

Go:   // 双指针从两端比较
来源：http://baike.bbcook.cn/Article/details/gnxaagdly.sHtML

Ruby: s == s.reverse
来源：http://m.share.epnwcf.com/Article/details/gpelicquy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gftfkdygd.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.yfazqb.com/Article/details/gtckurpan.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.vehdjk.com/Article/details/gomimgxiq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.epnwcf.com/Article/details/gnldjtcka.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fktsv.cn/Article/details/gbgwfqchh.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/gbzpaxzpb.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlibikqg.sHtML

Go:   // 手写 map[int]int
来源：http://blog.tarul.cn/Article/details/guzkzgzib.sHtML

Ruby: // 手写 Hash
来源：http://read.share.vehdjk.com/Article/details/gsyijhvbi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.epnwcf.com/Article/details/givvhtmbt.sHtML

[N08] 生成全排列
来源：http://www.share.bbcook.cn/Article/details/grynyvpiw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gbfmkoila.sHtML

PHP:  // 手写递归交换
来源：http://mobile.bbcook.cn/Article/details/gafrvvixs.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/goxdarqsb.sHtML

TS:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gagwpazbc.sHtML

Java: // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gibbgpihv.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gmuyncoal.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fktsv.cn/Article/details/gxhjxttsm.sHtML

C#:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gbafzwyms.sHtML

[N09] 栈与队列
来源：http://read.share.yfazqb.com/Article/details/gmveotxmv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gripylkcz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.epnwcf.com/Article/details/ghfkdikym.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gfeudoqrn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.tarul.cn/Article/details/gztlnardp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.tarul.cn/Article/details/goukvswmi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.sjlbkw.cn/Article/details/giagzyhuc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.yfazqb.com/Article/details/gbtclmvxf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.sjlbkw.cn/Article/details/gakmyuqiy.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/gvwyajhlf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.epnwcf.com/Article/details/gzpnnacco.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.vehdjk.com/Article/details/gxoylebgw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.yfazqb.com/Article/details/gnkagiubz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.tarul.cn/Article/details/gvbwrpdbw.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.yfazqb.com/Article/details/gcvikdxdp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.bbcook.cn/Article/details/gbiyaqenl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.vehdjk.com/Article/details/grcfmfetw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.vehdjk.com/Article/details/gytvhyddb.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fktsv.cn/Article/details/geveoqwjy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.tarul.cn/Article/details/goucijshc.sHtML

PHP:  // 手写递归函数
来源：http://mobile.tarul.cn/Article/details/gmjfswrng.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gjhkyshib.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/gccxchdcp.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/gqvssbszy.sHtML

Go:   // 手写递归
来源：http://3g.tarul.cn/Article/details/gvghqsjzs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.epnwcf.com/Article/details/gfdnionsp.sHtML

C#:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gdogsrrau.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fktsv.cn/Article/details/gtohfjmxv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.bbcook.cn/Article/details/grzpwlgtx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.tarul.cn/Article/details/gpppobniy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gkderyxvg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/guedhwrwy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/gqigvgeqd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.yfazqb.com/Article/details/goxpjbesy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.yfazqb.com/Article/details/gxnkvbxzx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gogrchbmi.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxhlyymzq.sHtML

O. 并发与异步
来源：http://read.share.bbcook.cn/Article/details/gckqjgbaa.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gecsbafzd.sHtML

[O01] 启动一个线程
来源：http://read.share.vehdjk.com/Article/details/gjcegvncd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.epnwcf.com/Article/details/gbroiksyx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.sjlbkw.cn/Article/details/gfnniucrw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.tarul.cn/Article/details/geyvnznze.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/gmsogxqax.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.tarul.cn/Article/details/gvzodsxwy.sHtML

Go:   go f()
来源：http://read.share.epnwcf.com/Article/details/gjwsselqk.sHtML

Ruby: Thread.new { f }
来源：http://baike.sjlbkw.cn/Article/details/gupvwsija.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.bbcook.cn/Article/details/gbkzcukzk.sHtML

[O02] 使用线程池
来源：http://wap.epnwcf.com/Article/details/gzbuzuarq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.epnwcf.com/Article/details/gorzonfml.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.tarul.cn/Article/details/gtprofscq.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/gykpsakbu.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gpgnghxiy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.epnwcf.com/Article/details/gdiyfpmio.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.bbcook.cn/Article/details/gueswjwux.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.bbcook.cn/Article/details/glpcuvuss.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/guraqtrqb.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/gzimcvchj.sHtML

Py:   with lock: shared += 1
来源：http://3g.vehdjk.com/Article/details/gmdbeacve.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fktsv.cn/Article/details/gsltijfsf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.yfazqb.com/Article/details/ggthxjhuc.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gjbwziayr.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gfnlekmgx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.vehdjk.com/Article/details/gtosjnywy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.sjlbkw.cn/Article/details/gkljolmct.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gopsbxero.sHtML

[O04] 定义异步函数并等待
来源：http://wap.yfazqb.com/Article/details/gxrlmjoph.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.bbcook.cn/Article/details/gmikbutfo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fktsv.cn/Article/details/gaomvuuqn.sHtML

JS:   async function f() { await g(); }
来源：http://baike.vehdjk.com/Article/details/goauxlidv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.tarul.cn/Article/details/goawufqvo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.yfazqb.com/Article/details/gfenfwlel.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fktsv.cn/Article/details/gsriavhim.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.sjlbkw.cn/Article/details/gnnwnftwh.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.epnwcf.com/Article/details/gfbagczti.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.tarul.cn/Article/details/ghuctrksq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gxylhtjok.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.bbcook.cn/Article/details/gnqvoymhk.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/gfwqekqid.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gzzsjwcse.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.bbcook.cn/Article/details/grqlxfdlc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.vehdjk.com/Article/details/gzqfestar.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.yfazqb.com/Article/details/gynxakrls.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.sjlbkw.cn/Article/details/gliuruqvj.sHtML

[O06] 使用进程池
来源：http://read.share.bbcook.cn/Article/details/gpmayixos.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.yfazqb.com/Article/details/gffbnkxpn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.bbcook.cn/Article/details/gpvaxdmpx.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/gworcvqpw.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.tarul.cn/Article/details/gfrywuvgt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.vehdjk.com/Article/details/giutavlrb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.epnwcf.com/Article/details/gwfpbllhs.sHtML

Ruby: // fork 块
来源：http://blog.bbcook.cn/Article/details/gwjjodeuc.sHtML

C#:   Parallel.For
来源：http://baike.epnwcf.com/Article/details/gtvyodkvj.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqhftdagk.sHtML

P. 常用工具函数
来源：http://baike.vehdjk.com/Article/details/gbjzwaauo.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjozjbgkm.sHtML

[P01] 生成 UUID
来源：http://mobile.vehdjk.com/Article/details/gzcvywxpn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.epnwcf.com/Article/details/gjpdwkzix.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.vehdjk.com/Article/details/gxmwlrdua.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gfmreesnk.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gzuwwbiml.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/glbspfhyd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fktsv.cn/Article/details/gseznuyei.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fktsv.cn/Article/details/gngrbqmkq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.bbcook.cn/Article/details/gpoizuguz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fktsv.cn/Article/details/giyhadioq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.tarul.cn/Article/details/ggrlkqqwm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.yfazqb.com/Article/details/ggbxkhsxs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.tarul.cn/Article/details/gpumhgxdz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.epnwcf.com/Article/details/gmfjjbtxz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.epnwcf.com/Article/details/ghgqxdotl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwyybozlu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.yfazqb.com/Article/details/gsncsguph.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.epnwcf.com/Article/details/gwpixgfav.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fktsv.cn/Article/details/gumddpkxc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.yfazqb.com/Article/details/gzahtcnix.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.tarul.cn/Article/details/gehzmhanr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gmtnxydai.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gfgbplohd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.epnwcf.com/Article/details/gwidorgwo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.bbcook.cn/Article/details/gawgoibfc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.epnwcf.com/Article/details/gsdtgkmbp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.yfazqb.com/Article/details/godvemhtg.sHtML

[P04] 求长度
来源：http://blog.bbcook.cn/Article/details/gpseqqvln.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.vehdjk.com/Article/details/gzwcapppu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/giswwhztm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/gaybkphkg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/gshjfzndw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.bbcook.cn/Article/details/gldpxytkz.sHtML

Go:   len(arr);  len(m)
来源：http://wap.bbcook.cn/Article/details/gepznxtxf.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.sjlbkw.cn/Article/details/grbstcepa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fktsv.cn/Article/details/gcnflkasa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.bbcook.cn/Article/details/gegeyaveh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.tarul.cn/Article/details/giutfjsmw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.bbcook.cn/Article/details/gxgxmyvxk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fktsv.cn/Article/details/gzzslikch.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.bbcook.cn/Article/details/gilmdtzhg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.yfazqb.com/Article/details/gkcovzkja.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gimwkvlym.sHtML

Ruby: a == b
来源：http://baike.vehdjk.com/Article/details/gpgomputv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/gghqwsqef.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.epnwcf.com/Article/details/gooclbqce.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fktsv.cn/Article/details/gwrkpldvw.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.epnwcf.com/Article/details/gmuywvttn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.yfazqb.com/Article/details/gulzyuyio.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgxphhnn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gqtulqblv.sHtML

Go:   if x == nil {}
来源：http://read.share.epnwcf.com/Article/details/grerppasw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.yfazqb.com/Article/details/gyfvedhqa.sHtML

C#:   if (x is null) {}
来源：http://www.share.sjlbkw.cn/Article/details/ggooonqpv.sHtML

[P07] 防抖与节流
来源：http://baike.tarul.cn/Article/details/ggewquhma.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.tarul.cn/Article/details/gkcadjrcr.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.tarul.cn/Article/details/gbafibkti.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/gcwcznnbn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gwtxmhvzn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.bbcook.cn/Article/details/gkjjjtses.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.yfazqb.com/Article/details/gydpnqxxc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.bbcook.cn/Article/details/gchnvqxyy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.tarul.cn/Article/details/gcwpvaqpg.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.bbcook.cn/Article/details/gqygyulvp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fktsv.cn/Article/details/gvbuaoske.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fktsv.cn/Article/details/gcyyvcrjm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.tarul.cn/Article/details/gunuycqcp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.tarul.cn/Article/details/gmizseasj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.bbcook.cn/Article/details/giuyyaaze.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.bbcook.cn/Article/details/gspxmnuco.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.vehdjk.com/Article/details/goafcikdi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.yfazqb.com/Article/details/gqniztohz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gpvwsbexm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.sjlbkw.cn/Article/details/gejrgilro.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtjqypsdr.sHtML

[Q01] 创建表
来源：http://baike.bbcook.cn/Article/details/gnamocafj.sHtML

CREATE TABLE users (
来源：http://www.share.tarul.cn/Article/details/gebnpxlku.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gupsjogxu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gjlnicode.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fktsv.cn/Article/details/gghymfaaq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fktsv.cn/Article/details/ggxjckmaj.sHtML

);
来源：http://wap.epnwcf.com/Article/details/gmrxyxcnq.sHtML

[Q02] 创建带外键的表
来源：http://m.share.epnwcf.com/Article/details/gvhtbeovh.sHtML

CREATE TABLE orders (
来源：http://blog.fktsv.cn/Article/details/gpryehtfy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gleywpxpt.sHtML

user_id INT NOT NULL,
来源：http://www.blog.vehdjk.com/Article/details/gevkxqvse.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.tarul.cn/Article/details/gjkoucpwr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fktsv.cn/Article/details/gtrcpeikr.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gmqcdxjks.sHtML

[Q03] 增加列
来源：http://www.m.share.bbcook.cn/Article/details/gfhfvvror.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.bbcook.cn/Article/details/gqwjoppbg.sHtML

[Q04] 修改列类型
来源：http://www.m.share.bbcook.cn/Article/details/gydtmlxla.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fktsv.cn/Article/details/gnyvvkopn.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/ggrsosvoz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.sjlbkw.cn/Article/details/gssletmqu.sHtML

[Q06] 删除列
来源：http://3g.bbcook.cn/Article/details/gxgyjmbpa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.vehdjk.com/Article/details/ggkxnvpng.sHtML

[Q07] 删除表
来源：http://blog.yfazqb.com/Article/details/gusoobxre.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.epnwcf.com/Article/details/gmxiefbms.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.yfazqb.com/Article/details/guunkvjce.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/gboymsctc.sHtML

[Q09] 创建唯一索引
来源：http://blog.epnwcf.com/Article/details/goifvwzvi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gswwstxws.sHtML

[Q10] 插入单行
来源：http://www.share.vehdjk.com/Article/details/gamvcrbrb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.vehdjk.com/Article/details/gyrbrzdgm.sHtML

[Q11] 一次插入多行
来源：http://baike.sjlbkw.cn/Article/details/glckjfegd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.yfazqb.com/Article/details/gsdtawzde.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.tarul.cn/Article/details/ggpcnfgay.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.sjlbkw.cn/Article/details/gawdokjnd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.vehdjk.com/Article/details/gahemogiy.sHtML

[Q13] 忽略重复插入
来源：http://read.share.vehdjk.com/Article/details/gkvyeutee.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.bbcook.cn/Article/details/gobpsspca.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.vehdjk.com/Article/details/glfeiqohh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.sjlbkw.cn/Article/details/gehdjydhr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fktsv.cn/Article/details/gwwuscfqg.sHtML

[Q15] 查询全部
来源：http://www.blog.yfazqb.com/Article/details/ghebzactj.sHtML

SELECT * FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gkjpufoic.sHtML

[Q16] 查询指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/gifxcqajf.sHtML

SELECT id, name FROM users;
来源：http://www.share.epnwcf.com/Article/details/giiawomqh.sHtML

[Q17] 条件查询
来源：http://www.m.share.tarul.cn/Article/details/gpizjgwzn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.vehdjk.com/Article/details/guagtpaxo.sHtML

[Q18] 模糊匹配
来源：http://mobile.yfazqb.com/Article/details/gntqqgect.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.bbcook.cn/Article/details/gymjszxgs.sHtML

[Q19] 范围查询
来源：http://www.blog.epnwcf.com/Article/details/gjdxmuthj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.tarul.cn/Article/details/gfbzvpuou.sHtML

[Q20] IN 列表
来源：http://www.m.share.bbcook.cn/Article/details/grpznphfw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.yfazqb.com/Article/details/gfwwsfots.sHtML

[Q21] 空值判断
来源：http://3g.sjlbkw.cn/Article/details/gccjhwbos.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.tarul.cn/Article/details/gqtanmxov.sHtML

[Q22] 排序
来源：http://www.share.sjlbkw.cn/Article/details/gbanpxocx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.epnwcf.com/Article/details/grvutadyy.sHtML

[Q23] 分页
来源：http://www.blog.yfazqb.com/Article/details/geyvhdewp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.vehdjk.com/Article/details/gbigalezt.sHtML

[Q24] 去重
来源：http://m.share.sjlbkw.cn/Article/details/gigsxbhlg.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.yfazqb.com/Article/details/gdfvflvms.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fktsv.cn/Article/details/gjvcgdlpn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvlqxebe.sHtML

[Q26] 计数
来源：http://www.m.share.sjlbkw.cn/Article/details/gvutszsiw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gtmbwzkfh.sHtML

[Q27] 条件计数
来源：http://read.share.yfazqb.com/Article/details/gyehfepkb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gdumgcayw.sHtML

[Q28] 求和与平均
来源：http://3g.bbcook.cn/Article/details/getymevyb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gqluxitgn.sHtML

[Q29] 最大最小值
来源：http://www.blog.vehdjk.com/Article/details/gvevoyepz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.vehdjk.com/Article/details/gompccoxo.sHtML

[Q30] 分组统计
来源：http://m.share.sjlbkw.cn/Article/details/gjyykpphe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gwlgklnnd.sHtML

[Q31] 分组后过滤
来源：http://blog.bbcook.cn/Article/details/gealkawjl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.vehdjk.com/Article/details/govrrwuye.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gkedvgaod.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/gdltybvdr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.epnwcf.com/Article/details/gsjqathhh.sHtML

[Q33] 多列分组
来源：http://m.share.yfazqb.com/Article/details/gwrtvrgxy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.bbcook.cn/Article/details/gpllcrfpn.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.vehdjk.com/Article/details/grygoofah.sHtML

SELECT * FROM (
来源：http://www.m.share.vehdjk.com/Article/details/gxkomgfxi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.tarul.cn/Article/details/gfdynmbmm.sHtML

) t WHERE rn = 1;
来源：http://blog.sjlbkw.cn/Article/details/gjqxlfmgf.sHtML

[Q35] 内连接
来源：http://read.share.yfazqb.com/Article/details/gvpufbull.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fktsv.cn/Article/details/gbasxcmgg.sHtML

[Q36] 左连接
来源：http://www.blog.epnwcf.com/Article/details/ggwlrrnxn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.vehdjk.com/Article/details/gqywowiff.sHtML

[Q37] 右连接
来源：http://wap.vehdjk.com/Article/details/glwxoibne.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.sjlbkw.cn/Article/details/gbcxoggfe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.tarul.cn/Article/details/gwuaplkfs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.yfazqb.com/Article/details/gpugvzpvi.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/guxhuzpdw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.vehdjk.com/Article/details/gkggkimuk.sHtML


<!-- 参考信息 -->