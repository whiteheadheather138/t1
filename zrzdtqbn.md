代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lkk.ehwqpu.com

Ruby: warn "err"
来源：http://qsv.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://nst.tarul.cn

[M07] 判断是否为主入口
来源：http://bmw.guannengcc.top

Py:   if __name__ == "__main__":
来源：http://vgd.svipenyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lql.hcnkem.com

JS:   require.main === module
来源：http://mci.9152youxi.cn

TS:   require.main === module
来源：http://zuq.yfazqb.com

Java: public static void main(String[] args)
来源：http://tbq.iojbl.cn

Go:   func main()
来源：http://eqg.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gqz.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://itu.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://fkx.vehdjk.com

Py:   platform.system();  platform.python_version()
来源：http://yrs.epnwcf.com

PHP:  PHP_OS;  phpversion();
来源：http://vrv.pycfn.com

JS:   process.platform;  process.version
来源：http://mcv.shanyushiyangtech.top

TS:   process.platform;  process.version
来源：http://hjc.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bte.quarkkingdee.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tlz.jiagoushi.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://osc.chenlongwang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://otk.epnwcf.com

================================================================================
来源：http://cpv.jinyuanbaomall.cn

N. 数据结构与算法
来源：http://ikt.wangdashe.top

================================================================================
来源：http://jiu.jyoumei.cn

[N01] 二分查找（有序数组）
来源：http://adq.zhixingplan.top

Py:   bisect.bisect_left(arr, x)
来源：http://vvy.dianchejie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cmp.tanke756.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ggk.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gjy.haohaochexian.top

Java: Arrays.binarySearch(arr, x)
来源：http://aca.jinqigfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://wpe.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xkx.fengsongda.top

C#:   Array.BinarySearch(arr, x)
来源：http://ukc.yj20258.top

[N02] 排序（工程实践用内置实现）
来源：http://sjy.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://vte.xziqi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://drg.ywan-chungtsiang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lko.sjlbkw.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pvn.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bdp.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://cyy.aizwys.cn

Ruby: arr.sort
来源：http://lbv.vqdsnc.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uei.wangdashe.top

[N03] 快速排序（分治示例）
来源：http://dnh.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://spv.cdnleiting.top

PHP:  // 递归实现，或用 usort
来源：http://jsy.9152youxi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eqv.guowangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cgz.9152youxi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ayh.316326.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pnp.daria6918.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bkb.zhongyouzk.top

C#:   // 手写递归，或 Array.Sort
来源：http://knn.ybcxt.top

[N04] 斐波那契数列
来源：http://ymb.jlsjyb.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kgl.sweek.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zuy.nwbrower.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qsn.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bnk.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nnq.andypj.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://adu.yuxming.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uay.jlsjyb.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qsh.chenjidiqi.icu

[N05] 最大公约数
来源：http://nmh.kuanghao11.cn

Py:   math.gcd(a, b)
来源：http://yow.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jgz.hnxiangtu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wrh.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://krh.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mli.gzhubu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dxs.gzhubu.top

Ruby: a.gcd(b)
来源：http://uak.shangyingyoupin.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bfd.meibo888.top

[N06] 判断回文字符串
来源：http://hir.zdqjudy.top

Py:   s == s[::-1]
来源：http://tyy.fanxiaobao.xyz

PHP:  $s === strrev($s);
来源：http://eex.xinyue.icu

JS:   s === [...s].reverse().join("")
来源：http://fdw.xingfuxueyuan.xyz

TS:   s === [...s].reverse().join("")
来源：http://mln.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ipj.yueranfly.top

Go:   // 双指针从两端比较
来源：http://fuv.chenjidiqi.icu

Ruby: s == s.reverse
来源：http://yfx.yanxiufei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jzd.sweek.top

[N07] 两数之和（返回下标）
来源：http://ulb.kuanghao11.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vnn.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vdr.uphjek.com

JS:   // 手写 Map：map.set(v, i)
来源：http://gdf.ctjpmb.com

TS:   // 手写 Map<string, number>
来源：http://odo.sjlbkw.cn

Java: // 手写 HashMap
来源：http://ebr.chenlongwang.top

Go:   // 手写 map[int]int
来源：http://whv.jinghuilouyu.cn

Ruby: // 手写 Hash
来源：http://ngi.sysykeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://gfz.wangshuangyany.cn

[N08] 生成全排列
来源：http://fjk.yj20258.top

Py:   itertools.permutations(arr)
来源：http://svw.yanxiufei.cn

PHP:  // 手写递归交换
来源：http://mvc.hnqzz.top

JS:   // 手写回溯递归
来源：http://cis.mhx1999.top

TS:   // 手写回溯递归
来源：http://ywm.jlsjyb.cn

Java: // 手写回溯递归
来源：http://ijg.zycfv.cn

Go:   // 手写回溯递归
来源：http://sua.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://lht.xylfe.cn

C#:   // 手写回溯递归
来源：http://qkw.gogol.net.cn

[N09] 栈与队列
来源：http://qxz.9152youxi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tcy.sjlbkw.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fiv.cheryme.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aop.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ttl.fehbvm.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wou.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bkb.hcnkem.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kqc.guannengcc.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xho.hammf.cn

[N10] 链表节点定义
来源：http://ckt.cheryme.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lpq.fzhhl.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ewe.wangdashe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ukp.feifeiyinyue.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ryy.jqgufenzy.top

Java: class Node { int v; Node next; }
来源：http://pyv.ehwqpu.com

Go:   type Node struct { V int; Next *Node }
来源：http://fjc.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://run.shanyushiyangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://poe.hysaishi.cn

[N11] 二叉树中序遍历
来源：http://yvt.0kj1m.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hun.zhengqikj.top

PHP:  // 手写递归函数
来源：http://xrv.jinyuanbaomall.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lam.cdnleiting.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vuo.pycfn.com

Java: // 手写递归
来源：http://wad.hesvh.cn

Go:   // 手写递归
来源：http://lsk.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yjm.yueranfly.top

C#:   // 手写递归
来源：http://add.pycfn.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oan.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sbu.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hjr.havefunace.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eox.c1oappe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jxp.yj20258.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oan.vqdsnc.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hqm.zhongyouzk.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yfd.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sjw.birdmap.top

================================================================================
来源：http://exx.ctjpmb.com

O. 并发与异步
来源：http://qxk.ehwqpu.com

================================================================================
来源：http://jzy.ywan-chungtsiang.top

[O01] 启动一个线程
来源：http://jrk.jianghu66.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xuc.zhijiandao.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zgq.vehdjk.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oiu.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://lcs.zhaomingkeji.xyz

Java: new Thread(() -> f()).start()
来源：http://jey.zdqjudy.top

Go:   go f()
来源：http://iqa.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://lle.yangfankeji.com

C#:   Task.Run(() => F());
来源：http://dla.cheryme.top

[O02] 使用线程池
来源：http://pzc.zhoulong.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jhi.zhiwuduotai.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://can.nwbrower.top

JS:   // worker_threads 线程池
来源：http://nam.hongshengwenyu.top

TS:   // worker_threads 线程池
来源：http://wqc.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oty.zhoulong.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://apo.316326.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bax.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mcv.yuanzhike.top

[O03] 加锁保护共享数据
来源：http://ivj.fzhhl.top

Py:   with lock: shared += 1
来源：http://yqi.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://iln.yuanzhike.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wkr.birdmap.top

TS:   // 同 JS
来源：http://eul.nanxinkj.top

Java: synchronized (this) { shared++; }
来源：http://oxf.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dup.sweek.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://oon.vehdjk.com

C#:   lock (gate) { shared++; }
来源：http://gpb.epnwcf.com

[O04] 定义异步函数并等待
来源：http://jrk.nanxuanxn.top

Py:   async def f():⏎    await g()
来源：http://mvp.shanyushiyangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gcs.snrcjt.cn

JS:   async function f() { await g(); }
来源：http://nay.gogol.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://psk.sjlbkw.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rus.zhaomingkeji.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hop.cdnleiting.top

Ruby: # 用 Fiber 或 async gem
来源：http://yei.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://npd.316326.xyz

[O05] 并发执行并等待全部完成
来源：http://zhr.dianchejie.cn

Py:   asyncio.gather(*tasks)
来源：http://ozq.zhiwuduotai.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://enf.zhaomingkeji.xyz

JS:   await Promise.all(tasks)
来源：http://jls.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://fpt.ppjwa.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sja.snrcjt.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nhs.chenzaomai.com

Ruby: threads.map(&:join)
来源：http://qeg.gogol.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://odr.yuxming.cn

[O06] 使用进程池
来源：http://djz.jiagoushi.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hpq.chenzaomai.com

PHP:  // pcntl_fork 或多进程队列
来源：http://fgv.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://oit.shzxlz.cn

TS:   // child_process / cluster 模块
来源：http://jia.hysaishi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jzv.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mra.wangdashe.top

Ruby: // fork 块
来源：http://ipw.c1oappe.top

C#:   Parallel.For
来源：http://qtc.fzhhl.top

================================================================================
来源：http://kvr.kuanghao11.cn

P. 常用工具函数
来源：http://bao.hnqzz.top

================================================================================
来源：http://fnp.andypj.xyz

[P01] 生成 UUID
来源：http://pfh.vqdsnc.cn

Py:   str(uuid.uuid4())
来源：http://ffm.yuxming.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zsz.redwolf501.top

JS:   crypto.randomUUID()
来源：http://wwj.sufxvd.cn

TS:   crypto.randomUUID()
来源：http://hei.chenlongwang.top

Java: UUID.randomUUID().toString()
来源：http://tgw.redwolf501.top

Go:   // 用 github.com/google/uuid
来源：http://rkb.hongshengwenyu.top

Ruby: SecureRandom.uuid
来源：http://vac.xylfe.cn

C#:   Guid.NewGuid().ToString()
来源：http://nus.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://arf.zhengqikj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hwy.chenjidiqi.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://jlg.zhengqikj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xwd.ppjwa.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xqq.pengpengdd.cyou

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nrl.cqqwz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lov.gotoacloud.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mid.guannengcc.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lze.gogol.net.cn

[P03] 生成短随机字符串
来源：http://uqy.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ihj.hnxiangtu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nkq.fengsongda.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hvb.dianchejie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://klo.svipenyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qho.hcnkem.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tkb.xinyue.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://omd.yonumen.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mph.fzhhl.top

[P04] 求长度
来源：http://svr.sysykeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rbk.zdqjudy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dqp.zdbjq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ryf.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tfk.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://kkg.ydzc1.top

Go:   len(arr);  len(m)
来源：http://jmm.haohaochexian.top

Ruby: x.length;  x.size
来源：http://tqm.zhiwuduotai.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ozz.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://vdy.zhiwuduotai.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fhm.yueranfly.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ywr.9152youxi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://plr.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uxw.fktsv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mth.nwbrower.top

Go:   reflect.DeepEqual(a, b)
来源：http://jgq.9152youxi.cn

Ruby: a == b
来源：http://kkj.dashuyun.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jis.aizwys.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sdf.chenzaomai.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blk.316326.xyz

PHP:  if (empty($x)) {}
来源：http://kgo.cdnleiting.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lso.sysykeji.top

TS:   if (x == null) {}
来源：http://iol.gotoacloud.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fqb.vqdsnc.cn

Go:   if x == nil {}
来源：http://abs.iojbl.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ppp.hongshengwenyu.top

C#:   if (x is null) {}
来源：http://dvh.jinghuilouyu.cn

[P07] 防抖与节流
来源：http://wld.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wem.hongshengwenyu.top

PHP:  // 手写时间戳比较
来源：http://nya.jlsjyb.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qqg.wangdashe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ilw.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://udx.yj202588.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dth.smart0.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://xjm.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://unp.shanyushiyangtech.top

[P08] 处理浮点精度问题
来源：http://bvd.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kha.zdbjq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zvy.zhengqikj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mws.yfazqb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qyf.chenlongwang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gol.hfpthk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sju.chenzaomai.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sdt.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rug.nanxinkj.top

================================================================================
来源：http://afp.cashguo.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ypd.gogol.net.cn

================================================================================
来源：http://ijp.wangshuangyany.cn

[Q01] 创建表
来源：http://zgi.xuanzx.com

CREATE TABLE users (
来源：http://qzq.wangdashe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sup.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://hmo.gotoacloud.top

email VARCHAR(100) UNIQUE,
来源：http://hbj.kuanghao11.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xgi.jqgufenzy.top

);
来源：http://aro.mhx1999.top

[Q02] 创建带外键的表
来源：http://wxp.wangdashe.top

CREATE TABLE orders (
来源：http://oba.daria6918.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ewo.jianghu66.top

user_id INT NOT NULL,
来源：http://qui.chenjidiqi.icu

amount DECIMAL(10, 2),
来源：http://ier.hnxiangtu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ndg.zdqjudy.top

);
来源：http://cvn.chenlongwang.top

[Q03] 增加列
来源：http://awz.chenlongwang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vge.316326.xyz

[Q04] 修改列类型
来源：http://vrr.52xcode.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fhx.yuxming.cn

[Q05] 重命名列
来源：http://tur.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ctv.jyoumei.cn

[Q06] 删除列
来源：http://grp.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://fkk.haohaochexian.top

[Q07] 删除表
来源：http://vqb.jinyuanbaomall.cn

DROP TABLE IF EXISTS orders;
来源：http://xge.havefunace.top

[Q08] 创建普通索引
来源：http://fra.jlsjyb.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://byq.gzhubu.top

[Q09] 创建唯一索引
来源：http://knf.zhoulong.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gmb.yj202588.top

[Q10] 插入单行
来源：http://chd.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dkf.jianghu66.top

[Q11] 一次插入多行
来源：http://joo.smart0.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zwh.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://uhy.andypj.xyz


<!-- 参考信息 -->