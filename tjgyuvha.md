代发 wailian999

Py:   if __name__ == "__main__":
来源：http://fbd.yonumen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jti.daria6918.cn

JS:   require.main === module
来源：http://lld.ydjk.org.cn

TS:   require.main === module
来源：http://ybt.jiagoushi.top

Java: public static void main(String[] args)
来源：http://zrb.nanxinkj.top

Go:   func main()
来源：http://mim.yueranfly.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eot.xylfe.cn

C#:   static void Main(string[] args)
来源：http://hcl.jinqigufen.top

[M08] 获取系统与运行时信息
来源：http://nrb.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://tze.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://trc.yvedp.cn

JS:   process.platform;  process.version
来源：http://vwk.ppjwa.cn

TS:   process.platform;  process.version
来源：http://bxv.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nwn.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lbz.meibo888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fgt.yonumen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bjl.shanyushiyangtech.top

================================================================================
来源：http://uiu.hongshengwenyu.top

N. 数据结构与算法
来源：http://obc.tianlin.xyz

================================================================================
来源：http://nat.hesvh.cn

[N01] 二分查找（有序数组）
来源：http://kld.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dtk.xuanzx.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://djr.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fel.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yff.xingfuxueyuan.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://spq.hammf.cn

Go:   sort.SearchInts(arr, x)
来源：http://siq.fanxiaobao.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://wcg.uphjek.com

C#:   Array.BinarySearch(arr, x)
来源：http://pzl.fktsv.cn

[N02] 排序（工程实践用内置实现）
来源：http://nve.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://hiw.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hzc.jinqigufen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nia.cqqwz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ajn.fanxiaobao.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ctj.jqgfzy.top

Go:   slices.Sort(arr)
来源：http://fdb.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://cpv.ywan-chungtsiang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dub.nanxinkj.top

[N03] 快速排序（分治示例）
来源：http://ang.zhiwuduotai.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kku.gotoacloud.top

PHP:  // 递归实现，或用 usort
来源：http://fzq.zhixingplan.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bqu.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kxz.nanxinkj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aeg.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uhu.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qjd.cdnleiting.top

C#:   // 手写递归，或 Array.Sort
来源：http://hkg.tianlin.xyz

[N04] 斐波那契数列
来源：http://icd.haohaochexian.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hge.jqgufenzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tpj.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oay.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oiy.chenjidiqi.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rqn.redwolf501.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://juw.gogol.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wyu.tarul.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dox.zhengqikj.top

[N05] 最大公约数
来源：http://lqw.jiagoushi.top

Py:   math.gcd(a, b)
来源：http://ist.hesvh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gim.ydzc1.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fst.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kih.yj20258888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://khi.zhongyouzk.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iwm.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://hib.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vtd.bjfxy.top

[N06] 判断回文字符串
来源：http://his.quarkkingdee.top

Py:   s == s[::-1]
来源：http://aqw.shanyushiyangtech.top

PHP:  $s === strrev($s);
来源：http://bpf.9152youxi.cn

JS:   s === [...s].reverse().join("")
来源：http://dic.epnwcf.com

TS:   s === [...s].reverse().join("")
来源：http://buv.yj202588.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gni.jianghu66.top

Go:   // 双指针从两端比较
来源：http://jap.shanyushiyangtech.top

Ruby: s == s.reverse
来源：http://peo.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lhg.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://cfg.guowangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://els.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bwu.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zjh.zhongyouzk.top

TS:   // 手写 Map<string, number>
来源：http://yrz.redwolf501.top

Java: // 手写 HashMap
来源：http://enr.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://ebi.guannengcc.top

Ruby: // 手写 Hash
来源：http://lob.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://tbc.havefunace.top

[N08] 生成全排列
来源：http://jvh.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://ouh.cdnleiting.top

PHP:  // 手写递归交换
来源：http://gfg.xziqi.cn

JS:   // 手写回溯递归
来源：http://ojm.xuanzx.com

TS:   // 手写回溯递归
来源：http://rgm.yfazqb.com

Java: // 手写回溯递归
来源：http://vso.zdqjudy.top

Go:   // 手写回溯递归
来源：http://ddy.yuanzhike.top

Ruby: arr.permutation.to_a
来源：http://uwj.jianghu66.top

C#:   // 手写回溯递归
来源：http://xrh.fengsongda.top

[N09] 栈与队列
来源：http://dsj.cucudq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hqh.haohaochexian.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hak.gzhubu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eee.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mes.zhengqikj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oxf.dashuyun.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cru.chenjidiqi.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oea.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://klm.jiagoushi.top

[N10] 链表节点定义
来源：http://lrj.fktsv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nra.sysykeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hdb.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nwl.shanyushiyangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ynq.chenlongwang.top

Java: class Node { int v; Node next; }
来源：http://ehe.haohaochexian.top

Go:   type Node struct { V int; Next *Node }
来源：http://slx.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://xcn.yangfankeji.com

C#:   class Node { public int V; public Node? Next; }
来源：http://jat.gzhubu.top

[N11] 二叉树中序遍历
来源：http://rqf.fehbvm.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wqh.smart0.xyz

PHP:  // 手写递归函数
来源：http://vah.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://txi.52xcode.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pfv.shanyushiyangtech.top

Java: // 手写递归
来源：http://iav.yuxming.cn

Go:   // 手写递归
来源：http://vgg.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gfy.nwbrower.top

C#:   // 手写递归
来源：http://sxe.zdqjudy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bjk.redwolf501.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ptt.hongshengwenyu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qeg.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tth.hnxiangtu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jyv.zycfv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bcy.tianlin.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://weh.fehbvm.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fcg.wangshuangyany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://krp.zhengqikj.top

================================================================================
来源：http://qck.jlsjyb.cn

O. 并发与异步
来源：http://bdw.chenzaomai.com

================================================================================
来源：http://upx.ppjwa.cn

[O01] 启动一个线程
来源：http://uwv.jinyuanbaomall.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dmr.meibo888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xuc.ppjwa.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xsv.gzhubu.top

TS:   // 同 JS
来源：http://rwv.uphjek.com

Java: new Thread(() -> f()).start()
来源：http://bsj.dashuyun.cn

Go:   go f()
来源：http://wcl.wangdashe.top

Ruby: Thread.new { f }
来源：http://mlb.bjfxy.top

C#:   Task.Run(() => F());
来源：http://nvx.uphjek.com

[O02] 使用线程池
来源：http://gol.yj202588.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ogq.zhoulong.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vtc.redwolf501.top

JS:   // worker_threads 线程池
来源：http://lfa.cheryme.top

TS:   // worker_threads 线程池
来源：http://rij.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dsl.yj20258888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xfh.hnqzz.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zhb.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zhf.zdqjudy.top

[O03] 加锁保护共享数据
来源：http://ydo.guannengcc.top

Py:   with lock: shared += 1
来源：http://zhe.9152youxi.cn

PHP:  // 用 flock() 做文件锁
来源：http://eyh.ivvv.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tbk.birdmap.top

TS:   // 同 JS
来源：http://aum.andypj.xyz

Java: synchronized (this) { shared++; }
来源：http://vvv.hnxiangtu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wtn.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rbe.zycfv.cn

C#:   lock (gate) { shared++; }
来源：http://ssf.birdmap.top

[O04] 定义异步函数并等待
来源：http://nnq.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://xfc.hcnkem.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pps.uphjek.com

JS:   async function f() { await g(); }
来源：http://gpq.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bgb.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gpq.meibo888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rnv.ctjpmb.com

Ruby: # 用 Fiber 或 async gem
来源：http://fci.chenzaomai.com

C#:   async Task F() { await G(); }
来源：http://rum.ywan-chungtsiang.top

[O05] 并发执行并等待全部完成
来源：http://jwo.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://aze.mhx1999.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fpe.meibo888.top

JS:   await Promise.all(tasks)
来源：http://vyk.hysaishi.cn

TS:   await Promise.all(tasks)
来源：http://vnx.vqdsnc.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://foy.sjlbkw.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mdp.vehdjk.com

Ruby: threads.map(&:join)
来源：http://krx.sweek.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cjr.epnwcf.com

[O06] 使用进程池
来源：http://wln.ybcxt.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wod.pycfn.com

PHP:  // pcntl_fork 或多进程队列
来源：http://keu.ctjpmb.com

JS:   // child_process / cluster 模块
来源：http://tzg.ybcxt.top

TS:   // child_process / cluster 模块
来源：http://nvk.wangdashe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tba.guannengcc.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gtf.cheryme.top

Ruby: // fork 块
来源：http://vgd.sysykeji.top

C#:   Parallel.For
来源：http://agn.hfpthk.cn

================================================================================
来源：http://jnq.mhx1999.top

P. 常用工具函数
来源：http://loi.feifeiyinyue.top

================================================================================
来源：http://uan.gotoacloud.top

[P01] 生成 UUID
来源：http://jpg.zhixingplan.top

Py:   str(uuid.uuid4())
来源：http://wxn.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rdk.zhixingplan.top

JS:   crypto.randomUUID()
来源：http://mop.nanxinkj.top

TS:   crypto.randomUUID()
来源：http://xei.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://bdn.zycfv.cn

Go:   // 用 github.com/google/uuid
来源：http://tbo.yongpay.top

Ruby: SecureRandom.uuid
来源：http://tas.cashguo.top

C#:   Guid.NewGuid().ToString()
来源：http://gmw.hammf.cn

[P02] MD5 / SHA256 摘要
来源：http://vpb.hnxiangtu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ctr.cashguo.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://umj.cheryme.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gda.meibo888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://szd.bjfxy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qef.jinqigufen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vcw.shanyushiyangtech.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bjw.xinyue.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nhf.mhx1999.top

[P03] 生成短随机字符串
来源：http://hwg.havefunace.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uur.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wom.ydzc1.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mrm.fanxiaobao.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://laj.yj202588.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://djm.gogol.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iys.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://plu.jinyuanbaomall.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://suf.zdbjq.cn

[P04] 求长度
来源：http://qls.wangshuangyany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ljc.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qsp.cheryme.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://udv.yanxiufei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xzd.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://jfq.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://qso.52xcode.cn

Ruby: x.length;  x.size
来源：http://tkz.xylfe.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rje.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://alc.pengpengdd.cyou

Py:   a == b              # 列表与字典递归比较内容
来源：http://kfb.cheryme.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mmc.jqgfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jnp.tian-w.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ulb.0kj1m.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vaw.jinqigufen.top

Go:   reflect.DeepEqual(a, b)
来源：http://mji.9152youxi.cn

Ruby: a == b
来源：http://pee.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hhr.sufxvd.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cgo.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zlj.meibo888.top

PHP:  if (empty($x)) {}
来源：http://jpj.yj20258.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://weo.tian-w.cn

TS:   if (x == null) {}
来源：http://tov.shuidangran.top

Java: if (x == null || x.isEmpty()) {}
来源：http://svj.kuanghao11.cn

Go:   if x == nil {}
来源：http://nny.ppjwa.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gsx.ivvv.top

C#:   if (x is null) {}
来源：http://xtl.epnwcf.com

[P07] 防抖与节流
来源：http://wev.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://abz.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://ieq.birdmap.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zfn.hammf.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rjn.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uny.316326.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dxh.yj20258888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://tnd.shanyushiyangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://btr.zhengqikj.top

[P08] 处理浮点精度问题
来源：http://wiv.jinqigfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vog.haohaochexian.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lng.sufxvd.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mys.yangfankeji.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ycq.kuanghao11.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ynh.hnxiangtu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://auw.xingfuxueyuan.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wny.smart0.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hbk.daxiang520.top

================================================================================
来源：http://klz.jinyuanbaomall.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wrc.fzhhl.top

================================================================================
来源：http://cmb.yj202588.top

[Q01] 创建表
来源：http://yst.sjlbkw.cn

CREATE TABLE users (
来源：http://tqi.ivvv.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zby.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://tvs.yj20258888.top

email VARCHAR(100) UNIQUE,
来源：http://ena.andypj.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://crp.meibo888.top

);
来源：http://rzr.cashguo.top

[Q02] 创建带外键的表
来源：http://axl.aizwys.cn

CREATE TABLE orders (
来源：http://rup.kuanghao11.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ima.jinghuilouyu.cn

user_id INT NOT NULL,
来源：http://dyy.nanxinkj.top

amount DECIMAL(10, 2),
来源：http://jvf.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mbw.uphjek.com

);
来源：http://pwu.nanxuanxn.top

[Q03] 增加列
来源：http://yvx.zhiwuduotai.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lat.tarul.cn

[Q04] 修改列类型
来源：http://jgm.zhixingplan.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iub.tarul.cn

[Q05] 重命名列
来源：http://adf.chenlongwang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mko.xuanzx.com

[Q06] 删除列
来源：http://snb.daria6918.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cqw.redwolf501.top

[Q07] 删除表
来源：http://xtp.zhixingplan.top

DROP TABLE IF EXISTS orders;
来源：http://std.smart0.xyz

[Q08] 创建普通索引
来源：http://dam.gogol.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pcv.xylfe.cn

[Q09] 创建唯一索引
来源：http://ptx.aizwys.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://slu.uphjek.com

[Q10] 插入单行
来源：http://nqm.sxryk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hjy.guowangkeji.top

[Q11] 一次插入多行
来源：http://nic.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rbn.guannengcc.top

[Q12] 插入后取自增 ID
来源：http://xxr.guannengcc.top

INSERT INTO users (name) VALUES ('C');
来源：http://ghe.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mxx.c1oappe.top

[Q13] 忽略重复插入
来源：http://rww.cheryme.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kwc.jianghu66.top


<!-- 参考信息 -->