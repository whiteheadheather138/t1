代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://utd.yfazqb.com

JS:   console.error("err")
来源：http://yaa.kuanghao11.cn

TS:   console.error("err")
来源：http://scr.hongshengwenyu.top

Java: System.err.println("err")
来源：http://lzt.ehwqpu.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dlo.yonumen.top

Ruby: warn "err"
来源：http://kiw.dianchejie.cn

C#:   Console.Error.WriteLine("err")
来源：http://ehl.yj20258888.top

[M07] 判断是否为主入口
来源：http://moo.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://kya.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hay.aizwys.cn

JS:   require.main === module
来源：http://ike.daria6918.cn

TS:   require.main === module
来源：http://qtn.sufxvd.cn

Java: public static void main(String[] args)
来源：http://urv.gaohongyu789.top

Go:   func main()
来源：http://khk.daxiang520.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rau.chenlongwang.top

C#:   static void Main(string[] args)
来源：http://brb.zhengqikj.top

[M08] 获取系统与运行时信息
来源：http://paj.c1oappe.top

Py:   platform.system();  platform.python_version()
来源：http://hjd.jyoumei.cn

PHP:  PHP_OS;  phpversion();
来源：http://trt.gzhubu.top

JS:   process.platform;  process.version
来源：http://sdi.hcnkem.com

TS:   process.platform;  process.version
来源：http://miv.gzhubu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tmq.ivvv.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mzh.yj20258.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nag.yanxiufei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pae.ybcxt.top

================================================================================
来源：http://maf.aibaodan.cn

N. 数据结构与算法
来源：http://rrb.yuanzhike.top

================================================================================
来源：http://ffv.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://cok.sufxvd.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kqu.cdnleiting.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eyl.yj20258888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qpf.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rqc.iojbl.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fad.jinqigufen.top

Go:   sort.SearchInts(arr, x)
来源：http://axz.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://xdw.yvedp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hlx.tianlin.xyz

[N02] 排序（工程实践用内置实现）
来源：http://mhx.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://mrh.yvedp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kqo.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mme.havefunace.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ryz.0kj1m.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rzz.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://kvw.zhoulong.xyz

Ruby: arr.sort
来源：http://sym.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dxi.epnwcf.com

[N03] 快速排序（分治示例）
来源：http://tit.pycfn.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wpo.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://axl.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ktq.sufxvd.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tca.birdmap.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iki.hongshengwenyu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://znq.yj20258888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nuo.hcnkem.com

C#:   // 手写递归，或 Array.Sort
来源：http://uly.ppjwa.cn

[N04] 斐波那契数列
来源：http://bet.ctjpmb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wmo.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nfg.smart0.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rcy.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pzb.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aqw.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://igj.kuanghao11.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ixj.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xmc.nwbrower.top

[N05] 最大公约数
来源：http://fpq.svipenyu.cn

Py:   math.gcd(a, b)
来源：http://phc.shzxlz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bvj.jqgfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pdw.redwolf501.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tch.vqdsnc.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cve.shuidangran.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ckn.zhaomingkeji.xyz

Ruby: a.gcd(b)
来源：http://kmm.fzhhl.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mii.iojbl.cn

[N06] 判断回文字符串
来源：http://abd.dashuyun.cn

Py:   s == s[::-1]
来源：http://jzs.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://vud.zhaomingkeji.xyz

JS:   s === [...s].reverse().join("")
来源：http://twh.aibaodan.cn

TS:   s === [...s].reverse().join("")
来源：http://dij.smart0.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iqa.guannengcc.top

Go:   // 双指针从两端比较
来源：http://oyt.ybcxt.top

Ruby: s == s.reverse
来源：http://mqu.cqqwz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zpi.cdnleiting.top

[N07] 两数之和（返回下标）
来源：http://agk.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kjd.hnxiangtu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xnx.fzhhl.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rkb.xuetiantiany.cn

TS:   // 手写 Map<string, number>
来源：http://ojc.aibaodan.cn

Java: // 手写 HashMap
来源：http://lfw.ppjwa.cn

Go:   // 手写 map[int]int
来源：http://ltv.fehbvm.com

Ruby: // 手写 Hash
来源：http://wql.zhijiandao.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nwc.xuetiantiany.cn

[N08] 生成全排列
来源：http://uxp.nanxuanxn.top

Py:   itertools.permutations(arr)
来源：http://zpo.vqdsnc.cn

PHP:  // 手写递归交换
来源：http://gqs.jyoumei.cn

JS:   // 手写回溯递归
来源：http://qib.hammf.cn

TS:   // 手写回溯递归
来源：http://end.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://mxy.pycfn.com

Go:   // 手写回溯递归
来源：http://xlc.jqgufenzy.top

Ruby: arr.permutation.to_a
来源：http://dun.iojbl.cn

C#:   // 手写回溯递归
来源：http://ofy.zdqjudy.top

[N09] 栈与队列
来源：http://yyw.dianchejie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rqj.yangfankeji.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vhu.shuidangran.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ghr.andypj.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sis.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ptw.fanxiaobao.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ylv.zhoulong.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gvi.316326.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://moi.gogol.net.cn

[N10] 链表节点定义
来源：http://jtb.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dqw.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pyz.quarkkingdee.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ptr.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://meg.hesvh.cn

Java: class Node { int v; Node next; }
来源：http://pgc.zhongyouzk.top

Go:   type Node struct { V int; Next *Node }
来源：http://atb.tanke756.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zxc.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wue.chenlongwang.top

[N11] 二叉树中序遍历
来源：http://olm.meibo888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://koz.nanxinkj.top

PHP:  // 手写递归函数
来源：http://loo.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mys.chenlongwang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wcu.jlsjyb.cn

Java: // 手写递归
来源：http://xrr.jlsjyb.cn

Go:   // 手写递归
来源：http://ejl.tian-w.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xyy.fktsv.cn

C#:   // 手写递归
来源：http://kwe.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fbr.meibo888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vod.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jzc.jinqigufen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hyj.fengsongda.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qkr.zhiwuduotai.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jqr.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kak.daxiang520.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tse.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dxr.hongshengwenyu.top

================================================================================
来源：http://qzb.hongshengwenyu.top

O. 并发与异步
来源：http://tbr.ybcxt.top

================================================================================
来源：http://azl.cheryme.top

[O01] 启动一个线程
来源：http://jvo.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xgu.cheryme.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ktj.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lam.pengpengdd.cyou

TS:   // 同 JS
来源：http://xgm.shangyingyoupin.top

Java: new Thread(() -> f()).start()
来源：http://ovb.andypj.xyz

Go:   go f()
来源：http://nfy.wangdashe.top

Ruby: Thread.new { f }
来源：http://vtl.sjlbkw.cn

C#:   Task.Run(() => F());
来源：http://iko.shanyushiyangkeji.top

[O02] 使用线程池
来源：http://bgc.xziqi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kxc.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ata.gotoacloud.top

JS:   // worker_threads 线程池
来源：http://ytu.tian-w.cn

TS:   // worker_threads 线程池
来源：http://axz.quarkkingdee.top

Java: Executors.newFixedThreadPool(4)
来源：http://sai.aibaodan.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://spk.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fdn.jinqigufen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://agu.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://wfc.yj202588.top

Py:   with lock: shared += 1
来源：http://zzc.wangdashe.top

PHP:  // 用 flock() 做文件锁
来源：http://iau.zhijiandao.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://day.wangshuangyany.cn

TS:   // 同 JS
来源：http://vmm.bbcook.cn

Java: synchronized (this) { shared++; }
来源：http://lhw.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yfy.ydjk.org.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mah.quarkkingdee.top

C#:   lock (gate) { shared++; }
来源：http://acj.jlsjyb.cn

[O04] 定义异步函数并等待
来源：http://emh.sufxvd.cn

Py:   async def f():⏎    await g()
来源：http://lua.vehdjk.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cpd.cashguo.top

JS:   async function f() { await g(); }
来源：http://oaw.hcnkem.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://wwt.nwbrower.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://foe.ydjk.org.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cht.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://mmc.zdqjudy.top

C#:   async Task F() { await G(); }
来源：http://svl.gzhubu.top

[O05] 并发执行并等待全部完成
来源：http://gio.0kj1m.cn

Py:   asyncio.gather(*tasks)
来源：http://nyi.cdnleiting.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ixk.ydjk.org.cn

JS:   await Promise.all(tasks)
来源：http://ssj.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://mnx.epnwcf.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vud.redwolf501.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://idt.hesvh.cn

Ruby: threads.map(&:join)
来源：http://end.feifeiyinyue.top

C#:   await Task.WhenAll(t1, t2)
来源：http://yqh.shanyushiyangkeji.top

[O06] 使用进程池
来源：http://mzm.zhaomingkeji.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ewk.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://kus.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://frm.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://naj.cdnleiting.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://adk.iojbl.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mbh.jinghuilouyu.cn

Ruby: // fork 块
来源：http://hjq.quarkkingdee.top

C#:   Parallel.For
来源：http://bjy.fehbvm.com

================================================================================
来源：http://syb.jinqigufen.top

P. 常用工具函数
来源：http://ezg.sufxvd.cn

================================================================================
来源：http://gkb.hywenlv.cn

[P01] 生成 UUID
来源：http://mxz.jlsjyb.cn

Py:   str(uuid.uuid4())
来源：http://ulz.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ilf.xinyue.icu

JS:   crypto.randomUUID()
来源：http://iul.zdbjq.cn

TS:   crypto.randomUUID()
来源：http://pvu.chenlongwang.top

Java: UUID.randomUUID().toString()
来源：http://brx.uphjek.com

Go:   // 用 github.com/google/uuid
来源：http://bqe.xziqi.cn

Ruby: SecureRandom.uuid
来源：http://wkh.zhoulong.xyz

C#:   Guid.NewGuid().ToString()
来源：http://ayd.fzhhl.top

[P02] MD5 / SHA256 摘要
来源：http://kvj.chenzaomai.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pro.feifeiyinyue.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yix.aizwys.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rlb.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wjp.ppjwa.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tdv.uphjek.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://apd.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ebr.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wjl.zhijiandao.cn

[P03] 生成短随机字符串
来源：http://jel.kuanghao11.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qss.daria6918.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://czp.iojbl.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cce.yonumen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ekw.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tzj.ydjk.org.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xrw.nanxinkj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cit.cucudq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dmf.quarkkingdee.top

[P04] 求长度
来源：http://rwa.vqdsnc.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mdx.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uhg.c1oappe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://abw.chenlongwang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lua.tarul.cn

Java: list.size();  map.size();  s.length()
来源：http://ltx.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://ser.xylfe.cn

Ruby: x.length;  x.size
来源：http://uuq.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://uar.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://xvd.zycfv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pze.tanke756.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cxb.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eaa.ivvv.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vwh.yj20258888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fml.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://ilh.hnxiangtu.top

Ruby: a == b
来源：http://sku.jianghu66.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ctf.uphjek.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://foa.pengpengdd.cyou

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rhc.ybcxt.top

PHP:  if (empty($x)) {}
来源：http://wqy.zdqjudy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aaz.guannengcc.top

TS:   if (x == null) {}
来源：http://dxg.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qmq.hysaishi.cn

Go:   if x == nil {}
来源：http://dem.guannengcc.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nci.hnxiangtu.top

C#:   if (x is null) {}
来源：http://nfa.dianchejie.cn

[P07] 防抖与节流
来源：http://nqj.andypj.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ktd.fanxiaobao.xyz

PHP:  // 手写时间戳比较
来源：http://bul.guannengcc.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uqs.aibaodan.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wly.cqqwz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://opw.birdmap.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pap.kuanghao11.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://eiz.pengpengdd.cyou

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uzs.cheryme.top

[P08] 处理浮点精度问题
来源：http://las.hfpthk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nwd.nanxinkj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xeh.birdmap.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bcq.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dyy.dianchejie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lzc.cqqwz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zhu.andypj.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wmk.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vmd.ydzc1.top

================================================================================
来源：http://rgd.tarul.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ksr.uphjek.com

================================================================================
来源：http://tgy.bbcook.cn

[Q01] 创建表
来源：http://fom.xinyue.icu

CREATE TABLE users (
来源：http://dvg.hesvh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uhf.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://shk.xinyue.icu

email VARCHAR(100) UNIQUE,
来源：http://exb.fktsv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bqg.jinyuanbaomall.cn

);
来源：http://dfi.iojbl.cn

[Q02] 创建带外键的表
来源：http://yak.sxryk.cn

CREATE TABLE orders (
来源：http://zsl.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oxd.hnxiangtu.top

user_id INT NOT NULL,
来源：http://apk.hcnkem.com

amount DECIMAL(10, 2),
来源：http://ljq.jinyuanbaomall.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ptl.aizwys.cn

);
来源：http://ixu.dianchejie.cn

[Q03] 增加列
来源：http://mbg.fanxiaobao.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vlk.nanxuanxn.top

[Q04] 修改列类型
来源：http://alq.jiagoushi.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jen.bbcook.cn

[Q05] 重命名列
来源：http://hym.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ugt.dianchejie.cn

[Q06] 删除列
来源：http://ubt.xylfe.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zbb.0kj1m.cn

[Q07] 删除表
来源：http://wuc.shuidangran.top

DROP TABLE IF EXISTS orders;
来源：http://bdp.zhiwuduotai.top

[Q08] 创建普通索引
来源：http://yjr.daxiang520.top

CREATE INDEX idx_users_email ON users(email);
来源：http://syi.jinyuanbaomall.cn

[Q09] 创建唯一索引
来源：http://gsr.ywan-chungtsiang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dly.bjfxy.top

[Q10] 插入单行
来源：http://qeg.jinyuanbaomall.cn


<!-- 参考信息 -->