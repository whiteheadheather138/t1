代发 wailian999

Ruby: exit 1
来源：http://mjr.316326.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gvz.xuetiantiany.cn

[M06] 向标准错误输出
来源：http://ahw.cdnleiting.top

Py:   print("err", file=sys.stderr)
来源：http://anh.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://ima.iojbl.cn

JS:   console.error("err")
来源：http://doz.fzhhl.top

TS:   console.error("err")
来源：http://cfs.zhijiandao.cn

Java: System.err.println("err")
来源：http://rwg.hywenlv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fvh.cqqwz.cn

Ruby: warn "err"
来源：http://ueo.ehwqpu.com

C#:   Console.Error.WriteLine("err")
来源：http://ork.tarul.cn

[M07] 判断是否为主入口
来源：http://ihx.uphjek.com

Py:   if __name__ == "__main__":
来源：http://iso.zhengqikj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://idq.sweek.top

JS:   require.main === module
来源：http://lbu.svipenyu.cn

TS:   require.main === module
来源：http://ymp.hongshengwenyu.top

Java: public static void main(String[] args)
来源：http://xlj.nanxuanxn.top

Go:   func main()
来源：http://itm.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wmn.daria6918.cn

C#:   static void Main(string[] args)
来源：http://pzm.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://sbi.ehwqpu.com

Py:   platform.system();  platform.python_version()
来源：http://dyt.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://nkt.dianchejie.cn

JS:   process.platform;  process.version
来源：http://klj.zhaomingkeji.xyz

TS:   process.platform;  process.version
来源：http://bbh.svipenyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nwy.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rwu.svipenyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xkg.chenzaomai.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ztv.yongpay.top

================================================================================
来源：http://vur.fzhhl.top

N. 数据结构与算法
来源：http://nfv.jqgfzy.top

================================================================================
来源：http://pft.hcnkem.com

[N01] 二分查找（有序数组）
来源：http://jaq.chenlongwang.top

Py:   bisect.bisect_left(arr, x)
来源：http://ltj.fengsongda.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xdy.shzxlz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nsu.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mtl.ehwqpu.com

Java: Arrays.binarySearch(arr, x)
来源：http://lmz.zycfv.cn

Go:   sort.SearchInts(arr, x)
来源：http://kwo.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zqk.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://xvq.yfazqb.com

[N02] 排序（工程实践用内置实现）
来源：http://uvr.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://rsx.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fim.nanxinkj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://wif.jianghu66.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fme.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wox.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://sjz.hesvh.cn

Ruby: arr.sort
来源：http://xyg.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qpj.chenzaomai.com

[N03] 快速排序（分治示例）
来源：http://gmg.yfazqb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xxu.fanxiaobao.xyz

PHP:  // 递归实现，或用 usort
来源：http://eih.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fyi.mhx1999.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wdj.dashuyun.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fpw.yangfankeji.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xjr.pengpengdd.cyou

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vjf.bbcook.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gvh.yvedp.cn

[N04] 斐波那契数列
来源：http://vrv.jyoumei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ymj.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ckr.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zsr.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sts.feifeiyinyue.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xyx.jyoumei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xrt.daxiang520.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://beh.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lwf.yj20258888.top

[N05] 最大公约数
来源：http://krq.shangyingyoupin.top

Py:   math.gcd(a, b)
来源：http://fcu.ivvv.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eol.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://utt.0kj1m.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fve.yj20258.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pwo.gogol.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uym.daxiang520.top

Ruby: a.gcd(b)
来源：http://xpj.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dlx.vehdjk.com

[N06] 判断回文字符串
来源：http://qll.jinqigufen.top

Py:   s == s[::-1]
来源：http://uso.hnxiangtu.top

PHP:  $s === strrev($s);
来源：http://jmi.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://oxw.xingfuxueyuan.xyz

TS:   s === [...s].reverse().join("")
来源：http://wlr.ppjwa.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eir.c1oappe.top

Go:   // 双指针从两端比较
来源：http://cgq.haohaochexian.top

Ruby: s == s.reverse
来源：http://ffi.tanke756.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ake.ybcxt.top

[N07] 两数之和（返回下标）
来源：http://jyn.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ysp.fktsv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sar.xingfuxueyuan.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://kuc.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://ofp.gotoacloud.top

Java: // 手写 HashMap
来源：http://uph.tanke756.top

Go:   // 手写 map[int]int
来源：http://dxb.yuxming.cn

Ruby: // 手写 Hash
来源：http://leh.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iel.epnwcf.com

[N08] 生成全排列
来源：http://zhb.shanyushiyangtech.top

Py:   itertools.permutations(arr)
来源：http://ios.hammf.cn

PHP:  // 手写递归交换
来源：http://cgx.jiagoushi.top

JS:   // 手写回溯递归
来源：http://qab.0kj1m.cn

TS:   // 手写回溯递归
来源：http://mgn.zhijiandao.cn

Java: // 手写回溯递归
来源：http://zsk.epnwcf.com

Go:   // 手写回溯递归
来源：http://tsx.chenjidiqi.icu

Ruby: arr.permutation.to_a
来源：http://rsk.hywenlv.cn

C#:   // 手写回溯递归
来源：http://edr.sufxvd.cn

[N09] 栈与队列
来源：http://xqd.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://azk.yj20258.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://loj.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eqr.redwolf501.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gad.xinyue.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://act.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zsv.pengpengdd.cyou

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xll.uphjek.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lny.fehbvm.com

[N10] 链表节点定义
来源：http://bwu.fehbvm.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kky.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ntp.vehdjk.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://weq.tarul.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dmm.gotoacloud.top

Java: class Node { int v; Node next; }
来源：http://ouq.jiagoushi.top

Go:   type Node struct { V int; Next *Node }
来源：http://xex.hywenlv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wjl.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rzj.meibo888.top

[N11] 二叉树中序遍历
来源：http://lum.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ceg.zhijiandao.cn

PHP:  // 手写递归函数
来源：http://uma.zhaomingkeji.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ebe.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dor.0kj1m.cn

Java: // 手写递归
来源：http://dua.birdmap.top

Go:   // 手写递归
来源：http://vnx.daxiang520.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wmn.nanxinkj.top

C#:   // 手写递归
来源：http://sen.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://acj.shanyushiyangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://png.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aye.jianghu66.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://chc.ctjpmb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rhc.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xfd.zhixingplan.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://izt.pycfn.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sey.fzhhl.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wbb.jinyuanbaomall.cn

================================================================================
来源：http://hhe.uphjek.com

O. 并发与异步
来源：http://mqe.hammf.cn

================================================================================
来源：http://geh.gogol.net.cn

[O01] 启动一个线程
来源：http://vhf.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://abx.jinghuilouyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ulq.jinghuilouyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gqq.havefunace.top

TS:   // 同 JS
来源：http://vgl.fengsongda.top

Java: new Thread(() -> f()).start()
来源：http://yae.yuanzhike.top

Go:   go f()
来源：http://mle.sysykeji.top

Ruby: Thread.new { f }
来源：http://kof.cheryme.top

C#:   Task.Run(() => F());
来源：http://ffo.yanxiufei.cn

[O02] 使用线程池
来源：http://ggl.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pdm.feifeiyinyue.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wdm.fzhhl.top

JS:   // worker_threads 线程池
来源：http://bas.52xcode.cn

TS:   // worker_threads 线程池
来源：http://cff.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://mnv.yvedp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nwc.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vwq.ctjpmb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xwr.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://avk.snrcjt.cn

Py:   with lock: shared += 1
来源：http://sdg.xuetiantiany.cn

PHP:  // 用 flock() 做文件锁
来源：http://nuc.sysykeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bvo.sweek.top

TS:   // 同 JS
来源：http://lcq.bjfxy.top

Java: synchronized (this) { shared++; }
来源：http://upa.xylfe.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ysp.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://emu.hfpthk.cn

C#:   lock (gate) { shared++; }
来源：http://ymo.gzhubu.top

[O04] 定义异步函数并等待
来源：http://ros.jqgfzy.top

Py:   async def f():⏎    await g()
来源：http://exa.hcnkem.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ykc.yj202588.top

JS:   async function f() { await g(); }
来源：http://gzw.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://evs.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bdw.yuanzhike.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://drj.jlsjyb.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gao.uphjek.com

C#:   async Task F() { await G(); }
来源：http://fen.yj20258888.top

[O05] 并发执行并等待全部完成
来源：http://jvp.zhoulong.xyz

Py:   asyncio.gather(*tasks)
来源：http://uyj.hcnkem.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tod.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://rbr.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://exb.fanxiaobao.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://glf.dianchejie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ccx.iojbl.cn

Ruby: threads.map(&:join)
来源：http://pui.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gsb.cucudq.cn

[O06] 使用进程池
来源：http://rox.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hij.yanxiufei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cfd.9152youxi.cn

JS:   // child_process / cluster 模块
来源：http://ene.jinqigfzy.top

TS:   // child_process / cluster 模块
来源：http://fgl.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iiy.jyoumei.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pbn.fktsv.cn

Ruby: // fork 块
来源：http://gzo.jiagoushi.top

C#:   Parallel.For
来源：http://oxt.meibo888.top

================================================================================
来源：http://nmk.vehdjk.com

P. 常用工具函数
来源：http://tit.ehwqpu.com

================================================================================
来源：http://mze.cheryme.top

[P01] 生成 UUID
来源：http://ipy.hammf.cn

Py:   str(uuid.uuid4())
来源：http://qyg.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://poh.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://aig.fanxiaobao.xyz

TS:   crypto.randomUUID()
来源：http://drp.fktsv.cn

Java: UUID.randomUUID().toString()
来源：http://mai.zhoulong.xyz

Go:   // 用 github.com/google/uuid
来源：http://prf.redwolf501.top

Ruby: SecureRandom.uuid
来源：http://xon.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://fgh.zhoulong.xyz

[P02] MD5 / SHA256 摘要
来源：http://dmy.shanyushiyangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oft.xingfuxueyuan.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://rut.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://szx.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xms.fengsongda.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gft.hongshengwenyu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oqn.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://otk.zhoulong.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vrd.hongshengwenyu.top

[P03] 生成短随机字符串
来源：http://vja.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://foz.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dkz.gogol.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ezb.birdmap.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xmb.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cau.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fgz.hcnkem.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://uto.fanxiaobao.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://usq.jyoumei.cn

[P04] 求长度
来源：http://jyt.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://awx.yj20258888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vxo.epnwcf.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dlc.andypj.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yjz.sysykeji.top

Java: list.size();  map.size();  s.length()
来源：http://rda.tianlin.xyz

Go:   len(arr);  len(m)
来源：http://nrj.svipenyu.cn

Ruby: x.length;  x.size
来源：http://tnz.xuetiantiany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bfo.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://muq.mhx1999.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://uzn.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sok.jyoumei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nla.bbcook.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hbs.fengsongda.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rll.yuanzhike.top

Go:   reflect.DeepEqual(a, b)
来源：http://dgs.yfazqb.com

Ruby: a == b
来源：http://hbo.jqgfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ius.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qsz.sufxvd.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jkf.yongpay.top

PHP:  if (empty($x)) {}
来源：http://bhi.gzhubu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dpn.yangfankeji.com

TS:   if (x == null) {}
来源：http://zwo.cdnleiting.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vdu.xylfe.cn

Go:   if x == nil {}
来源：http://olu.havefunace.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://svf.316326.xyz

C#:   if (x is null) {}
来源：http://dhd.tian-w.cn

[P07] 防抖与节流
来源：http://bnt.ivvv.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fgz.tanke756.top

PHP:  // 手写时间戳比较
来源：http://wsg.hfpthk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fqm.fehbvm.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qnb.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yso.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xrv.jinqigfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://izw.ehwqpu.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tqd.xingfuxueyuan.xyz

[P08] 处理浮点精度问题
来源：http://zcz.sweek.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lgw.0kj1m.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ofl.fanxiaobao.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ajq.hnqzz.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kjp.uphjek.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wyt.hnqzz.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://thv.zhengqikj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://acb.shuidangran.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zub.xuanzx.com

================================================================================
来源：http://fay.hnxiangtu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hix.xylfe.cn

================================================================================
来源：http://zyj.9152youxi.cn

[Q01] 创建表
来源：http://myd.cashguo.top

CREATE TABLE users (
来源：http://pkj.sysykeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://apb.shangyingyoupin.top

name VARCHAR(50) NOT NULL,
来源：http://tll.tarul.cn

email VARCHAR(100) UNIQUE,
来源：http://hcn.xziqi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nrs.yuxming.cn

);
来源：http://jki.havefunace.top

[Q02] 创建带外键的表
来源：http://rfl.shangyingyoupin.top

CREATE TABLE orders (
来源：http://wmi.yj20258888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nvu.jinghuilouyu.cn

user_id INT NOT NULL,
来源：http://nay.zhoulong.xyz

amount DECIMAL(10, 2),
来源：http://jdl.ywan-chungtsiang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://avf.mhx1999.top

);
来源：http://xsx.wangshuangyany.cn

[Q03] 增加列
来源：http://tif.yonumen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ahe.gzhubu.top

[Q04] 修改列类型
来源：http://mhh.aibaodan.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zsw.birdmap.top

[Q05] 重命名列
来源：http://dgt.haohaochexian.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xhr.redwolf501.top

[Q06] 删除列
来源：http://faj.jinqigufen.top

ALTER TABLE users DROP COLUMN age;
来源：http://pnl.aizwys.cn

[Q07] 删除表
来源：http://cxy.c1oappe.top

DROP TABLE IF EXISTS orders;
来源：http://lyi.jlsjyb.cn

[Q08] 创建普通索引
来源：http://ujr.nwbrower.top


<!-- 参考信息 -->