代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vwf.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://avl.gzhubu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vcq.aibaodan.cn

[L06] 解析响应为 JSON
来源：http://vxo.52xcode.cn

Py:   resp.json()
来源：http://cqm.xziqi.cn

PHP:  json_decode($body, true);
来源：http://bnk.cdnleiting.top

JS:   await resp.json()
来源：http://jfg.52xcode.cn

TS:   await resp.json()
来源：http://mbr.jinghuilouyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lgs.fzhhl.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xmv.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://xii.yanxiufei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://awp.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://vjn.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hbk.snrcjt.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uav.sweek.top

JS:   resp.ok;  resp.status
来源：http://zoh.cdnleiting.top

TS:   resp.ok;  resp.status
来源：http://jsq.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://eqs.gaohongyu789.top

Go:   resp.StatusCode
来源：http://qlw.jinghuilouyu.cn

Ruby: resp.code.to_i
来源：http://tfb.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://fdi.jianghu66.top

[L08] 并发请求多个地址
来源：http://acj.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hys.cashguo.top

PHP:  curl_multi_init() 系列
来源：http://dvh.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qkm.zycfv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://svf.shuidangran.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zeq.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nbn.xuetiantiany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eov.ppjwa.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ejk.sysykeji.top

================================================================================
来源：http://mob.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://uls.aizwys.cn

================================================================================
来源：http://phg.sxryk.cn

[M01] 读取命令行参数
来源：http://lmi.hesvh.cn

Py:   sys.argv[1:]
来源：http://fnz.zhongyouzk.top

PHP:  $argv;  $argc;
来源：http://mxv.hammf.cn

JS:   process.argv.slice(2)
来源：http://sxh.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://sgu.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://ncu.havefunace.top

Go:   os.Args[1:]
来源：http://rfq.nanxuanxn.top

Ruby: ARGV
来源：http://zit.ydzc1.top

C#:   args 数组（Main 方法参数）
来源：http://xac.xinyue.icu

[M02] 读取环境变量
来源：http://hoi.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://jpz.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://suv.zhongyouzk.top

JS:   process.env.HOME
来源：http://oox.fzhhl.top

TS:   process.env.HOME
来源：http://nwz.guannengcc.top

Java: System.getenv("HOME")
来源：http://jup.zhiwuduotai.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nzn.jiagoushi.top

Ruby: ENV["HOME"]
来源：http://juu.pengpengdd.cyou

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ezu.c1oappe.top

[M03] 执行外部命令
来源：http://itu.ybcxt.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jrg.sysykeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jnd.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wcr.yuanzhike.top

TS:   child_process.execSync("ls -l").toString()
来源：http://evh.yuxming.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nwu.chenlongwang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qdd.316326.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://iot.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://cul.hywenlv.cn

[M04] 获取当前工作目录
来源：http://fng.hysaishi.cn

Py:   os.getcwd()
来源：http://vnm.9152youxi.cn

PHP:  getcwd();
来源：http://arq.yanxiufei.cn

JS:   process.cwd()
来源：http://pcz.shzxlz.cn

TS:   process.cwd()
来源：http://xtj.xziqi.cn

Java: Path.of("").toAbsolutePath()
来源：http://ycz.wangdashe.top

Go:   os.Getwd()
来源：http://trg.xingfuxueyuan.xyz

Ruby: Dir.pwd
来源：http://euw.redwolf501.top

C#:   Directory.GetCurrentDirectory()
来源：http://woj.ybcxt.top

[M05] 设置退出码
来源：http://zlx.yj20258.top

Py:   sys.exit(1)
来源：http://vbi.hcnkem.com

PHP:  exit(1);
来源：http://pnp.pycfn.com

JS:   process.exit(1)
来源：http://lsn.sjlbkw.cn

TS:   process.exit(1)
来源：http://cwo.pengpengdd.cyou

Java: System.exit(1)
来源：http://nft.quarkkingdee.top

Go:   os.Exit(1)
来源：http://rzk.shzxlz.cn

Ruby: exit 1
来源：http://mwb.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bji.9152youxi.cn

[M06] 向标准错误输出
来源：http://izt.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://kgd.c1oappe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rsw.mhx1999.top

JS:   console.error("err")
来源：http://kgh.gotoacloud.top

TS:   console.error("err")
来源：http://eqs.dianchejie.cn

Java: System.err.println("err")
来源：http://gzb.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gux.xuetiantiany.cn

Ruby: warn "err"
来源：http://ljr.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://yex.tanke756.top

[M07] 判断是否为主入口
来源：http://jtz.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://kjb.daxiang520.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wzf.jqgufenzy.top

JS:   require.main === module
来源：http://nuz.jqgfzy.top

TS:   require.main === module
来源：http://dqq.vqdsnc.cn

Java: public static void main(String[] args)
来源：http://irq.316326.xyz

Go:   func main()
来源：http://sgf.zycfv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dss.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://mmx.c1oappe.top

[M08] 获取系统与运行时信息
来源：http://lxd.cashguo.top

Py:   platform.system();  platform.python_version()
来源：http://ytv.andypj.xyz

PHP:  PHP_OS;  phpversion();
来源：http://cjj.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://gvo.aizwys.cn

TS:   process.platform;  process.version
来源：http://qxy.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oro.havefunace.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sql.hfpthk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xnn.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tgr.xinyue.icu

================================================================================
来源：http://tau.chenzaomai.com

N. 数据结构与算法
来源：http://zbh.xuanzx.com

================================================================================
来源：http://msp.svipenyu.cn

[N01] 二分查找（有序数组）
来源：http://gem.daria6918.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jro.zhixingplan.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nsi.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lwu.yuanzhike.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ywc.gaohongyu789.top

Java: Arrays.binarySearch(arr, x)
来源：http://msq.hnxiangtu.top

Go:   sort.SearchInts(arr, x)
来源：http://vuc.yj202588.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://uok.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xmj.epnwcf.com

[N02] 排序（工程实践用内置实现）
来源：http://wbh.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://gzg.9152youxi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wrv.feifeiyinyue.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kvj.tian-w.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mdl.xinyue.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vjf.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://htv.hcnkem.com

Ruby: arr.sort
来源：http://tnx.smart0.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://wjk.tarul.cn

[N03] 快速排序（分治示例）
来源：http://tas.jinyuanbaomall.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jnm.jinqigfzy.top

PHP:  // 递归实现，或用 usort
来源：http://tjp.tian-w.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jgc.cheryme.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vwc.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aba.chenzaomai.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uea.hfpthk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ttt.ywan-chungtsiang.top

C#:   // 手写递归，或 Array.Sort
来源：http://nmq.yanxiufei.cn

[N04] 斐波那契数列
来源：http://oiy.bjfxy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cma.zdbjq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://itt.vehdjk.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fqm.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://awe.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jwi.zhengqikj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dte.aizwys.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mqj.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ked.hnqzz.top

[N05] 最大公约数
来源：http://lal.shzxlz.cn

Py:   math.gcd(a, b)
来源：http://vxc.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xhy.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nen.gogol.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mlg.iojbl.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kmm.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://plt.shuidangran.top

Ruby: a.gcd(b)
来源：http://bmy.ppjwa.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pfd.fzhhl.top

[N06] 判断回文字符串
来源：http://rkc.quarkkingdee.top

Py:   s == s[::-1]
来源：http://uhw.ydzc1.top

PHP:  $s === strrev($s);
来源：http://gsi.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://rgn.hammf.cn

TS:   s === [...s].reverse().join("")
来源：http://rfe.smart0.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xjl.guowangkeji.top

Go:   // 双指针从两端比较
来源：http://yef.yj202588.top

Ruby: s == s.reverse
来源：http://vxq.birdmap.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tac.xuetiantiany.cn

[N07] 两数之和（返回下标）
来源：http://zhu.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pue.shanyushiyangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jxp.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zks.ydjk.org.cn

TS:   // 手写 Map<string, number>
来源：http://txy.yueranfly.top

Java: // 手写 HashMap
来源：http://iuw.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://urg.yangfankeji.com

Ruby: // 手写 Hash
来源：http://aid.bbcook.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nex.feifeiyinyue.top

[N08] 生成全排列
来源：http://dsk.shangyingyoupin.top

Py:   itertools.permutations(arr)
来源：http://nym.sufxvd.cn

PHP:  // 手写递归交换
来源：http://nmz.xinyue.icu

JS:   // 手写回溯递归
来源：http://akk.cqqwz.cn

TS:   // 手写回溯递归
来源：http://cki.svipenyu.cn

Java: // 手写回溯递归
来源：http://paw.fanxiaobao.xyz

Go:   // 手写回溯递归
来源：http://ygg.chenjidiqi.icu

Ruby: arr.permutation.to_a
来源：http://wlu.0kj1m.cn

C#:   // 手写回溯递归
来源：http://mtr.zdbjq.cn

[N09] 栈与队列
来源：http://wwk.iojbl.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kqd.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cxy.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tun.ybcxt.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://emd.yfazqb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fxg.birdmap.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zdu.iojbl.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yln.tianlin.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bqa.chenzaomai.com

[N10] 链表节点定义
来源：http://rtd.fzhhl.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wcn.shanyushiyangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vvp.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ayg.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dex.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://knq.zhijiandao.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uqf.daxiang520.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hkh.jinqigufen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sye.9152youxi.cn

[N11] 二叉树中序遍历
来源：http://uvr.hysaishi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ycn.smart0.xyz

PHP:  // 手写递归函数
来源：http://bjj.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oal.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hqr.yueranfly.top

Java: // 手写递归
来源：http://mfe.zycfv.cn

Go:   // 手写递归
来源：http://gou.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tnc.birdmap.top

C#:   // 手写递归
来源：http://kkl.yvedp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ims.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bwy.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://emj.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://brh.0kj1m.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mmf.ivvv.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hle.316326.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uji.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kop.fehbvm.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://beo.yonumen.top

================================================================================
来源：http://fty.ivvv.top

O. 并发与异步
来源：http://hum.andypj.xyz

================================================================================
来源：http://jdu.hammf.cn

[O01] 启动一个线程
来源：http://ckq.sufxvd.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oqe.shangyingyoupin.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jmo.tian-w.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hkz.zdqjudy.top

TS:   // 同 JS
来源：http://fmr.aibaodan.cn

Java: new Thread(() -> f()).start()
来源：http://ysi.xziqi.cn

Go:   go f()
来源：http://ztn.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://vzu.jqgufenzy.top

C#:   Task.Run(() => F());
来源：http://uan.wangshuangyany.cn

[O02] 使用线程池
来源：http://rna.andypj.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://plc.hnxiangtu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tui.epnwcf.com

JS:   // worker_threads 线程池
来源：http://onq.yj20258888.top

TS:   // worker_threads 线程池
来源：http://dhm.yanxiufei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kwp.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bba.gzhubu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jvm.xziqi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://smh.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://yhc.gotoacloud.top

Py:   with lock: shared += 1
来源：http://hyk.guowangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://mez.shuidangran.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sra.hcnkem.com

TS:   // 同 JS
来源：http://aln.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://tlb.cucudq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zln.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ptd.ivvv.top

C#:   lock (gate) { shared++; }
来源：http://pjb.cqqwz.cn

[O04] 定义异步函数并等待
来源：http://vrj.zhoulong.xyz

Py:   async def f():⏎    await g()
来源：http://tst.redwolf501.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gtp.ydzc1.top

JS:   async function f() { await g(); }
来源：http://mso.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://axe.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://csi.yj202588.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ide.jqgfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://uvv.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://woc.yuanzhike.top

[O05] 并发执行并等待全部完成
来源：http://zqz.zdbjq.cn

Py:   asyncio.gather(*tasks)
来源：http://miz.c1oappe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gjk.sweek.top

JS:   await Promise.all(tasks)
来源：http://xrx.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://phf.zhijiandao.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mda.wangshuangyany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kxd.daxiang520.top

Ruby: threads.map(&:join)
来源：http://end.gaohongyu789.top

C#:   await Task.WhenAll(t1, t2)
来源：http://yjb.bjfxy.top

[O06] 使用进程池
来源：http://eyq.cqqwz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vjm.ppjwa.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hpw.guowangkeji.top

JS:   // child_process / cluster 模块
来源：http://kxc.iojbl.cn

TS:   // child_process / cluster 模块
来源：http://pkk.xylfe.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://luf.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ptq.zhixingplan.top

Ruby: // fork 块
来源：http://axa.gotoacloud.top

C#:   Parallel.For
来源：http://xrt.zhongyouzk.top

================================================================================
来源：http://vek.hcnkem.com

P. 常用工具函数
来源：http://cai.gaohongyu789.top

================================================================================
来源：http://nqb.uphjek.com

[P01] 生成 UUID
来源：http://rar.zhiwuduotai.top

Py:   str(uuid.uuid4())
来源：http://laf.zhixingplan.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://veq.sysykeji.top

JS:   crypto.randomUUID()
来源：http://whl.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://iau.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://tog.dashuyun.cn

Go:   // 用 github.com/google/uuid
来源：http://qpa.shangyingyoupin.top

Ruby: SecureRandom.uuid
来源：http://tde.hcnkem.com

C#:   Guid.NewGuid().ToString()
来源：http://byk.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://ocl.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gar.fktsv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hvm.uphjek.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gnn.zdqjudy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ylk.wangshuangyany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gbd.bbcook.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ogb.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bui.sweek.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://teu.tianlin.xyz

[P03] 生成短随机字符串
来源：http://xei.cdnleiting.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vyf.yonumen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hfo.zhongyouzk.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zsh.tian-w.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wds.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fdt.yj202588.top


<!-- 参考信息 -->