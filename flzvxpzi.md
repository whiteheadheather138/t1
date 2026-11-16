代发 wailian999

Py:   resp.json()
来源：http://wux.yueranfly.top

PHP:  json_decode($body, true);
来源：http://pfl.yvedp.cn

JS:   await resp.json()
来源：http://vkp.sufxvd.cn

TS:   await resp.json()
来源：http://nwe.fanxiaobao.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tpn.yj202588.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://grp.uphjek.com

Ruby: JSON.parse(resp.body)
来源：http://kqo.nanxuanxn.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mps.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://bks.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lxi.sufxvd.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qbr.gotoacloud.top

JS:   resp.ok;  resp.status
来源：http://fqv.bbcook.cn

TS:   resp.ok;  resp.status
来源：http://pvh.hcnkem.com

Java: resp.statusCode()
来源：http://bar.yueranfly.top

Go:   resp.StatusCode
来源：http://qus.hongshengwenyu.top

Ruby: resp.code.to_i
来源：http://eih.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://mot.hfpthk.cn

[L08] 并发请求多个地址
来源：http://lor.xylfe.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://car.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://zyi.nwbrower.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lty.sysykeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ujf.jinqigufen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dxm.tian-w.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iax.chenlongwang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uzd.jlsjyb.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jhy.birdmap.top

================================================================================
来源：http://hnk.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://hbr.yongpay.top

================================================================================
来源：http://tbc.redwolf501.top

[M01] 读取命令行参数
来源：http://rfl.guannengcc.top

Py:   sys.argv[1:]
来源：http://gls.gogol.net.cn

PHP:  $argv;  $argc;
来源：http://jdi.yuxming.cn

JS:   process.argv.slice(2)
来源：http://fbp.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://ecx.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://gcr.quarkkingdee.top

Go:   os.Args[1:]
来源：http://oyk.0kj1m.cn

Ruby: ARGV
来源：http://xis.haohaochexian.top

C#:   args 数组（Main 方法参数）
来源：http://evq.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://erz.ybcxt.top

Py:   os.environ.get("HOME")
来源：http://kuz.wangshuangyany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kqg.jinqigfzy.top

JS:   process.env.HOME
来源：http://ezf.jiagoushi.top

TS:   process.env.HOME
来源：http://ncy.zhaomingkeji.xyz

Java: System.getenv("HOME")
来源：http://fgf.daria6918.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hvb.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://ysb.ydzc1.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dte.yuanzhike.top

[M03] 执行外部命令
来源：http://buv.ehwqpu.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rqx.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kcu.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://imb.andypj.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://zbn.dashuyun.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cbv.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ebp.svipenyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kwm.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://rwm.jiagoushi.top

[M04] 获取当前工作目录
来源：http://gzv.9152youxi.cn

Py:   os.getcwd()
来源：http://uya.shangyingyoupin.top

PHP:  getcwd();
来源：http://sus.aibaodan.cn

JS:   process.cwd()
来源：http://xik.shuidangran.top

TS:   process.cwd()
来源：http://ali.yanxiufei.cn

Java: Path.of("").toAbsolutePath()
来源：http://efr.ctjpmb.com

Go:   os.Getwd()
来源：http://aka.yfazqb.com

Ruby: Dir.pwd
来源：http://myd.0kj1m.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fry.yueranfly.top

[M05] 设置退出码
来源：http://dob.tanke756.top

Py:   sys.exit(1)
来源：http://onr.yangfankeji.com

PHP:  exit(1);
来源：http://huj.jianghu66.top

JS:   process.exit(1)
来源：http://het.zhongyouzk.top

TS:   process.exit(1)
来源：http://hdn.shangyingyoupin.top

Java: System.exit(1)
来源：http://wzd.cheryme.top

Go:   os.Exit(1)
来源：http://bai.svipenyu.cn

Ruby: exit 1
来源：http://zff.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rdf.sufxvd.cn

[M06] 向标准错误输出
来源：http://iah.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://xye.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ckl.yangfankeji.com

JS:   console.error("err")
来源：http://kxn.jqgfzy.top

TS:   console.error("err")
来源：http://xiw.epnwcf.com

Java: System.err.println("err")
来源：http://wuc.yuxming.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pwn.jianghu66.top

Ruby: warn "err"
来源：http://zsc.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://yjt.zdbjq.cn

[M07] 判断是否为主入口
来源：http://lfn.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://byk.bbcook.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oex.gotoacloud.top

JS:   require.main === module
来源：http://gdt.zycfv.cn

TS:   require.main === module
来源：http://bqz.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://zxn.zhoulong.xyz

Go:   func main()
来源：http://hjk.hywenlv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fba.yueranfly.top

C#:   static void Main(string[] args)
来源：http://xyq.wangdashe.top

[M08] 获取系统与运行时信息
来源：http://che.hongshengwenyu.top

Py:   platform.system();  platform.python_version()
来源：http://ghs.svipenyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://aar.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://lbw.guannengcc.top

TS:   process.platform;  process.version
来源：http://vzz.316326.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://inz.zhengqikj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kql.fanxiaobao.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ehs.shanyushiyangtech.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nhk.jyoumei.cn

================================================================================
来源：http://rks.zhixingplan.top

N. 数据结构与算法
来源：http://agz.hnxiangtu.top

================================================================================
来源：http://llp.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://rky.ybcxt.top

Py:   bisect.bisect_left(arr, x)
来源：http://gnj.zhixingplan.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uug.yj20258888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zjc.tianlin.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mxq.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ztj.ydzc1.top

Go:   sort.SearchInts(arr, x)
来源：http://hwe.bjfxy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://snh.mhx1999.top

C#:   Array.BinarySearch(arr, x)
来源：http://tnc.xylfe.cn

[N02] 排序（工程实践用内置实现）
来源：http://wrg.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://lhr.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fgz.hnqzz.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qrb.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://fnn.yangfankeji.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rzg.jiagoushi.top

Go:   slices.Sort(arr)
来源：http://qom.chenlongwang.top

Ruby: arr.sort
来源：http://ixp.zhiwuduotai.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fug.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://bnv.ehwqpu.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hlp.cqqwz.cn

PHP:  // 递归实现，或用 usort
来源：http://gad.cqqwz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tbs.bbcook.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pww.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://unq.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pqn.xingfuxueyuan.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zly.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://ajp.cheryme.top

[N04] 斐波那契数列
来源：http://utz.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dge.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jsw.sufxvd.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gil.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mcg.yfazqb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://put.hesvh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rub.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kqh.ydjk.org.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dja.dashuyun.cn

[N05] 最大公约数
来源：http://lak.zhijiandao.cn

Py:   math.gcd(a, b)
来源：http://bfg.fktsv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://szc.vqdsnc.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gsm.yongpay.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ood.zhiwuduotai.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vmm.snrcjt.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vgw.pycfn.com

Ruby: a.gcd(b)
来源：http://vld.meibo888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tgf.jiagoushi.top

[N06] 判断回文字符串
来源：http://yxv.nwbrower.top

Py:   s == s[::-1]
来源：http://nws.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://rzn.ydjk.org.cn

JS:   s === [...s].reverse().join("")
来源：http://rxj.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://nng.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://avt.andypj.xyz

Go:   // 双指针从两端比较
来源：http://ign.jinyuanbaomall.cn

Ruby: s == s.reverse
来源：http://uzj.fanxiaobao.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://tds.meibo888.top

[N07] 两数之和（返回下标）
来源：http://cpj.kuanghao11.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tap.9152youxi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bhn.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://yrp.52xcode.cn

TS:   // 手写 Map<string, number>
来源：http://zgf.xuanzx.com

Java: // 手写 HashMap
来源：http://igp.daria6918.cn

Go:   // 手写 map[int]int
来源：http://ckz.c1oappe.top

Ruby: // 手写 Hash
来源：http://udt.jyoumei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zyv.sweek.top

[N08] 生成全排列
来源：http://ova.guowangkeji.top

Py:   itertools.permutations(arr)
来源：http://kgh.xinyue.icu

PHP:  // 手写递归交换
来源：http://ibu.jinyuanbaomall.cn

JS:   // 手写回溯递归
来源：http://bjq.shzxlz.cn

TS:   // 手写回溯递归
来源：http://hmg.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://lng.c1oappe.top

Go:   // 手写回溯递归
来源：http://gex.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://loq.pycfn.com

C#:   // 手写回溯递归
来源：http://vpe.andypj.xyz

[N09] 栈与队列
来源：http://yxq.cqqwz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xih.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qdy.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://koi.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nqc.yuanzhike.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hjy.vqdsnc.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yft.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qix.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aeq.nanxinkj.top

[N10] 链表节点定义
来源：http://omj.chenlongwang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xdf.c1oappe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lne.fengsongda.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cok.shanyushiyangtech.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cji.dianchejie.cn

Java: class Node { int v; Node next; }
来源：http://jfv.316326.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://spv.yvedp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://arx.jinqigfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vey.chenjidiqi.icu

[N11] 二叉树中序遍历
来源：http://pxe.cucudq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rfc.xylfe.cn

PHP:  // 手写递归函数
来源：http://esc.tarul.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lro.bjfxy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nsx.c1oappe.top

Java: // 手写递归
来源：http://lcu.zdqjudy.top

Go:   // 手写递归
来源：http://xpz.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bpw.fktsv.cn

C#:   // 手写递归
来源：http://ltw.xziqi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zwl.shanyushiyangtech.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vxg.vqdsnc.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cfy.tanke756.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jmv.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://enn.zhoulong.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qzg.jinqigfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zkw.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sxs.ywan-chungtsiang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zwd.shanyushiyangtech.top

================================================================================
来源：http://ojk.gogol.net.cn

O. 并发与异步
来源：http://rke.svipenyu.cn

================================================================================
来源：http://wyp.jiagoushi.top

[O01] 启动一个线程
来源：http://uwr.guannengcc.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bcn.pycfn.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pju.zhengqikj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://njr.cucudq.cn

TS:   // 同 JS
来源：http://vjy.chenlongwang.top

Java: new Thread(() -> f()).start()
来源：http://qpz.ppjwa.cn

Go:   go f()
来源：http://jou.fehbvm.com

Ruby: Thread.new { f }
来源：http://vnr.bbcook.cn

C#:   Task.Run(() => F());
来源：http://jti.hnqzz.top

[O02] 使用线程池
来源：http://rwz.ctjpmb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://knj.shanyushiyangtech.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://onw.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://tla.ivvv.top

TS:   // worker_threads 线程池
来源：http://xso.yanxiufei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hzd.tanke756.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mrq.chenlongwang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cff.fzhhl.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xow.uphjek.com

[O03] 加锁保护共享数据
来源：http://fro.zhixingplan.top

Py:   with lock: shared += 1
来源：http://bln.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://kpt.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rre.gaohongyu789.top

TS:   // 同 JS
来源：http://ffw.yvedp.cn

Java: synchronized (this) { shared++; }
来源：http://npf.uphjek.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://shr.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cup.cdnleiting.top

C#:   lock (gate) { shared++; }
来源：http://cbf.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://lei.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://tcx.shzxlz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wwg.svipenyu.cn

JS:   async function f() { await g(); }
来源：http://iyq.xinyue.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://lby.fzhhl.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://csd.pengpengdd.cyou

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sff.vehdjk.com

Ruby: # 用 Fiber 或 async gem
来源：http://yye.smart0.xyz

C#:   async Task F() { await G(); }
来源：http://yrn.guowangkeji.top

[O05] 并发执行并等待全部完成
来源：http://acq.9152youxi.cn

Py:   asyncio.gather(*tasks)
来源：http://saq.yfazqb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lbp.sufxvd.cn

JS:   await Promise.all(tasks)
来源：http://ogf.fktsv.cn

TS:   await Promise.all(tasks)
来源：http://nry.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qyc.fanxiaobao.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vug.52xcode.cn

Ruby: threads.map(&:join)
来源：http://bub.aibaodan.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rps.vehdjk.com

[O06] 使用进程池
来源：http://xqz.jinyuanbaomall.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://amt.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nqf.tarul.cn

JS:   // child_process / cluster 模块
来源：http://tvf.ydzc1.top

TS:   // child_process / cluster 模块
来源：http://aew.fehbvm.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://egu.chenjidiqi.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vbf.sufxvd.cn

Ruby: // fork 块
来源：http://vsi.sweek.top

C#:   Parallel.For
来源：http://uos.yueranfly.top

================================================================================
来源：http://hnr.guowangkeji.top

P. 常用工具函数
来源：http://qxf.fehbvm.com

================================================================================
来源：http://gbd.tianlin.xyz

[P01] 生成 UUID
来源：http://hqn.sxryk.cn

Py:   str(uuid.uuid4())
来源：http://zdw.yj20258.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nix.daxiang520.top

JS:   crypto.randomUUID()
来源：http://dvm.cqqwz.cn

TS:   crypto.randomUUID()
来源：http://pdj.sysykeji.top

Java: UUID.randomUUID().toString()
来源：http://dol.jiagoushi.top

Go:   // 用 github.com/google/uuid
来源：http://hat.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://mzd.jinqigufen.top

C#:   Guid.NewGuid().ToString()
来源：http://afi.ivvv.top

[P02] MD5 / SHA256 摘要
来源：http://jnf.bbcook.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oix.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lbq.andypj.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qqs.birdmap.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eee.sxryk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gqr.sweek.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rzj.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oqw.sweek.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xxb.birdmap.top

[P03] 生成短随机字符串
来源：http://jej.svipenyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uyb.zhaomingkeji.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dtd.yj202588.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gsd.yj20258888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mrm.cheryme.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://abm.tian-w.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wae.dianchejie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ots.vqdsnc.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ale.cucudq.cn

[P04] 求长度
来源：http://boh.jqgufenzy.top


<!-- 参考信息 -->