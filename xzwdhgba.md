代发 wailian999

Py:   if __name__ == "__main__":
来源：http://hiw.vehdjk.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vbz.yj20258.top

JS:   require.main === module
来源：http://hze.sysykeji.top

TS:   require.main === module
来源：http://nvc.birdmap.top

Java: public static void main(String[] args)
来源：http://pyl.chenlongwang.top

Go:   func main()
来源：http://lmn.yueranfly.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bce.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://uhs.shuidangran.top

[M08] 获取系统与运行时信息
来源：http://ksh.9152youxi.cn

Py:   platform.system();  platform.python_version()
来源：http://fkb.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://hhz.hesvh.cn

JS:   process.platform;  process.version
来源：http://cmg.shanyushiyangtech.top

TS:   process.platform;  process.version
来源：http://pxp.sxryk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bod.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://liw.hysaishi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uek.havefunace.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://pvt.guowangkeji.top

================================================================================
来源：http://hcd.hywenlv.cn

N. 数据结构与算法
来源：http://vsq.zdbjq.cn

================================================================================
来源：http://eby.cqqwz.cn

[N01] 二分查找（有序数组）
来源：http://sfd.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xov.guowangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lpk.daxiang520.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zgm.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xal.yfazqb.com

Java: Arrays.binarySearch(arr, x)
来源：http://dac.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://ygm.jianghu66.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rlc.tanke756.top

C#:   Array.BinarySearch(arr, x)
来源：http://ocx.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://cwe.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://xyg.9152youxi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gnv.yanxiufei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lch.yangfankeji.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://emj.jinqigfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eib.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://wik.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://eed.vqdsnc.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hts.epnwcf.com

[N03] 快速排序（分治示例）
来源：http://dvx.hnqzz.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gyw.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://ica.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wrk.jinqigufen.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sqi.yanxiufei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fjt.shuidangran.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://plh.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dxg.shangyingyoupin.top

C#:   // 手写递归，或 Array.Sort
来源：http://xat.9152youxi.cn

[N04] 斐波那契数列
来源：http://ebz.tian-w.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://amx.cdnleiting.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lkn.fanxiaobao.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lty.chenzaomai.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mch.cucudq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qkm.hnqzz.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jyl.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hib.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fub.daria6918.cn

[N05] 最大公约数
来源：http://uhd.bjfxy.top

Py:   math.gcd(a, b)
来源：http://jdy.bbcook.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kxd.jianghu66.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eor.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xyn.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rac.yuxming.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zwi.wangshuangyany.cn

Ruby: a.gcd(b)
来源：http://thf.zhengqikj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mbt.jinyuanbaomall.cn

[N06] 判断回文字符串
来源：http://uka.yonumen.top

Py:   s == s[::-1]
来源：http://veu.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://acn.jqgufenzy.top

JS:   s === [...s].reverse().join("")
来源：http://jeh.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://ifu.yonumen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rzg.bbcook.cn

Go:   // 双指针从两端比较
来源：http://mku.316326.xyz

Ruby: s == s.reverse
来源：http://coi.fehbvm.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://dul.jiagoushi.top

[N07] 两数之和（返回下标）
来源：http://hvo.zdbjq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hqx.meibo888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gmd.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wbk.smart0.xyz

TS:   // 手写 Map<string, number>
来源：http://wkg.yongpay.top

Java: // 手写 HashMap
来源：http://rns.hywenlv.cn

Go:   // 手写 map[int]int
来源：http://pho.vehdjk.com

Ruby: // 手写 Hash
来源：http://wcn.svipenyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cba.chenlongwang.top

[N08] 生成全排列
来源：http://adn.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://jzm.c1oappe.top

PHP:  // 手写递归交换
来源：http://zgo.daria6918.cn

JS:   // 手写回溯递归
来源：http://bvg.ybcxt.top

TS:   // 手写回溯递归
来源：http://hmr.gotoacloud.top

Java: // 手写回溯递归
来源：http://wzb.ppjwa.cn

Go:   // 手写回溯递归
来源：http://xuj.ybcxt.top

Ruby: arr.permutation.to_a
来源：http://kfy.yonumen.top

C#:   // 手写回溯递归
来源：http://kmw.zhijiandao.cn

[N09] 栈与队列
来源：http://fqt.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://njt.sjlbkw.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vjj.sxryk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cwi.ydjk.org.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ywb.ywan-chungtsiang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ptj.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bqs.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bji.uphjek.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kuf.gaohongyu789.top

[N10] 链表节点定义
来源：http://pwz.xziqi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rou.shangyingyoupin.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rzt.cqqwz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lyf.hnqzz.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://txs.zhongyouzk.top

Java: class Node { int v; Node next; }
来源：http://egz.yuanzhike.top

Go:   type Node struct { V int; Next *Node }
来源：http://dvn.vqdsnc.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fto.xingfuxueyuan.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://cly.sysykeji.top

[N11] 二叉树中序遍历
来源：http://tee.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://das.yongpay.top

PHP:  // 手写递归函数
来源：http://uhx.aizwys.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zgi.daxiang520.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://onx.yj20258.top

Java: // 手写递归
来源：http://maf.jqgfzy.top

Go:   // 手写递归
来源：http://qak.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dls.sjlbkw.cn

C#:   // 手写递归
来源：http://yhr.hfpthk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hbx.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ojp.guowangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hxs.chenjidiqi.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hzs.nwbrower.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kol.yongpay.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ned.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yis.jinghuilouyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hlj.zhiwuduotai.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hgk.guowangkeji.top

================================================================================
来源：http://cuw.svipenyu.cn

O. 并发与异步
来源：http://alj.redwolf501.top

================================================================================
来源：http://gau.fengsongda.top

[O01] 启动一个线程
来源：http://hta.yangfankeji.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uzu.shangyingyoupin.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mkx.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lbf.yj20258.top

TS:   // 同 JS
来源：http://kov.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://xfm.aibaodan.cn

Go:   go f()
来源：http://son.c1oappe.top

Ruby: Thread.new { f }
来源：http://xur.redwolf501.top

C#:   Task.Run(() => F());
来源：http://jjh.iojbl.cn

[O02] 使用线程池
来源：http://zzq.xylfe.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pmb.ivvv.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://csb.jyoumei.cn

JS:   // worker_threads 线程池
来源：http://chy.xziqi.cn

TS:   // worker_threads 线程池
来源：http://dhf.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://vkz.ctjpmb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bhb.ywan-chungtsiang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qcp.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ocn.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://yko.fzhhl.top

Py:   with lock: shared += 1
来源：http://yhj.c1oappe.top

PHP:  // 用 flock() 做文件锁
来源：http://bia.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jkz.fanxiaobao.xyz

TS:   // 同 JS
来源：http://dcv.9152youxi.cn

Java: synchronized (this) { shared++; }
来源：http://tzk.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gfp.bbcook.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ryr.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://zyi.vqdsnc.cn

[O04] 定义异步函数并等待
来源：http://pil.cdnleiting.top

Py:   async def f():⏎    await g()
来源：http://pyd.ivvv.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bsl.yfazqb.com

JS:   async function f() { await g(); }
来源：http://bzo.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://nsh.hywenlv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uju.cucudq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pkf.yonumen.top

Ruby: # 用 Fiber 或 async gem
来源：http://ldr.yj20258.top

C#:   async Task F() { await G(); }
来源：http://pbi.ppjwa.cn

[O05] 并发执行并等待全部完成
来源：http://era.ywan-chungtsiang.top

Py:   asyncio.gather(*tasks)
来源：http://amq.hesvh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kos.jyoumei.cn

JS:   await Promise.all(tasks)
来源：http://hti.uphjek.com

TS:   await Promise.all(tasks)
来源：http://ipx.zhiwuduotai.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bau.tian-w.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ggw.feifeiyinyue.top

Ruby: threads.map(&:join)
来源：http://hin.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://srd.mhx1999.top

[O06] 使用进程池
来源：http://xyy.jinqigfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jgl.jinyuanbaomall.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xfu.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://qkc.hnqzz.top

TS:   // child_process / cluster 模块
来源：http://drx.jinqigufen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://luq.fzhhl.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gmt.jinqigfzy.top

Ruby: // fork 块
来源：http://bng.yuanzhike.top

C#:   Parallel.For
来源：http://lgp.shangyingyoupin.top

================================================================================
来源：http://atl.kuanghao11.cn

P. 常用工具函数
来源：http://qhj.vqdsnc.cn

================================================================================
来源：http://lze.zhengqikj.top

[P01] 生成 UUID
来源：http://gvu.zdbjq.cn

Py:   str(uuid.uuid4())
来源：http://vef.gaohongyu789.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jia.hesvh.cn

JS:   crypto.randomUUID()
来源：http://uvo.redwolf501.top

TS:   crypto.randomUUID()
来源：http://cdj.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://cqp.ybcxt.top

Go:   // 用 github.com/google/uuid
来源：http://szb.zhoulong.xyz

Ruby: SecureRandom.uuid
来源：http://bkc.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://bnw.meibo888.top

[P02] MD5 / SHA256 摘要
来源：http://ysj.dashuyun.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ziy.shanyushiyangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vhb.zhijiandao.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kyc.quarkkingdee.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ism.svipenyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lax.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bvu.birdmap.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vrs.yonumen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://epd.guannengcc.top

[P03] 生成短随机字符串
来源：http://ybn.chenzaomai.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zxt.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pmn.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lwi.jqgfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ewb.zycfv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jra.ydzc1.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://okj.smart0.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://xlk.jyoumei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iig.ywan-chungtsiang.top

[P04] 求长度
来源：http://ymu.jlsjyb.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ptt.cucudq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vbw.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rov.ppjwa.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kwj.xziqi.cn

Java: list.size();  map.size();  s.length()
来源：http://fdf.redwolf501.top

Go:   len(arr);  len(m)
来源：http://zbr.yangfankeji.com

Ruby: x.length;  x.size
来源：http://bam.zhongyouzk.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qpt.ydjk.org.cn

[P05] 判断两个对象内容是否相等
来源：http://wbf.mhx1999.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yal.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wqo.ydzc1.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hlw.jinghuilouyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qoo.zhongyouzk.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wcf.jinyuanbaomall.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dzz.yuanzhike.top

Ruby: a == b
来源：http://ugq.jqgufenzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uvt.shanyushiyangtech.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xzr.yueranfly.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jzj.jianghu66.top

PHP:  if (empty($x)) {}
来源：http://zqn.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vud.guannengcc.top

TS:   if (x == null) {}
来源：http://lcv.chenlongwang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rib.316326.xyz

Go:   if x == nil {}
来源：http://onu.chenlongwang.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mdk.fzhhl.top

C#:   if (x is null) {}
来源：http://xaf.sweek.top

[P07] 防抖与节流
来源：http://lvt.ydjk.org.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gqd.jinqigfzy.top

PHP:  // 手写时间戳比较
来源：http://emp.ydjk.org.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xor.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cqo.cheryme.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zbj.c1oappe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ymc.yangfankeji.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://bjh.zhixingplan.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://shh.shanyushiyangtech.top

[P08] 处理浮点精度问题
来源：http://pvu.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mwp.jqgufenzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xes.jyoumei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tup.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ipm.xinyue.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lvs.snrcjt.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gwo.0kj1m.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aaj.fktsv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dxr.sysykeji.top

================================================================================
来源：http://wqn.cucudq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aps.zhongyouzk.top

================================================================================
来源：http://mfq.fanxiaobao.xyz

[Q01] 创建表
来源：http://ptd.gaohongyu789.top

CREATE TABLE users (
来源：http://gze.ywan-chungtsiang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gvt.fktsv.cn

name VARCHAR(50) NOT NULL,
来源：http://vlq.fktsv.cn

email VARCHAR(100) UNIQUE,
来源：http://wgp.wangshuangyany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pkl.svipenyu.cn

);
来源：http://scd.nwbrower.top

[Q02] 创建带外键的表
来源：http://mvg.zhiwuduotai.top

CREATE TABLE orders (
来源：http://rcw.zdbjq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tqk.yuanzhike.top

user_id INT NOT NULL,
来源：http://qgz.hfpthk.cn

amount DECIMAL(10, 2),
来源：http://goc.tanke756.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yyj.gzhubu.top

);
来源：http://zmr.c1oappe.top

[Q03] 增加列
来源：http://cbz.guowangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hui.daria6918.cn

[Q04] 修改列类型
来源：http://jtw.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gmz.ywan-chungtsiang.top

[Q05] 重命名列
来源：http://lyb.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blr.tianlin.xyz

[Q06] 删除列
来源：http://qph.nanxinkj.top

ALTER TABLE users DROP COLUMN age;
来源：http://mzf.fanxiaobao.xyz

[Q07] 删除表
来源：http://qww.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://zsb.jqgfzy.top

[Q08] 创建普通索引
来源：http://wks.fengsongda.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pnu.316326.xyz

[Q09] 创建唯一索引
来源：http://oba.yangfankeji.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zok.zycfv.cn

[Q10] 插入单行
来源：http://tmy.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yqg.zhoulong.xyz

[Q11] 一次插入多行
来源：http://yaj.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zhg.hfpthk.cn

[Q12] 插入后取自增 ID
来源：http://hmt.zdqjudy.top

INSERT INTO users (name) VALUES ('C');
来源：http://uoh.svipenyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qeo.dashuyun.cn

[Q13] 忽略重复插入
来源：http://zxz.zhoulong.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zpn.ybcxt.top


<!-- 参考信息 -->