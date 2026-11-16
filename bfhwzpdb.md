代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tzo.c1oappe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fzm.havefunace.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pph.zhoulong.xyz

[L06] 解析响应为 JSON
来源：http://ogs.svipenyu.cn

Py:   resp.json()
来源：http://pzz.yj202588.top

PHP:  json_decode($body, true);
来源：http://pom.c1oappe.top

JS:   await resp.json()
来源：http://gdy.zdqjudy.top

TS:   await resp.json()
来源：http://jkw.ehwqpu.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oqf.ybcxt.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ayy.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://lxo.jiagoushi.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mgi.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://xjc.bbcook.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cru.yvedp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dpk.yuxming.cn

JS:   resp.ok;  resp.status
来源：http://qeg.aibaodan.cn

TS:   resp.ok;  resp.status
来源：http://lck.yj20258.top

Java: resp.statusCode()
来源：http://opy.daria6918.cn

Go:   resp.StatusCode
来源：http://ddz.xingfuxueyuan.xyz

Ruby: resp.code.to_i
来源：http://vpk.ppjwa.cn

C#:   (int)resp.StatusCode
来源：http://khv.nwbrower.top

[L08] 并发请求多个地址
来源：http://yra.zycfv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://arw.birdmap.top

PHP:  curl_multi_init() 系列
来源：http://zvt.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zzg.ehwqpu.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xhw.jqgufenzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fdb.fzhhl.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fcd.zhijiandao.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xwh.fanxiaobao.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://exe.zdbjq.cn

================================================================================
来源：http://lzw.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://psc.fanxiaobao.xyz

================================================================================
来源：http://ozi.yangfankeji.com

[M01] 读取命令行参数
来源：http://sob.gogol.net.cn

Py:   sys.argv[1:]
来源：http://xkd.sysykeji.top

PHP:  $argv;  $argc;
来源：http://syc.c1oappe.top

JS:   process.argv.slice(2)
来源：http://xub.haohaochexian.top

TS:   process.argv.slice(2)
来源：http://hzl.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://kzj.cdnleiting.top

Go:   os.Args[1:]
来源：http://jss.birdmap.top

Ruby: ARGV
来源：http://iyr.zdqjudy.top

C#:   args 数组（Main 方法参数）
来源：http://uqq.tianlin.xyz

[M02] 读取环境变量
来源：http://xzr.smart0.xyz

Py:   os.environ.get("HOME")
来源：http://qhk.gaohongyu789.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://skm.sufxvd.cn

JS:   process.env.HOME
来源：http://cng.zdbjq.cn

TS:   process.env.HOME
来源：http://moj.c1oappe.top

Java: System.getenv("HOME")
来源：http://jhk.hcnkem.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ndd.snrcjt.cn

Ruby: ENV["HOME"]
来源：http://nnb.haohaochexian.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kkf.daxiang520.top

[M03] 执行外部命令
来源：http://hpu.hongshengwenyu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://szz.yuxming.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hfb.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yjd.mhx1999.top

TS:   child_process.execSync("ls -l").toString()
来源：http://khv.yongpay.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gzn.dashuyun.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nkb.fehbvm.com

Ruby: system("ls -l");  `ls -l`
来源：http://pdw.yuxming.cn

C#:   Process.Start("ls", "-l");
来源：http://eyq.uphjek.com

[M04] 获取当前工作目录
来源：http://dwj.fzhhl.top

Py:   os.getcwd()
来源：http://yej.tarul.cn

PHP:  getcwd();
来源：http://ccp.jlsjyb.cn

JS:   process.cwd()
来源：http://vqe.yj20258888.top

TS:   process.cwd()
来源：http://shq.kuanghao11.cn

Java: Path.of("").toAbsolutePath()
来源：http://dzw.bjfxy.top

Go:   os.Getwd()
来源：http://jmd.aizwys.cn

Ruby: Dir.pwd
来源：http://hmo.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://ncf.gzhubu.top

[M05] 设置退出码
来源：http://tuk.smart0.xyz

Py:   sys.exit(1)
来源：http://dxa.jqgfzy.top

PHP:  exit(1);
来源：http://kkh.fanxiaobao.xyz

JS:   process.exit(1)
来源：http://uab.iojbl.cn

TS:   process.exit(1)
来源：http://azy.andypj.xyz

Java: System.exit(1)
来源：http://nbk.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://jna.fzhhl.top

Ruby: exit 1
来源：http://oqt.birdmap.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gzn.cqqwz.cn

[M06] 向标准错误输出
来源：http://fwk.chenzaomai.com

Py:   print("err", file=sys.stderr)
来源：http://cma.iojbl.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ott.chenlongwang.top

JS:   console.error("err")
来源：http://hmw.jianghu66.top

TS:   console.error("err")
来源：http://whv.tian-w.cn

Java: System.err.println("err")
来源：http://aok.c1oappe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://keh.feifeiyinyue.top

Ruby: warn "err"
来源：http://mac.shanyushiyangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://sii.yonumen.top

[M07] 判断是否为主入口
来源：http://mdb.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://cpf.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bdn.xuetiantiany.cn

JS:   require.main === module
来源：http://roy.yvedp.cn

TS:   require.main === module
来源：http://fxx.zhongyouzk.top

Java: public static void main(String[] args)
来源：http://efj.zhixingplan.top

Go:   func main()
来源：http://xvh.ywan-chungtsiang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fbn.zycfv.cn

C#:   static void Main(string[] args)
来源：http://pjx.fengsongda.top

[M08] 获取系统与运行时信息
来源：http://omv.sxryk.cn

Py:   platform.system();  platform.python_version()
来源：http://eba.316326.xyz

PHP:  PHP_OS;  phpversion();
来源：http://oez.tanke756.top

JS:   process.platform;  process.version
来源：http://ydr.ivvv.top

TS:   process.platform;  process.version
来源：http://qyi.hcnkem.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vhh.redwolf501.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ivu.zhaomingkeji.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mwu.svipenyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://raq.zhongyouzk.top

================================================================================
来源：http://xit.hnxiangtu.top

N. 数据结构与算法
来源：http://vxv.snrcjt.cn

================================================================================
来源：http://mcv.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://snu.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://kfp.chenzaomai.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rcv.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hbn.nanxinkj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wlm.jlsjyb.cn

Java: Arrays.binarySearch(arr, x)
来源：http://phb.hongshengwenyu.top

Go:   sort.SearchInts(arr, x)
来源：http://smg.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gfa.zhijiandao.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zhk.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://pfs.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://xwy.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ewp.9152youxi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ols.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bqy.birdmap.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bgt.jinqigfzy.top

Go:   slices.Sort(arr)
来源：http://tqw.xinyue.icu

Ruby: arr.sort
来源：http://iyc.jyoumei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hqw.yanxiufei.cn

[N03] 快速排序（分治示例）
来源：http://bgr.tanke756.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dvj.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://jwy.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yzd.quarkkingdee.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lxp.guowangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hnu.andypj.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uxm.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mxk.redwolf501.top

C#:   // 手写递归，或 Array.Sort
来源：http://pfq.ydzc1.top

[N04] 斐波那契数列
来源：http://kjf.wangshuangyany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tzv.chenlongwang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bwz.jianghu66.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lba.shanyushiyangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hzp.yanxiufei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qrd.tianlin.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://een.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://imc.chenlongwang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://frn.haohaochexian.top

[N05] 最大公约数
来源：http://jte.bbcook.cn

Py:   math.gcd(a, b)
来源：http://emi.cqqwz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://abv.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bcq.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rpq.jinqigufen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kru.haohaochexian.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lod.zycfv.cn

Ruby: a.gcd(b)
来源：http://cod.sxryk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://krs.aibaodan.cn

[N06] 判断回文字符串
来源：http://qhe.jiagoushi.top

Py:   s == s[::-1]
来源：http://ipv.fengsongda.top

PHP:  $s === strrev($s);
来源：http://isl.shangyingyoupin.top

JS:   s === [...s].reverse().join("")
来源：http://dut.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://jft.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tns.ybcxt.top

Go:   // 双指针从两端比较
来源：http://nny.daria6918.cn

Ruby: s == s.reverse
来源：http://sad.chenlongwang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bda.uphjek.com

[N07] 两数之和（返回下标）
来源：http://agv.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rxh.sweek.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xwd.gaohongyu789.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vjn.havefunace.top

TS:   // 手写 Map<string, number>
来源：http://qlg.jyoumei.cn

Java: // 手写 HashMap
来源：http://idv.jianghu66.top

Go:   // 手写 map[int]int
来源：http://qji.ctjpmb.com

Ruby: // 手写 Hash
来源：http://zya.hysaishi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://umd.chenzaomai.com

[N08] 生成全排列
来源：http://rkm.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://alo.cqqwz.cn

PHP:  // 手写递归交换
来源：http://ign.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://iqw.xuetiantiany.cn

TS:   // 手写回溯递归
来源：http://kbx.hysaishi.cn

Java: // 手写回溯递归
来源：http://qff.svipenyu.cn

Go:   // 手写回溯递归
来源：http://lqk.xylfe.cn

Ruby: arr.permutation.to_a
来源：http://axn.jinqigfzy.top

C#:   // 手写回溯递归
来源：http://fif.redwolf501.top

[N09] 栈与队列
来源：http://xrb.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fik.hongshengwenyu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rel.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lmv.snrcjt.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bpl.epnwcf.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://twx.yueranfly.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zyg.ctjpmb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://asn.ywan-chungtsiang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zoo.gotoacloud.top

[N10] 链表节点定义
来源：http://dsp.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cgw.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fub.pengpengdd.cyou

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wgf.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ygp.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://lwj.yj20258.top

Go:   type Node struct { V int; Next *Node }
来源：http://olz.yuxming.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ott.sweek.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zrl.shzxlz.cn

[N11] 二叉树中序遍历
来源：http://mzj.gotoacloud.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mfe.zhengqikj.top

PHP:  // 手写递归函数
来源：http://bvt.pycfn.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lrk.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ziq.andypj.xyz

Java: // 手写递归
来源：http://ppt.yuxming.cn

Go:   // 手写递归
来源：http://hly.xziqi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rso.yuxming.cn

C#:   // 手写递归
来源：http://kig.uphjek.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://irk.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wjk.zhiwuduotai.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aol.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://swx.yuxming.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ggf.feifeiyinyue.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kvi.redwolf501.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lcr.aibaodan.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nhb.meibo888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cjb.hfpthk.cn

================================================================================
来源：http://jgt.meibo888.top

O. 并发与异步
来源：http://mzk.xinyue.icu

================================================================================
来源：http://msr.andypj.xyz

[O01] 启动一个线程
来源：http://qqu.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rsl.feifeiyinyue.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://urj.zhengqikj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://txv.quarkkingdee.top

TS:   // 同 JS
来源：http://cgy.haohaochexian.top

Java: new Thread(() -> f()).start()
来源：http://hyx.jinqigfzy.top

Go:   go f()
来源：http://fdo.yuxming.cn

Ruby: Thread.new { f }
来源：http://lhe.daxiang520.top

C#:   Task.Run(() => F());
来源：http://dfw.feifeiyinyue.top

[O02] 使用线程池
来源：http://ppc.ivvv.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cns.birdmap.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ccc.jyoumei.cn

JS:   // worker_threads 线程池
来源：http://hcf.havefunace.top

TS:   // worker_threads 线程池
来源：http://hjc.yueranfly.top

Java: Executors.newFixedThreadPool(4)
来源：http://gpw.ydjk.org.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jdz.sjlbkw.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bea.wangshuangyany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gxs.jinyuanbaomall.cn

[O03] 加锁保护共享数据
来源：http://xiw.yueranfly.top

Py:   with lock: shared += 1
来源：http://fdl.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://sqm.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jhk.52xcode.cn

TS:   // 同 JS
来源：http://aau.guannengcc.top

Java: synchronized (this) { shared++; }
来源：http://dlf.yanxiufei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vym.yvedp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vml.havefunace.top

C#:   lock (gate) { shared++; }
来源：http://kse.guowangkeji.top

[O04] 定义异步函数并等待
来源：http://yfh.ywan-chungtsiang.top

Py:   async def f():⏎    await g()
来源：http://qcv.quarkkingdee.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mkk.jqgufenzy.top

JS:   async function f() { await g(); }
来源：http://ylg.zdbjq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hef.cucudq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wkh.dashuyun.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hub.xinyue.icu

Ruby: # 用 Fiber 或 async gem
来源：http://qkc.quarkkingdee.top

C#:   async Task F() { await G(); }
来源：http://ssr.xuanzx.com

[O05] 并发执行并等待全部完成
来源：http://mpg.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://mlu.yvedp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zje.jlsjyb.cn

JS:   await Promise.all(tasks)
来源：http://jyf.svipenyu.cn

TS:   await Promise.all(tasks)
来源：http://vjg.tanke756.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hot.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uzz.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://pfx.ydjk.org.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vpx.316326.xyz

[O06] 使用进程池
来源：http://wph.svipenyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fpb.yj20258888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://elx.feifeiyinyue.top

JS:   // child_process / cluster 模块
来源：http://qcs.ybcxt.top

TS:   // child_process / cluster 模块
来源：http://sov.tarul.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mvx.wangshuangyany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sqv.yvedp.cn

Ruby: // fork 块
来源：http://hde.haohaochexian.top

C#:   Parallel.For
来源：http://vnc.ehwqpu.com

================================================================================
来源：http://dqg.xingfuxueyuan.xyz

P. 常用工具函数
来源：http://cto.cashguo.top

================================================================================
来源：http://pxu.sufxvd.cn

[P01] 生成 UUID
来源：http://smc.sysykeji.top

Py:   str(uuid.uuid4())
来源：http://emt.fzhhl.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wov.hesvh.cn

JS:   crypto.randomUUID()
来源：http://qyv.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://fsj.hywenlv.cn

Java: UUID.randomUUID().toString()
来源：http://xzi.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://ybf.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://wqa.vehdjk.com

C#:   Guid.NewGuid().ToString()
来源：http://gyy.yangfankeji.com

[P02] MD5 / SHA256 摘要
来源：http://yxc.jqgufenzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tkm.sweek.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nfl.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cwt.ywan-chungtsiang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sgb.daria6918.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ppl.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xjv.daria6918.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hdn.hywenlv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ukd.zycfv.cn

[P03] 生成短随机字符串
来源：http://joy.hesvh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qes.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gbm.shanyushiyangtech.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yqk.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mki.nwbrower.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ylg.chenzaomai.com


<!-- 参考信息 -->