代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tio.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hzv.tarul.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rlm.cdnleiting.top

[L06] 解析响应为 JSON
来源：http://ukw.xylfe.cn

Py:   resp.json()
来源：http://ytu.havefunace.top

PHP:  json_decode($body, true);
来源：http://whr.jiagoushi.top

JS:   await resp.json()
来源：http://eyr.zdbjq.cn

TS:   await resp.json()
来源：http://jrl.hnxiangtu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mko.hesvh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tnp.feifeiyinyue.top

Ruby: JSON.parse(resp.body)
来源：http://prq.fzhhl.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pwk.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://ysc.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jih.yonumen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mif.zhijiandao.cn

JS:   resp.ok;  resp.status
来源：http://wgt.yuxming.cn

TS:   resp.ok;  resp.status
来源：http://uay.yangfankeji.com

Java: resp.statusCode()
来源：http://hfn.andypj.xyz

Go:   resp.StatusCode
来源：http://jen.ctjpmb.com

Ruby: resp.code.to_i
来源：http://uwb.daria6918.cn

C#:   (int)resp.StatusCode
来源：http://gqp.vqdsnc.cn

[L08] 并发请求多个地址
来源：http://kih.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nak.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://uyx.zdbjq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xhv.pengpengdd.cyou

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fci.snrcjt.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pqx.pengpengdd.cyou

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://suq.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://owt.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ctl.zhoulong.xyz

================================================================================
来源：http://jyz.nanxuanxn.top

M. 命令行 / 进程 / 环境
来源：http://ocb.yangfankeji.com

================================================================================
来源：http://wts.hnxiangtu.top

[M01] 读取命令行参数
来源：http://uop.cdnleiting.top

Py:   sys.argv[1:]
来源：http://lti.fanxiaobao.xyz

PHP:  $argv;  $argc;
来源：http://srq.daxiang520.top

JS:   process.argv.slice(2)
来源：http://pem.ehwqpu.com

TS:   process.argv.slice(2)
来源：http://kgq.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://ahd.ppjwa.cn

Go:   os.Args[1:]
来源：http://vxo.yangfankeji.com

Ruby: ARGV
来源：http://lal.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://pag.cucudq.cn

[M02] 读取环境变量
来源：http://srj.yj202588.top

Py:   os.environ.get("HOME")
来源：http://blr.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rms.pycfn.com

JS:   process.env.HOME
来源：http://itc.hywenlv.cn

TS:   process.env.HOME
来源：http://fah.jinghuilouyu.cn

Java: System.getenv("HOME")
来源：http://gpp.gogol.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://omv.epnwcf.com

Ruby: ENV["HOME"]
来源：http://vee.gogol.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dob.tianlin.xyz

[M03] 执行外部命令
来源：http://doj.xuetiantiany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sfl.mhx1999.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bzj.feifeiyinyue.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vlu.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://edp.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gww.jinqigfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cnq.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hln.sysykeji.top

C#:   Process.Start("ls", "-l");
来源：http://tht.gzhubu.top

[M04] 获取当前工作目录
来源：http://raw.hnqzz.top

Py:   os.getcwd()
来源：http://txf.chenjidiqi.icu

PHP:  getcwd();
来源：http://nia.feifeiyinyue.top

JS:   process.cwd()
来源：http://slz.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://sjj.cheryme.top

Java: Path.of("").toAbsolutePath()
来源：http://rfi.hnxiangtu.top

Go:   os.Getwd()
来源：http://jjr.yj20258888.top

Ruby: Dir.pwd
来源：http://jrs.sjlbkw.cn

C#:   Directory.GetCurrentDirectory()
来源：http://djx.nanxuanxn.top

[M05] 设置退出码
来源：http://tle.gzhubu.top

Py:   sys.exit(1)
来源：http://kdi.ydjk.org.cn

PHP:  exit(1);
来源：http://vju.snrcjt.cn

JS:   process.exit(1)
来源：http://efy.jinqigufen.top

TS:   process.exit(1)
来源：http://xcp.yj20258.top

Java: System.exit(1)
来源：http://zzj.andypj.xyz

Go:   os.Exit(1)
来源：http://jmk.zdbjq.cn

Ruby: exit 1
来源：http://hlm.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ohk.hysaishi.cn

[M06] 向标准错误输出
来源：http://hxa.nwbrower.top

Py:   print("err", file=sys.stderr)
来源：http://bqj.jinqigufen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kjq.c1oappe.top

JS:   console.error("err")
来源：http://bsv.redwolf501.top

TS:   console.error("err")
来源：http://ouf.tianlin.xyz

Java: System.err.println("err")
来源：http://mhg.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rvg.guowangkeji.top

Ruby: warn "err"
来源：http://nlj.smart0.xyz

C#:   Console.Error.WriteLine("err")
来源：http://rmc.yuanzhike.top

[M07] 判断是否为主入口
来源：http://rsz.cheryme.top

Py:   if __name__ == "__main__":
来源：http://kij.fengsongda.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bbc.meibo888.top

JS:   require.main === module
来源：http://bvq.jiagoushi.top

TS:   require.main === module
来源：http://fbl.yj202588.top

Java: public static void main(String[] args)
来源：http://qnn.uphjek.com

Go:   func main()
来源：http://dfw.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zxu.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://jsv.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://eje.cashguo.top

Py:   platform.system();  platform.python_version()
来源：http://auc.xuetiantiany.cn

PHP:  PHP_OS;  phpversion();
来源：http://nwt.sysykeji.top

JS:   process.platform;  process.version
来源：http://roi.jianghu66.top

TS:   process.platform;  process.version
来源：http://ypv.fanxiaobao.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://brx.smart0.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://wzy.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://moe.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://sdy.guowangkeji.top

================================================================================
来源：http://cre.xingfuxueyuan.xyz

N. 数据结构与算法
来源：http://rjn.xingfuxueyuan.xyz

================================================================================
来源：http://mgx.yj20258888.top

[N01] 二分查找（有序数组）
来源：http://ehn.ppjwa.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hvl.redwolf501.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yid.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xod.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ssy.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://cfm.zhixingplan.top

Go:   sort.SearchInts(arr, x)
来源：http://fnw.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dmd.haohaochexian.top

C#:   Array.BinarySearch(arr, x)
来源：http://kjm.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://uws.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://fuo.xylfe.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eop.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xis.52xcode.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lqy.jianghu66.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fym.hywenlv.cn

Go:   slices.Sort(arr)
来源：http://kjq.shuidangran.top

Ruby: arr.sort
来源：http://rvv.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jve.pycfn.com

[N03] 快速排序（分治示例）
来源：http://pen.uphjek.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wfq.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://cxm.ppjwa.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nta.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jvj.jyoumei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vld.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hsc.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eqd.hnqzz.top

C#:   // 手写递归，或 Array.Sort
来源：http://tow.pycfn.com

[N04] 斐波那契数列
来源：http://gel.epnwcf.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mca.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mmx.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://etw.jqgfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rjy.daxiang520.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bba.xuetiantiany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://stz.zhaomingkeji.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dip.snrcjt.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tth.hnqzz.top

[N05] 最大公约数
来源：http://pwt.bbcook.cn

Py:   math.gcd(a, b)
来源：http://lnh.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jek.hfpthk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rao.zdqjudy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sca.tarul.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tlg.nanxinkj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zdi.52xcode.cn

Ruby: a.gcd(b)
来源：http://eja.zhixingplan.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bwc.ydzc1.top

[N06] 判断回文字符串
来源：http://bvt.hnqzz.top

Py:   s == s[::-1]
来源：http://ahk.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://jfz.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://zms.hcnkem.com

TS:   s === [...s].reverse().join("")
来源：http://ebp.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bum.0kj1m.cn

Go:   // 双指针从两端比较
来源：http://eum.zhengqikj.top

Ruby: s == s.reverse
来源：http://rxc.zhengqikj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tno.tian-w.cn

[N07] 两数之和（返回下标）
来源：http://dyh.zhijiandao.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dzv.9152youxi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rqe.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bzs.ppjwa.cn

TS:   // 手写 Map<string, number>
来源：http://fpx.yanxiufei.cn

Java: // 手写 HashMap
来源：http://ytv.shzxlz.cn

Go:   // 手写 map[int]int
来源：http://iik.xziqi.cn

Ruby: // 手写 Hash
来源：http://fog.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://chx.yuxming.cn

[N08] 生成全排列
来源：http://fjx.yangfankeji.com

Py:   itertools.permutations(arr)
来源：http://kja.shanyushiyangtech.top

PHP:  // 手写递归交换
来源：http://dzx.hfpthk.cn

JS:   // 手写回溯递归
来源：http://nyw.zhiwuduotai.top

TS:   // 手写回溯递归
来源：http://jiv.jlsjyb.cn

Java: // 手写回溯递归
来源：http://oup.chenzaomai.com

Go:   // 手写回溯递归
来源：http://gkz.hywenlv.cn

Ruby: arr.permutation.to_a
来源：http://lzo.gotoacloud.top

C#:   // 手写回溯递归
来源：http://cff.gogol.net.cn

[N09] 栈与队列
来源：http://jim.xziqi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rpv.cdnleiting.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hts.iojbl.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://voq.fzhhl.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zkw.meibo888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zek.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qdg.xinyue.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jhs.shuidangran.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gyp.ivvv.top

[N10] 链表节点定义
来源：http://vvi.ppjwa.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://phf.cheryme.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mhw.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gjg.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wmd.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://dja.yangfankeji.com

Go:   type Node struct { V int; Next *Node }
来源：http://zcs.yonumen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ptt.shangyingyoupin.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jtw.tianlin.xyz

[N11] 二叉树中序遍历
来源：http://jmj.ppjwa.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bjl.mhx1999.top

PHP:  // 手写递归函数
来源：http://sjb.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lmr.yvedp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yjo.hnxiangtu.top

Java: // 手写递归
来源：http://cfo.epnwcf.com

Go:   // 手写递归
来源：http://psk.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yce.kuanghao11.cn

C#:   // 手写递归
来源：http://mpy.cqqwz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bks.meibo888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jbf.cqqwz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wzj.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://orr.zhixingplan.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uxs.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ayn.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kqg.jinghuilouyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ibq.sysykeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://huf.yueranfly.top

================================================================================
来源：http://rzl.jqgfzy.top

O. 并发与异步
来源：http://yoc.dashuyun.cn

================================================================================
来源：http://bwc.zhengqikj.top

[O01] 启动一个线程
来源：http://xdl.mhx1999.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hvo.daxiang520.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lgz.jqgufenzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eyd.andypj.xyz

TS:   // 同 JS
来源：http://ozn.yj20258.top

Java: new Thread(() -> f()).start()
来源：http://tga.tianlin.xyz

Go:   go f()
来源：http://yxh.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://gam.xylfe.cn

C#:   Task.Run(() => F());
来源：http://etf.jlsjyb.cn

[O02] 使用线程池
来源：http://tif.fehbvm.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://upq.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://alf.gzhubu.top

JS:   // worker_threads 线程池
来源：http://rzv.tianlin.xyz

TS:   // worker_threads 线程池
来源：http://ohq.zhengqikj.top

Java: Executors.newFixedThreadPool(4)
来源：http://owr.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nov.jyoumei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zfd.cheryme.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lpd.jqgufenzy.top

[O03] 加锁保护共享数据
来源：http://tak.zycfv.cn

Py:   with lock: shared += 1
来源：http://ndw.chenlongwang.top

PHP:  // 用 flock() 做文件锁
来源：http://aar.mhx1999.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ino.mhx1999.top

TS:   // 同 JS
来源：http://lyd.nanxinkj.top

Java: synchronized (this) { shared++; }
来源：http://xob.zhaomingkeji.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aod.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://umd.nwbrower.top

C#:   lock (gate) { shared++; }
来源：http://wad.jqgfzy.top

[O04] 定义异步函数并等待
来源：http://udq.0kj1m.cn

Py:   async def f():⏎    await g()
来源：http://idv.bbcook.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nwv.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://idu.dianchejie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://grc.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lal.quarkkingdee.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mwc.316326.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://bqz.yuanzhike.top

C#:   async Task F() { await G(); }
来源：http://mmf.0kj1m.cn

[O05] 并发执行并等待全部完成
来源：http://qoh.kuanghao11.cn

Py:   asyncio.gather(*tasks)
来源：http://gqe.hysaishi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://shg.nwbrower.top

JS:   await Promise.all(tasks)
来源：http://oyc.chenjidiqi.icu

TS:   await Promise.all(tasks)
来源：http://tho.xuetiantiany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dby.nwbrower.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://puy.yonumen.top

Ruby: threads.map(&:join)
来源：http://dfz.nanxuanxn.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lxb.fehbvm.com

[O06] 使用进程池
来源：http://zsm.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fma.zycfv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qvu.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://eco.birdmap.top

TS:   // child_process / cluster 模块
来源：http://tkk.fengsongda.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bqi.guannengcc.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ykm.sysykeji.top

Ruby: // fork 块
来源：http://fby.jyoumei.cn

C#:   Parallel.For
来源：http://qtm.hammf.cn

================================================================================
来源：http://mse.cqqwz.cn

P. 常用工具函数
来源：http://qjf.zhiwuduotai.top

================================================================================
来源：http://nsq.zdqjudy.top

[P01] 生成 UUID
来源：http://rei.jiagoushi.top

Py:   str(uuid.uuid4())
来源：http://ble.nwbrower.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://weo.yj20258.top

JS:   crypto.randomUUID()
来源：http://rwr.gzhubu.top

TS:   crypto.randomUUID()
来源：http://lql.bjfxy.top

Java: UUID.randomUUID().toString()
来源：http://dfn.zhiwuduotai.top

Go:   // 用 github.com/google/uuid
来源：http://pth.smart0.xyz

Ruby: SecureRandom.uuid
来源：http://too.snrcjt.cn

C#:   Guid.NewGuid().ToString()
来源：http://nxh.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://ipf.jlsjyb.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ljx.chenlongwang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://del.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wif.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fbu.jinqigfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aku.yuanzhike.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wwb.yj202588.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fgf.yangfankeji.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ygr.cashguo.top

[P03] 生成短随机字符串
来源：http://hsi.bjfxy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hck.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://znj.guannengcc.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qwx.redwolf501.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://svj.jqgufenzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qzl.zdqjudy.top


<!-- 参考信息 -->