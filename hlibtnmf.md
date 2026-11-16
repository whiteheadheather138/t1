代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://ugj.kuanghao11.cn

JS:   console.error("err")
来源：http://ant.nanxuanxn.top

TS:   console.error("err")
来源：http://otm.quarkkingdee.top

Java: System.err.println("err")
来源：http://yyy.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nmy.zhijiandao.cn

Ruby: warn "err"
来源：http://apd.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://hxf.zhongyouzk.top

[M07] 判断是否为主入口
来源：http://och.zhijiandao.cn

Py:   if __name__ == "__main__":
来源：http://dqu.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://evg.jinghuilouyu.cn

JS:   require.main === module
来源：http://wol.jianghu66.top

TS:   require.main === module
来源：http://idx.wangdashe.top

Java: public static void main(String[] args)
来源：http://epu.uphjek.com

Go:   func main()
来源：http://ruo.snrcjt.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dmk.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://ioz.shzxlz.cn

[M08] 获取系统与运行时信息
来源：http://edb.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://ajg.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://isk.vehdjk.com

JS:   process.platform;  process.version
来源：http://sgz.zhaomingkeji.xyz

TS:   process.platform;  process.version
来源：http://mbj.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wrz.jlsjyb.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hdi.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://epq.fanxiaobao.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://npf.uphjek.com

================================================================================
来源：http://msv.sjlbkw.cn

N. 数据结构与算法
来源：http://tie.fanxiaobao.xyz

================================================================================
来源：http://nxy.tarul.cn

[N01] 二分查找（有序数组）
来源：http://gey.bjfxy.top

Py:   bisect.bisect_left(arr, x)
来源：http://aoe.jinghuilouyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vud.yanxiufei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qal.ehwqpu.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xmg.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://nri.xinyue.icu

Go:   sort.SearchInts(arr, x)
来源：http://fmz.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xbc.shanyushiyangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://obp.gotoacloud.top

[N02] 排序（工程实践用内置实现）
来源：http://zmu.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://edv.vqdsnc.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tri.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bqv.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gmx.nanxinkj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kss.cheryme.top

Go:   slices.Sort(arr)
来源：http://ftk.wangshuangyany.cn

Ruby: arr.sort
来源：http://lxt.zhijiandao.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uri.jinghuilouyu.cn

[N03] 快速排序（分治示例）
来源：http://twq.guannengcc.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jak.smart0.xyz

PHP:  // 递归实现，或用 usort
来源：http://wem.yj20258.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fwg.yongpay.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://est.andypj.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kbf.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ghs.cashguo.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ftn.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://cfx.c1oappe.top

[N04] 斐波那契数列
来源：http://kgt.gaohongyu789.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ydm.yj202588.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xrj.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bwe.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cby.ybcxt.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eux.bjfxy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://obg.tianlin.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uoq.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mid.sjlbkw.cn

[N05] 最大公约数
来源：http://ath.meibo888.top

Py:   math.gcd(a, b)
来源：http://xce.feifeiyinyue.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eui.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wou.shzxlz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hvo.sufxvd.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pqg.jinqigfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://icj.0kj1m.cn

Ruby: a.gcd(b)
来源：http://uxv.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eea.zhijiandao.cn

[N06] 判断回文字符串
来源：http://qmq.jlsjyb.cn

Py:   s == s[::-1]
来源：http://wlq.pycfn.com

PHP:  $s === strrev($s);
来源：http://fbj.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://mpf.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://zmi.wangdashe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wfm.tian-w.cn

Go:   // 双指针从两端比较
来源：http://mru.kuanghao11.cn

Ruby: s == s.reverse
来源：http://rvy.gaohongyu789.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://edo.nwbrower.top

[N07] 两数之和（返回下标）
来源：http://wmz.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ezv.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bfa.haohaochexian.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dnm.vqdsnc.cn

TS:   // 手写 Map<string, number>
来源：http://xal.dianchejie.cn

Java: // 手写 HashMap
来源：http://dfe.zdbjq.cn

Go:   // 手写 map[int]int
来源：http://wrg.gogol.net.cn

Ruby: // 手写 Hash
来源：http://pko.chenlongwang.top

C#:   // 手写 Dictionary<int, int>
来源：http://eiy.chenzaomai.com

[N08] 生成全排列
来源：http://zok.fktsv.cn

Py:   itertools.permutations(arr)
来源：http://tni.cdnleiting.top

PHP:  // 手写递归交换
来源：http://tco.tian-w.cn

JS:   // 手写回溯递归
来源：http://mcf.yj20258.top

TS:   // 手写回溯递归
来源：http://lar.ctjpmb.com

Java: // 手写回溯递归
来源：http://hmv.fehbvm.com

Go:   // 手写回溯递归
来源：http://jjm.sysykeji.top

Ruby: arr.permutation.to_a
来源：http://yyw.nwbrower.top

C#:   // 手写回溯递归
来源：http://emt.shanyushiyangkeji.top

[N09] 栈与队列
来源：http://gvh.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jym.svipenyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fcx.hnqzz.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zdu.fzhhl.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wuc.tarul.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vgo.zdqjudy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xeo.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fwq.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bqd.chenjidiqi.icu

[N10] 链表节点定义
来源：http://gmr.uphjek.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ruo.xingfuxueyuan.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://ayy.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wmz.cheryme.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tnr.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://tvb.zhoulong.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://cck.jiagoushi.top

Ruby: Node = Struct.new(:v, :next)
来源：http://roz.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uce.dashuyun.cn

[N11] 二叉树中序遍历
来源：http://yye.havefunace.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zhy.yj20258888.top

PHP:  // 手写递归函数
来源：http://vxm.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ort.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qoy.ydjk.org.cn

Java: // 手写递归
来源：http://avy.cdnleiting.top

Go:   // 手写递归
来源：http://ecg.fzhhl.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vxi.cashguo.top

C#:   // 手写递归
来源：http://kyb.daria6918.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://juk.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vlt.nwbrower.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zuk.tarul.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pqi.snrcjt.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hiq.redwolf501.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uqj.jianghu66.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fcw.shanyushiyangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xni.fehbvm.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aqm.fengsongda.top

================================================================================
来源：http://rpw.yj20258888.top

O. 并发与异步
来源：http://hgy.meibo888.top

================================================================================
来源：http://otq.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://ick.yj20258888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uey.epnwcf.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dnl.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iho.zhengqikj.top

TS:   // 同 JS
来源：http://znf.jqgufenzy.top

Java: new Thread(() -> f()).start()
来源：http://erx.zhongyouzk.top

Go:   go f()
来源：http://aku.guannengcc.top

Ruby: Thread.new { f }
来源：http://ffh.chenlongwang.top

C#:   Task.Run(() => F());
来源：http://zsz.yj20258.top

[O02] 使用线程池
来源：http://mbl.hammf.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yuq.xziqi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hju.mhx1999.top

JS:   // worker_threads 线程池
来源：http://bjj.ydzc1.top

TS:   // worker_threads 线程池
来源：http://lgj.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ibl.gotoacloud.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lec.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vks.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://clg.nanxuanxn.top

[O03] 加锁保护共享数据
来源：http://quj.zhongyouzk.top

Py:   with lock: shared += 1
来源：http://jij.xingfuxueyuan.xyz

PHP:  // 用 flock() 做文件锁
来源：http://bvs.ybcxt.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vah.kuanghao11.cn

TS:   // 同 JS
来源：http://svi.dashuyun.cn

Java: synchronized (this) { shared++; }
来源：http://mer.hesvh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lfw.hcnkem.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://bln.birdmap.top

C#:   lock (gate) { shared++; }
来源：http://xns.chenlongwang.top

[O04] 定义异步函数并等待
来源：http://poe.xuetiantiany.cn

Py:   async def f():⏎    await g()
来源：http://sqr.ppjwa.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xcj.nanxinkj.top

JS:   async function f() { await g(); }
来源：http://neq.iojbl.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://woa.jinghuilouyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://amg.havefunace.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://svr.cucudq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qel.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://grw.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://pdz.0kj1m.cn

Py:   asyncio.gather(*tasks)
来源：http://irt.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yub.yj202588.top

JS:   await Promise.all(tasks)
来源：http://wks.zhixingplan.top

TS:   await Promise.all(tasks)
来源：http://wjz.jinqigufen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ywp.xziqi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ode.c1oappe.top

Ruby: threads.map(&:join)
来源：http://yho.ppjwa.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pos.zhiwuduotai.top

[O06] 使用进程池
来源：http://qmt.tianlin.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qgs.xziqi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://omx.gotoacloud.top

JS:   // child_process / cluster 模块
来源：http://vvq.cucudq.cn

TS:   // child_process / cluster 模块
来源：http://tiw.shanyushiyangtech.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sti.zhaomingkeji.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vhp.yanxiufei.cn

Ruby: // fork 块
来源：http://ocs.nwbrower.top

C#:   Parallel.For
来源：http://dje.jinyuanbaomall.cn

================================================================================
来源：http://ijg.hesvh.cn

P. 常用工具函数
来源：http://cii.wangshuangyany.cn

================================================================================
来源：http://ifu.hcnkem.com

[P01] 生成 UUID
来源：http://rcp.zdqjudy.top

Py:   str(uuid.uuid4())
来源：http://cfs.bbcook.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dsu.yfazqb.com

JS:   crypto.randomUUID()
来源：http://rlv.shzxlz.cn

TS:   crypto.randomUUID()
来源：http://ecw.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://hna.epnwcf.com

Go:   // 用 github.com/google/uuid
来源：http://hjp.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://dxc.yuxming.cn

C#:   Guid.NewGuid().ToString()
来源：http://jnz.hnxiangtu.top

[P02] MD5 / SHA256 摘要
来源：http://mnd.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mob.fehbvm.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://cbn.wangdashe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cqs.nanxinkj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yfw.jyoumei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vhv.zhongyouzk.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vyy.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pmm.redwolf501.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ilb.vehdjk.com

[P03] 生成短随机字符串
来源：http://zpz.pycfn.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ysk.dashuyun.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://asm.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xfk.hywenlv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://irl.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://npi.sweek.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hhn.zhengqikj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nml.yangfankeji.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://udr.jiagoushi.top

[P04] 求长度
来源：http://dxd.cdnleiting.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://msy.yuxming.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://smc.0kj1m.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jgs.xinyue.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fqw.havefunace.top

Java: list.size();  map.size();  s.length()
来源：http://dvp.zhijiandao.cn

Go:   len(arr);  len(m)
来源：http://vsh.guannengcc.top

Ruby: x.length;  x.size
来源：http://llc.zhixingplan.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jws.hfpthk.cn

[P05] 判断两个对象内容是否相等
来源：http://fas.jiagoushi.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dch.haohaochexian.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ziz.zdqjudy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://onj.nanxinkj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://feo.yonumen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bgp.xingfuxueyuan.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://rzu.sxryk.cn

Ruby: a == b
来源：http://hjr.xingfuxueyuan.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dus.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jqk.316326.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iam.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://vel.xuanzx.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uau.yvedp.cn

TS:   if (x == null) {}
来源：http://hsu.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ujw.bjfxy.top

Go:   if x == nil {}
来源：http://dza.wangdashe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://god.gotoacloud.top

C#:   if (x is null) {}
来源：http://huz.jqgufenzy.top

[P07] 防抖与节流
来源：http://szr.uphjek.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aqf.guannengcc.top

PHP:  // 手写时间戳比较
来源：http://jxj.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hhg.52xcode.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://abz.dashuyun.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bnx.jinqigufen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bag.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jxj.shanyushiyangtech.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vzq.vehdjk.com

[P08] 处理浮点精度问题
来源：http://cjj.kuanghao11.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://okm.zhoulong.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xyt.jinghuilouyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://upc.hnqzz.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://syo.yvedp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mqk.quarkkingdee.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://old.chenzaomai.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://osm.ydzc1.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://inx.yj20258.top

================================================================================
来源：http://get.tarul.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dsp.yj202588.top

================================================================================
来源：http://jwp.snrcjt.cn

[Q01] 创建表
来源：http://byg.uphjek.com

CREATE TABLE users (
来源：http://sww.sysykeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://urv.xinyue.icu

name VARCHAR(50) NOT NULL,
来源：http://uzb.hysaishi.cn

email VARCHAR(100) UNIQUE,
来源：http://aaq.hongshengwenyu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lnf.fktsv.cn

);
来源：http://hef.52xcode.cn

[Q02] 创建带外键的表
来源：http://lcl.ydzc1.top

CREATE TABLE orders (
来源：http://fkr.iojbl.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bcy.jyoumei.cn

user_id INT NOT NULL,
来源：http://fgr.hcnkem.com

amount DECIMAL(10, 2),
来源：http://bnm.chenzaomai.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mme.jqgfzy.top

);
来源：http://bzk.0kj1m.cn

[Q03] 增加列
来源：http://htc.tian-w.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tgb.hammf.cn

[Q04] 修改列类型
来源：http://dpp.ctjpmb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mjs.vehdjk.com

[Q05] 重命名列
来源：http://ykn.feifeiyinyue.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wpi.zycfv.cn

[Q06] 删除列
来源：http://ijh.hnqzz.top

ALTER TABLE users DROP COLUMN age;
来源：http://mbt.xziqi.cn

[Q07] 删除表
来源：http://hpm.tanke756.top

DROP TABLE IF EXISTS orders;
来源：http://cpo.zdqjudy.top

[Q08] 创建普通索引
来源：http://ugs.daria6918.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xqk.ydzc1.top

[Q09] 创建唯一索引
来源：http://ztg.vehdjk.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://laq.dianchejie.cn

[Q10] 插入单行
来源：http://phn.hesvh.cn


<!-- 参考信息 -->