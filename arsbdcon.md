代发 wailian999

JS:   process.exit(1)
来源：http://hwp.snrcjt.cn

TS:   process.exit(1)
来源：http://slk.yj20258.top

Java: System.exit(1)
来源：http://jcv.daria6918.cn

Go:   os.Exit(1)
来源：http://vhh.hysaishi.cn

Ruby: exit 1
来源：http://ldn.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://web.jyoumei.cn

[M06] 向标准错误输出
来源：http://coy.yuanzhike.top

Py:   print("err", file=sys.stderr)
来源：http://wtg.c1oappe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vmz.feifeiyinyue.top

JS:   console.error("err")
来源：http://djt.svipenyu.cn

TS:   console.error("err")
来源：http://xxs.snrcjt.cn

Java: System.err.println("err")
来源：http://skf.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ird.chenlongwang.top

Ruby: warn "err"
来源：http://nzt.ydjk.org.cn

C#:   Console.Error.WriteLine("err")
来源：http://dgd.yuanzhike.top

[M07] 判断是否为主入口
来源：http://pyd.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://jau.cqqwz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ivp.hnqzz.top

JS:   require.main === module
来源：http://edd.tarul.cn

TS:   require.main === module
来源：http://hkb.zhiwuduotai.top

Java: public static void main(String[] args)
来源：http://tgf.0kj1m.cn

Go:   func main()
来源：http://nmj.jinyuanbaomall.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xde.yj202588.top

C#:   static void Main(string[] args)
来源：http://slg.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://qev.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://pad.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://xpe.daxiang520.top

JS:   process.platform;  process.version
来源：http://btg.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://ddq.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tgq.chenzaomai.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://rft.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qra.xuanzx.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://xbb.smart0.xyz

================================================================================
来源：http://ycx.fktsv.cn

N. 数据结构与算法
来源：http://dqg.yongpay.top

================================================================================
来源：http://dtx.quarkkingdee.top

[N01] 二分查找（有序数组）
来源：http://ytu.redwolf501.top

Py:   bisect.bisect_left(arr, x)
来源：http://qci.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qok.ehwqpu.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://afd.ydzc1.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ola.jianghu66.top

Java: Arrays.binarySearch(arr, x)
来源：http://vib.sysykeji.top

Go:   sort.SearchInts(arr, x)
来源：http://jqr.cdnleiting.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://for.shuidangran.top

C#:   Array.BinarySearch(arr, x)
来源：http://vdu.yfazqb.com

[N02] 排序（工程实践用内置实现）
来源：http://qnp.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://pot.sjlbkw.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://szm.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xwi.tarul.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://iow.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ryg.guowangkeji.top

Go:   slices.Sort(arr)
来源：http://opp.0kj1m.cn

Ruby: arr.sort
来源：http://rkq.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zfa.yj202588.top

[N03] 快速排序（分治示例）
来源：http://jpq.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yzd.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://ent.tianlin.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rfa.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gqn.xingfuxueyuan.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vpq.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aur.sysykeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rbt.fengsongda.top

C#:   // 手写递归，或 Array.Sort
来源：http://jei.zdbjq.cn

[N04] 斐波那契数列
来源：http://otr.quarkkingdee.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ezk.cheryme.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mdw.aibaodan.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rmy.zhengqikj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ouh.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wdb.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xdw.cdnleiting.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ovw.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jjw.hcnkem.com

[N05] 最大公约数
来源：http://ait.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://vat.pycfn.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iud.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ama.vehdjk.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cae.hammf.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xih.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sdu.sweek.top

Ruby: a.gcd(b)
来源：http://ybm.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fse.ppjwa.cn

[N06] 判断回文字符串
来源：http://uvk.quarkkingdee.top

Py:   s == s[::-1]
来源：http://upk.cqqwz.cn

PHP:  $s === strrev($s);
来源：http://axo.zhaomingkeji.xyz

JS:   s === [...s].reverse().join("")
来源：http://nlk.9152youxi.cn

TS:   s === [...s].reverse().join("")
来源：http://uyt.snrcjt.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tca.aizwys.cn

Go:   // 双指针从两端比较
来源：http://vqj.zdbjq.cn

Ruby: s == s.reverse
来源：http://phm.bjfxy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://frd.zhijiandao.cn

[N07] 两数之和（返回下标）
来源：http://qrm.wangshuangyany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sew.yuxming.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://upx.quarkkingdee.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pgg.dianchejie.cn

TS:   // 手写 Map<string, number>
来源：http://qsd.xuetiantiany.cn

Java: // 手写 HashMap
来源：http://jvv.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://aig.sweek.top

Ruby: // 手写 Hash
来源：http://xmn.svipenyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rhr.9152youxi.cn

[N08] 生成全排列
来源：http://rkh.hywenlv.cn

Py:   itertools.permutations(arr)
来源：http://smp.tanke756.top

PHP:  // 手写递归交换
来源：http://krs.chenlongwang.top

JS:   // 手写回溯递归
来源：http://ifl.kuanghao11.cn

TS:   // 手写回溯递归
来源：http://lbv.yfazqb.com

Java: // 手写回溯递归
来源：http://pbq.vqdsnc.cn

Go:   // 手写回溯递归
来源：http://xlu.zhijiandao.cn

Ruby: arr.permutation.to_a
来源：http://zfy.jinghuilouyu.cn

C#:   // 手写回溯递归
来源：http://vmm.nanxinkj.top

[N09] 栈与队列
来源：http://tfq.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ooe.shanyushiyangtech.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vru.sysykeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eal.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fna.zycfv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dlm.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zcq.iojbl.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mdn.fengsongda.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zdc.fktsv.cn

[N10] 链表节点定义
来源：http://nqo.tarul.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hcr.316326.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://bpf.gaohongyu789.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dfe.yonumen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mgh.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://nif.tian-w.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fnm.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://oqy.ivvv.top

C#:   class Node { public int V; public Node? Next; }
来源：http://olg.hysaishi.cn

[N11] 二叉树中序遍历
来源：http://kcc.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qdq.ydzc1.top

PHP:  // 手写递归函数
来源：http://ggb.quarkkingdee.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eyj.epnwcf.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oyw.tianlin.xyz

Java: // 手写递归
来源：http://mqd.vehdjk.com

Go:   // 手写递归
来源：http://oqb.guowangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nyv.aizwys.cn

C#:   // 手写递归
来源：http://gyj.sjlbkw.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zay.sxryk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ykb.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mge.yj20258888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jhg.cqqwz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://euc.zdqjudy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://goe.jqgufenzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ovh.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hqo.ppjwa.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yfj.zdqjudy.top

================================================================================
来源：http://aog.gogol.net.cn

O. 并发与异步
来源：http://wsl.cdnleiting.top

================================================================================
来源：http://cdn.aizwys.cn

[O01] 启动一个线程
来源：http://ddw.gotoacloud.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ucr.iojbl.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kaj.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pqw.52xcode.cn

TS:   // 同 JS
来源：http://qix.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://ovj.ydzc1.top

Go:   go f()
来源：http://zmd.pycfn.com

Ruby: Thread.new { f }
来源：http://xmu.daria6918.cn

C#:   Task.Run(() => F());
来源：http://rbk.fanxiaobao.xyz

[O02] 使用线程池
来源：http://nds.yvedp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://msl.quarkkingdee.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kto.ybcxt.top

JS:   // worker_threads 线程池
来源：http://pqu.andypj.xyz

TS:   // worker_threads 线程池
来源：http://bch.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://kgu.redwolf501.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ies.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wnl.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://irr.ywan-chungtsiang.top

[O03] 加锁保护共享数据
来源：http://ncp.cucudq.cn

Py:   with lock: shared += 1
来源：http://rea.xuetiantiany.cn

PHP:  // 用 flock() 做文件锁
来源：http://daw.sjlbkw.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tid.ivvv.top

TS:   // 同 JS
来源：http://nbe.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://vro.vehdjk.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://meu.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bcz.zhengqikj.top

C#:   lock (gate) { shared++; }
来源：http://prm.ydzc1.top

[O04] 定义异步函数并等待
来源：http://oii.cdnleiting.top

Py:   async def f():⏎    await g()
来源：http://wuu.xingfuxueyuan.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sty.fanxiaobao.xyz

JS:   async function f() { await g(); }
来源：http://ftc.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://lwg.zycfv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://omc.fktsv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jld.cqqwz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://prq.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://wbr.gzhubu.top

[O05] 并发执行并等待全部完成
来源：http://ezv.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://fhl.bbcook.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hsv.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://tdl.snrcjt.cn

TS:   await Promise.all(tasks)
来源：http://noe.yuanzhike.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qpy.yfazqb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wig.cdnleiting.top

Ruby: threads.map(&:join)
来源：http://uts.shuidangran.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nxv.chenjidiqi.icu

[O06] 使用进程池
来源：http://bsv.sweek.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vgv.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://fzp.yuxming.cn

JS:   // child_process / cluster 模块
来源：http://cfg.aibaodan.cn

TS:   // child_process / cluster 模块
来源：http://zke.gotoacloud.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pfg.yj20258888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://det.havefunace.top

Ruby: // fork 块
来源：http://nyw.yuxming.cn

C#:   Parallel.For
来源：http://ucz.fengsongda.top

================================================================================
来源：http://xyp.hongshengwenyu.top

P. 常用工具函数
来源：http://wko.yj20258888.top

================================================================================
来源：http://cft.hnxiangtu.top

[P01] 生成 UUID
来源：http://doa.cdnleiting.top

Py:   str(uuid.uuid4())
来源：http://mml.hywenlv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rkm.chenlongwang.top

JS:   crypto.randomUUID()
来源：http://zxv.andypj.xyz

TS:   crypto.randomUUID()
来源：http://afs.yj20258.top

Java: UUID.randomUUID().toString()
来源：http://ezj.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://yxd.dashuyun.cn

Ruby: SecureRandom.uuid
来源：http://xyo.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://mfw.aizwys.cn

[P02] MD5 / SHA256 摘要
来源：http://xwz.sxryk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bax.jlsjyb.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yfh.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ugm.kuanghao11.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://edx.shangyingyoupin.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nkl.gzhubu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mtt.yanxiufei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kka.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sla.ybcxt.top

[P03] 生成短随机字符串
来源：http://jnf.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mpm.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lfm.hongshengwenyu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fdy.xylfe.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lwe.tanke756.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cnj.fengsongda.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nso.shangyingyoupin.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dcj.quarkkingdee.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cso.chenlongwang.top

[P04] 求长度
来源：http://zck.52xcode.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dni.yuanzhike.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://foj.fehbvm.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vet.epnwcf.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wwe.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://jex.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://jwv.sweek.top

Ruby: x.length;  x.size
来源：http://kxr.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://tmz.meibo888.top

[P05] 判断两个对象内容是否相等
来源：http://nyk.nwbrower.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hqf.zhaomingkeji.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://htv.fengsongda.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hsk.xuanzx.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hme.smart0.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ahk.c1oappe.top

Go:   reflect.DeepEqual(a, b)
来源：http://ckd.havefunace.top

Ruby: a == b
来源：http://uoq.havefunace.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jdk.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xui.jianghu66.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bvw.jlsjyb.cn

PHP:  if (empty($x)) {}
来源：http://sak.gzhubu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rhq.xylfe.cn

TS:   if (x == null) {}
来源：http://yev.0kj1m.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uwu.sysykeji.top

Go:   if x == nil {}
来源：http://zhc.smart0.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dzo.xuanzx.com

C#:   if (x is null) {}
来源：http://jyd.hysaishi.cn

[P07] 防抖与节流
来源：http://fry.aibaodan.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zvx.yuxming.cn

PHP:  // 手写时间戳比较
来源：http://cbn.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cln.wangdashe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rej.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://prl.wangshuangyany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://evt.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://fpz.pycfn.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://klg.yanxiufei.cn

[P08] 处理浮点精度问题
来源：http://ind.gogol.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jlb.yongpay.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xgc.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://byu.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zjb.tianlin.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bvi.svipenyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rql.jinqigfzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zmw.daxiang520.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zsh.pengpengdd.cyou

================================================================================
来源：http://sfe.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ome.wangdashe.top

================================================================================
来源：http://fbo.zdbjq.cn

[Q01] 创建表
来源：http://kew.tanke756.top

CREATE TABLE users (
来源：http://knk.havefunace.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qeg.jqgufenzy.top

name VARCHAR(50) NOT NULL,
来源：http://frm.hcnkem.com

email VARCHAR(100) UNIQUE,
来源：http://mch.aibaodan.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zjc.zdbjq.cn

);
来源：http://evo.yangfankeji.com

[Q02] 创建带外键的表
来源：http://aie.sxryk.cn

CREATE TABLE orders (
来源：http://eku.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ehl.bbcook.cn

user_id INT NOT NULL,
来源：http://jwk.nanxinkj.top

amount DECIMAL(10, 2),
来源：http://usq.hfpthk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dcu.jiagoushi.top

);
来源：http://mzl.sxryk.cn

[Q03] 增加列
来源：http://esx.0kj1m.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cjs.sweek.top

[Q04] 修改列类型
来源：http://wdq.daxiang520.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cwx.jyoumei.cn

[Q05] 重命名列
来源：http://btm.jinyuanbaomall.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vvv.yuxming.cn

[Q06] 删除列
来源：http://chf.daxiang520.top


<!-- 参考信息 -->