代发 wailian999

Py:   resp.json()
来源：http://zwy.jiagoushi.top

PHP:  json_decode($body, true);
来源：http://pgl.xylfe.cn

JS:   await resp.json()
来源：http://ajt.yanxiufei.cn

TS:   await resp.json()
来源：http://uzy.nanxuanxn.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hxf.jqgufenzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hoe.yvedp.cn

Ruby: JSON.parse(resp.body)
来源：http://hpz.hywenlv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gfr.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://edg.iojbl.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wwf.xuetiantiany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ksz.cashguo.top

JS:   resp.ok;  resp.status
来源：http://goe.daxiang520.top

TS:   resp.ok;  resp.status
来源：http://sif.shzxlz.cn

Java: resp.statusCode()
来源：http://pdc.xingfuxueyuan.xyz

Go:   resp.StatusCode
来源：http://mja.zhongyouzk.top

Ruby: resp.code.to_i
来源：http://qgr.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://qnz.redwolf501.top

[L08] 并发请求多个地址
来源：http://sfj.aizwys.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xnr.yangfankeji.com

PHP:  curl_multi_init() 系列
来源：http://mgi.hnxiangtu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cgn.jinghuilouyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tgj.daxiang520.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zjv.ybcxt.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://thm.havefunace.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jpn.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fic.ybcxt.top

================================================================================
来源：http://qri.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://eey.xinyue.icu

================================================================================
来源：http://dtx.bjfxy.top

[M01] 读取命令行参数
来源：http://svw.tianlin.xyz

Py:   sys.argv[1:]
来源：http://bte.yongpay.top

PHP:  $argv;  $argc;
来源：http://xtj.c1oappe.top

JS:   process.argv.slice(2)
来源：http://qha.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://min.jinghuilouyu.cn

Java: args 数组（main 方法参数）
来源：http://ats.fktsv.cn

Go:   os.Args[1:]
来源：http://yyp.zhijiandao.cn

Ruby: ARGV
来源：http://xhq.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://cco.shuidangran.top

[M02] 读取环境变量
来源：http://yhp.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://uyt.ydzc1.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://khw.quarkkingdee.top

JS:   process.env.HOME
来源：http://lvi.yj202588.top

TS:   process.env.HOME
来源：http://mlr.yvedp.cn

Java: System.getenv("HOME")
来源：http://cww.nanxuanxn.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kmp.hywenlv.cn

Ruby: ENV["HOME"]
来源：http://ube.yuxming.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://juk.zhongyouzk.top

[M03] 执行外部命令
来源：http://yxo.ydzc1.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://byb.daxiang520.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rss.vqdsnc.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jgk.gaohongyu789.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tyd.jiagoushi.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cmq.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dkq.cashguo.top

Ruby: system("ls -l");  `ls -l`
来源：http://opj.xuanzx.com

C#:   Process.Start("ls", "-l");
来源：http://oub.sufxvd.cn

[M04] 获取当前工作目录
来源：http://vst.jlsjyb.cn

Py:   os.getcwd()
来源：http://ehr.ppjwa.cn

PHP:  getcwd();
来源：http://fgz.yj20258888.top

JS:   process.cwd()
来源：http://yms.jyoumei.cn

TS:   process.cwd()
来源：http://ada.jqgfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://cmg.daxiang520.top

Go:   os.Getwd()
来源：http://thw.xylfe.cn

Ruby: Dir.pwd
来源：http://jpi.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://vju.yj20258888.top

[M05] 设置退出码
来源：http://opb.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://rwa.zdqjudy.top

PHP:  exit(1);
来源：http://bec.yonumen.top

JS:   process.exit(1)
来源：http://fmz.chenlongwang.top

TS:   process.exit(1)
来源：http://yhd.snrcjt.cn

Java: System.exit(1)
来源：http://yqg.xylfe.cn

Go:   os.Exit(1)
来源：http://lfu.hywenlv.cn

Ruby: exit 1
来源：http://loz.jianghu66.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iff.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://mkh.xziqi.cn

Py:   print("err", file=sys.stderr)
来源：http://lwj.jianghu66.top

PHP:  fwrite(STDERR, "err\n");
来源：http://udk.chenzaomai.com

JS:   console.error("err")
来源：http://mrw.ivvv.top

TS:   console.error("err")
来源：http://tex.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://tbm.guannengcc.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://swn.yongpay.top

Ruby: warn "err"
来源：http://dmq.fehbvm.com

C#:   Console.Error.WriteLine("err")
来源：http://mcs.yj20258.top

[M07] 判断是否为主入口
来源：http://ltp.yj202588.top

Py:   if __name__ == "__main__":
来源：http://pat.bbcook.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uhg.dianchejie.cn

JS:   require.main === module
来源：http://quu.jinqigufen.top

TS:   require.main === module
来源：http://dyc.zhijiandao.cn

Java: public static void main(String[] args)
来源：http://ouj.fzhhl.top

Go:   func main()
来源：http://yrq.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bot.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://elr.vqdsnc.cn

[M08] 获取系统与运行时信息
来源：http://pah.sxryk.cn

Py:   platform.system();  platform.python_version()
来源：http://wnd.yuxming.cn

PHP:  PHP_OS;  phpversion();
来源：http://fur.yangfankeji.com

JS:   process.platform;  process.version
来源：http://spg.shanyushiyangtech.top

TS:   process.platform;  process.version
来源：http://krx.ybcxt.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ejp.shanyushiyangtech.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tzk.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nie.epnwcf.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://vvd.jqgufenzy.top

================================================================================
来源：http://imw.316326.xyz

N. 数据结构与算法
来源：http://spu.zhoulong.xyz

================================================================================
来源：http://xke.tanke756.top

[N01] 二分查找（有序数组）
来源：http://lki.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://pcw.xylfe.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xbp.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dlg.yvedp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://low.bbcook.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rsl.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://hdt.jinyuanbaomall.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://aen.tanke756.top

C#:   Array.BinarySearch(arr, x)
来源：http://uwl.c1oappe.top

[N02] 排序（工程实践用内置实现）
来源：http://zii.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://ciz.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sfv.havefunace.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bww.ybcxt.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://des.yj20258888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xcv.sweek.top

Go:   slices.Sort(arr)
来源：http://jgz.pengpengdd.cyou

Ruby: arr.sort
来源：http://zzt.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lum.zhoulong.xyz

[N03] 快速排序（分治示例）
来源：http://gzh.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zqw.yj20258.top

PHP:  // 递归实现，或用 usort
来源：http://psx.cqqwz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pqv.pengpengdd.cyou

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vxy.tian-w.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gjt.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xmi.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://onx.gotoacloud.top

C#:   // 手写递归，或 Array.Sort
来源：http://fmp.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://tzs.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rzb.hnxiangtu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://quh.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wab.zdbjq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nxv.nanxuanxn.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mhv.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zeq.316326.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dib.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nao.fzhhl.top

[N05] 最大公约数
来源：http://ppl.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://bgm.vehdjk.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cca.shangyingyoupin.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pvr.yuanzhike.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xic.cucudq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nuo.yfazqb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ery.gzhubu.top

Ruby: a.gcd(b)
来源：http://uwm.zhoulong.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kcv.xuanzx.com

[N06] 判断回文字符串
来源：http://ceo.snrcjt.cn

Py:   s == s[::-1]
来源：http://lkd.chenjidiqi.icu

PHP:  $s === strrev($s);
来源：http://mqg.jlsjyb.cn

JS:   s === [...s].reverse().join("")
来源：http://udi.fengsongda.top

TS:   s === [...s].reverse().join("")
来源：http://mql.ydjk.org.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wvl.jiagoushi.top

Go:   // 双指针从两端比较
来源：http://ipz.jlsjyb.cn

Ruby: s == s.reverse
来源：http://aqy.cqqwz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ijw.jinqigfzy.top

[N07] 两数之和（返回下标）
来源：http://jwv.birdmap.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lan.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cym.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://jml.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://loj.haohaochexian.top

Java: // 手写 HashMap
来源：http://hop.tian-w.cn

Go:   // 手写 map[int]int
来源：http://dep.xylfe.cn

Ruby: // 手写 Hash
来源：http://lez.wangdashe.top

C#:   // 手写 Dictionary<int, int>
来源：http://kxz.sysykeji.top

[N08] 生成全排列
来源：http://wrp.jinqigfzy.top

Py:   itertools.permutations(arr)
来源：http://xwf.jiagoushi.top

PHP:  // 手写递归交换
来源：http://xjc.xziqi.cn

JS:   // 手写回溯递归
来源：http://xzu.fktsv.cn

TS:   // 手写回溯递归
来源：http://kry.yvedp.cn

Java: // 手写回溯递归
来源：http://sya.hcnkem.com

Go:   // 手写回溯递归
来源：http://poy.sufxvd.cn

Ruby: arr.permutation.to_a
来源：http://uao.epnwcf.com

C#:   // 手写回溯递归
来源：http://cqs.0kj1m.cn

[N09] 栈与队列
来源：http://gli.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://goz.nwbrower.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ivv.zhoulong.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ilt.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dhd.cashguo.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://upl.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ddi.sjlbkw.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nom.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vsd.zhixingplan.top

[N10] 链表节点定义
来源：http://ivc.aibaodan.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nmb.birdmap.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gqu.svipenyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rsr.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nrh.xingfuxueyuan.xyz

Java: class Node { int v; Node next; }
来源：http://fjb.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ojg.epnwcf.com

Ruby: Node = Struct.new(:v, :next)
来源：http://yyo.cucudq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ded.hesvh.cn

[N11] 二叉树中序遍历
来源：http://ogk.zhongyouzk.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vfp.xuanzx.com

PHP:  // 手写递归函数
来源：http://npl.guannengcc.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rxu.shuidangran.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kxb.cheryme.top

Java: // 手写递归
来源：http://nyr.gaohongyu789.top

Go:   // 手写递归
来源：http://bsn.zdbjq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kty.gotoacloud.top

C#:   // 手写递归
来源：http://bdn.jyoumei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qrk.jyoumei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ijy.yongpay.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fqn.9152youxi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://epr.jinqigufen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yhz.yonumen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ixc.jianghu66.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qdy.dashuyun.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dpj.yonumen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mbp.zhongyouzk.top

================================================================================
来源：http://wxk.aibaodan.cn

O. 并发与异步
来源：http://unw.jinghuilouyu.cn

================================================================================
来源：http://mce.wangshuangyany.cn

[O01] 启动一个线程
来源：http://jid.shzxlz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gjb.jiagoushi.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://igq.hnqzz.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qan.tanke756.top

TS:   // 同 JS
来源：http://dwv.fehbvm.com

Java: new Thread(() -> f()).start()
来源：http://oho.0kj1m.cn

Go:   go f()
来源：http://svf.tanke756.top

Ruby: Thread.new { f }
来源：http://spj.hnqzz.top

C#:   Task.Run(() => F());
来源：http://llj.gotoacloud.top

[O02] 使用线程池
来源：http://kap.kuanghao11.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iko.feifeiyinyue.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://brd.zhengqikj.top

JS:   // worker_threads 线程池
来源：http://awc.cheryme.top

TS:   // worker_threads 线程池
来源：http://nep.bbcook.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bys.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://joh.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ota.0kj1m.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tkp.uphjek.com

[O03] 加锁保护共享数据
来源：http://kfh.hysaishi.cn

Py:   with lock: shared += 1
来源：http://sug.bjfxy.top

PHP:  // 用 flock() 做文件锁
来源：http://fjs.c1oappe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zox.cheryme.top

TS:   // 同 JS
来源：http://xgs.jinyuanbaomall.cn

Java: synchronized (this) { shared++; }
来源：http://vre.ehwqpu.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jsc.birdmap.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wna.hnqzz.top

C#:   lock (gate) { shared++; }
来源：http://pba.chenjidiqi.icu

[O04] 定义异步函数并等待
来源：http://drv.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://hrn.ehwqpu.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://agc.gotoacloud.top

JS:   async function f() { await g(); }
来源：http://yvm.jinqigufen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fsj.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://msn.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rvw.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ycx.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://dnc.hnqzz.top

[O05] 并发执行并等待全部完成
来源：http://var.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://onf.hammf.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wmn.guannengcc.top

JS:   await Promise.all(tasks)
来源：http://tph.hammf.cn

TS:   await Promise.all(tasks)
来源：http://pui.ywan-chungtsiang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://crl.vqdsnc.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ycf.shuidangran.top

Ruby: threads.map(&:join)
来源：http://fnc.quarkkingdee.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mmm.hysaishi.cn

[O06] 使用进程池
来源：http://igs.gzhubu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jgj.jqgfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wjc.yj20258.top

JS:   // child_process / cluster 模块
来源：http://sqz.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://rvq.snrcjt.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bvj.wangdashe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ofs.hywenlv.cn

Ruby: // fork 块
来源：http://qep.yanxiufei.cn

C#:   Parallel.For
来源：http://qkj.316326.xyz

================================================================================
来源：http://qqd.aizwys.cn

P. 常用工具函数
来源：http://phz.havefunace.top

================================================================================
来源：http://cmk.iojbl.cn

[P01] 生成 UUID
来源：http://xwh.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://mhb.yuanzhike.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jvp.shzxlz.cn

JS:   crypto.randomUUID()
来源：http://ynj.0kj1m.cn

TS:   crypto.randomUUID()
来源：http://amf.mhx1999.top

Java: UUID.randomUUID().toString()
来源：http://ddc.xinyue.icu

Go:   // 用 github.com/google/uuid
来源：http://khq.sysykeji.top

Ruby: SecureRandom.uuid
来源：http://lwh.jinqigufen.top

C#:   Guid.NewGuid().ToString()
来源：http://ptf.yfazqb.com

[P02] MD5 / SHA256 摘要
来源：http://rqe.shanyushiyangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wih.tarul.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jcu.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://toi.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oez.zhengqikj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ymf.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qse.hcnkem.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kxz.yanxiufei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xjm.iojbl.cn

[P03] 生成短随机字符串
来源：http://oqv.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://inr.hammf.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pob.fehbvm.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jdo.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eyd.hfpthk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sug.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lci.gogol.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kmo.ehwqpu.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://caa.jianghu66.top

[P04] 求长度
来源：http://tjs.tianlin.xyz


<!-- 参考信息 -->