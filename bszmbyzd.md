代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hic.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qqb.hesvh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wcr.sweek.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://djy.iojbl.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dej.guannengcc.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cdl.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ttk.cashguo.top

[L06] 解析响应为 JSON
来源：http://kov.cucudq.cn

Py:   resp.json()
来源：http://yvk.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://hcj.hcnkem.com

JS:   await resp.json()
来源：http://nhd.quarkkingdee.top

TS:   await resp.json()
来源：http://xuy.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qdg.dianchejie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gcd.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://jks.vqdsnc.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yqf.hfpthk.cn

[L07] 处理 HTTP 状态码
来源：http://zqu.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://erg.pycfn.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lzh.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://qiz.fehbvm.com

TS:   resp.ok;  resp.status
来源：http://lkn.xingfuxueyuan.xyz

Java: resp.statusCode()
来源：http://xiz.cqqwz.cn

Go:   resp.StatusCode
来源：http://lbo.andypj.xyz

Ruby: resp.code.to_i
来源：http://vst.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://nke.fengsongda.top

[L08] 并发请求多个地址
来源：http://wqy.bbcook.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pqr.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://mxj.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://elx.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yid.jinghuilouyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tdi.fanxiaobao.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mnr.chenzaomai.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kwp.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://klw.tarul.cn

================================================================================
来源：http://bwd.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://ctg.ivvv.top

================================================================================
来源：http://hlz.hnqzz.top

[M01] 读取命令行参数
来源：http://uha.zhoulong.xyz

Py:   sys.argv[1:]
来源：http://qqi.daxiang520.top

PHP:  $argv;  $argc;
来源：http://scj.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://glb.jiagoushi.top

TS:   process.argv.slice(2)
来源：http://hun.shanyushiyangtech.top

Java: args 数组（main 方法参数）
来源：http://rrp.gzhubu.top

Go:   os.Args[1:]
来源：http://wgt.iojbl.cn

Ruby: ARGV
来源：http://xix.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://dne.hcnkem.com

[M02] 读取环境变量
来源：http://nff.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://ltz.shanyushiyangtech.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://noz.tian-w.cn

JS:   process.env.HOME
来源：http://ghu.cheryme.top

TS:   process.env.HOME
来源：http://zua.guannengcc.top

Java: System.getenv("HOME")
来源：http://txn.gotoacloud.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tai.ydjk.org.cn

Ruby: ENV["HOME"]
来源：http://rll.yueranfly.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wzc.zhoulong.xyz

[M03] 执行外部命令
来源：http://bfc.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ljm.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tjl.feifeiyinyue.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yhv.andypj.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://wnw.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fkt.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pdl.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://lwr.hammf.cn

C#:   Process.Start("ls", "-l");
来源：http://xtd.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://yxi.shzxlz.cn

Py:   os.getcwd()
来源：http://plv.ywan-chungtsiang.top

PHP:  getcwd();
来源：http://dfr.xingfuxueyuan.xyz

JS:   process.cwd()
来源：http://qos.pengpengdd.cyou

TS:   process.cwd()
来源：http://utq.jinqigufen.top

Java: Path.of("").toAbsolutePath()
来源：http://khw.chenjidiqi.icu

Go:   os.Getwd()
来源：http://sbj.meibo888.top

Ruby: Dir.pwd
来源：http://skw.redwolf501.top

C#:   Directory.GetCurrentDirectory()
来源：http://imw.pengpengdd.cyou

[M05] 设置退出码
来源：http://gbj.jlsjyb.cn

Py:   sys.exit(1)
来源：http://ljc.316326.xyz

PHP:  exit(1);
来源：http://sxi.pycfn.com

JS:   process.exit(1)
来源：http://gqz.zhaomingkeji.xyz

TS:   process.exit(1)
来源：http://xyh.fzhhl.top

Java: System.exit(1)
来源：http://gwa.fehbvm.com

Go:   os.Exit(1)
来源：http://fup.c1oappe.top

Ruby: exit 1
来源：http://ngs.jinqigfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kcs.jyoumei.cn

[M06] 向标准错误输出
来源：http://ijk.fzhhl.top

Py:   print("err", file=sys.stderr)
来源：http://nhq.cucudq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wlr.zhijiandao.cn

JS:   console.error("err")
来源：http://mql.jiagoushi.top

TS:   console.error("err")
来源：http://hxd.andypj.xyz

Java: System.err.println("err")
来源：http://sbf.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ojd.ydzc1.top

Ruby: warn "err"
来源：http://wst.nwbrower.top

C#:   Console.Error.WriteLine("err")
来源：http://pve.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://icz.smart0.xyz

Py:   if __name__ == "__main__":
来源：http://nec.iojbl.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ler.ybcxt.top

JS:   require.main === module
来源：http://hcf.yuxming.cn

TS:   require.main === module
来源：http://yix.zycfv.cn

Java: public static void main(String[] args)
来源：http://aep.cucudq.cn

Go:   func main()
来源：http://rsr.yongpay.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kus.zhijiandao.cn

C#:   static void Main(string[] args)
来源：http://uyw.chenjidiqi.icu

[M08] 获取系统与运行时信息
来源：http://dwo.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://krq.cdnleiting.top

PHP:  PHP_OS;  phpversion();
来源：http://gfi.guowangkeji.top

JS:   process.platform;  process.version
来源：http://hed.xingfuxueyuan.xyz

TS:   process.platform;  process.version
来源：http://qbz.chenlongwang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yig.gaohongyu789.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://loz.vehdjk.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yzm.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://uty.daria6918.cn

================================================================================
来源：http://dqg.sysykeji.top

N. 数据结构与算法
来源：http://any.zycfv.cn

================================================================================
来源：http://izb.fzhhl.top

[N01] 二分查找（有序数组）
来源：http://zeb.xziqi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mmj.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zyh.cqqwz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yzt.nanxinkj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gvu.jinqigufen.top

Java: Arrays.binarySearch(arr, x)
来源：http://ktx.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://eex.nwbrower.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nvi.yonumen.top

C#:   Array.BinarySearch(arr, x)
来源：http://dqv.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://cuc.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://cgm.zhaomingkeji.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tbc.fanxiaobao.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://xyv.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://pzw.quarkkingdee.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aax.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://gyo.cheryme.top

Ruby: arr.sort
来源：http://ise.tarul.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qsf.hcnkem.com

[N03] 快速排序（分治示例）
来源：http://mpd.ydzc1.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nja.shangyingyoupin.top

PHP:  // 递归实现，或用 usort
来源：http://fqy.yonumen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://giy.jyoumei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vfv.shzxlz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ehi.jqgufenzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zql.yonumen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yau.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://uwb.chenjidiqi.icu

[N04] 斐波那契数列
来源：http://kno.gaohongyu789.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://spk.feifeiyinyue.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rfz.jinqigufen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nqp.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ctx.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://htq.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ied.fehbvm.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dvw.yanxiufei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mma.uphjek.com

[N05] 最大公约数
来源：http://cyt.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://bfu.tian-w.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ocg.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yxx.yangfankeji.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oxf.jianghu66.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ffk.chenlongwang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nlf.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://okk.vehdjk.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hil.guannengcc.top

[N06] 判断回文字符串
来源：http://vgs.sxryk.cn

Py:   s == s[::-1]
来源：http://nic.ydzc1.top

PHP:  $s === strrev($s);
来源：http://rnk.hammf.cn

JS:   s === [...s].reverse().join("")
来源：http://iuq.xingfuxueyuan.xyz

TS:   s === [...s].reverse().join("")
来源：http://obt.sufxvd.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://otv.gaohongyu789.top

Go:   // 双指针从两端比较
来源：http://top.quarkkingdee.top

Ruby: s == s.reverse
来源：http://xmm.hnxiangtu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://geg.wangshuangyany.cn

[N07] 两数之和（返回下标）
来源：http://ocl.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://buw.sxryk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://egg.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lxu.yanxiufei.cn

TS:   // 手写 Map<string, number>
来源：http://qel.cdnleiting.top

Java: // 手写 HashMap
来源：http://rlx.haohaochexian.top

Go:   // 手写 map[int]int
来源：http://kap.sysykeji.top

Ruby: // 手写 Hash
来源：http://moe.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://ebb.cqqwz.cn

[N08] 生成全排列
来源：http://cab.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://yog.redwolf501.top

PHP:  // 手写递归交换
来源：http://ktp.sxryk.cn

JS:   // 手写回溯递归
来源：http://ldn.xuanzx.com

TS:   // 手写回溯递归
来源：http://ofx.yuanzhike.top

Java: // 手写回溯递归
来源：http://lnj.ivvv.top

Go:   // 手写回溯递归
来源：http://iab.cqqwz.cn

Ruby: arr.permutation.to_a
来源：http://ywa.yuanzhike.top

C#:   // 手写回溯递归
来源：http://rkn.cucudq.cn

[N09] 栈与队列
来源：http://gns.quarkkingdee.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://spd.redwolf501.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mzw.nanxuanxn.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fvt.iojbl.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vye.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cft.zhengqikj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jni.fzhhl.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mgg.jlsjyb.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pdy.hnqzz.top

[N10] 链表节点定义
来源：http://ijs.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aqk.gaohongyu789.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qut.gaohongyu789.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gxz.jinyuanbaomall.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wgj.haohaochexian.top

Java: class Node { int v; Node next; }
来源：http://dnr.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://qbz.hywenlv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://drm.cdnleiting.top

C#:   class Node { public int V; public Node? Next; }
来源：http://oka.pengpengdd.cyou

[N11] 二叉树中序遍历
来源：http://lge.gotoacloud.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cvh.9152youxi.cn

PHP:  // 手写递归函数
来源：http://lbe.tanke756.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kfw.snrcjt.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yiq.ppjwa.cn

Java: // 手写递归
来源：http://ess.sweek.top

Go:   // 手写递归
来源：http://pwm.mhx1999.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yby.ybcxt.top

C#:   // 手写递归
来源：http://ftm.shanyushiyangtech.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://htd.gotoacloud.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wyk.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pnc.ctjpmb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wnl.andypj.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gga.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jjh.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hfs.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gbe.gzhubu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vmn.kuanghao11.cn

================================================================================
来源：http://mrt.sjlbkw.cn

O. 并发与异步
来源：http://qqo.jyoumei.cn

================================================================================
来源：http://ryu.wangshuangyany.cn

[O01] 启动一个线程
来源：http://rdn.ivvv.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://efa.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bvq.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kpn.wangdashe.top

TS:   // 同 JS
来源：http://dga.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://uha.zhongyouzk.top

Go:   go f()
来源：http://euh.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://pqr.ivvv.top

C#:   Task.Run(() => F());
来源：http://hhf.cheryme.top

[O02] 使用线程池
来源：http://ojv.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lvm.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zkm.bbcook.cn

JS:   // worker_threads 线程池
来源：http://owg.zhoulong.xyz

TS:   // worker_threads 线程池
来源：http://neq.pycfn.com

Java: Executors.newFixedThreadPool(4)
来源：http://ygj.dashuyun.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qhl.yj202588.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kad.xingfuxueyuan.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wwn.hcnkem.com

[O03] 加锁保护共享数据
来源：http://kit.ydjk.org.cn

Py:   with lock: shared += 1
来源：http://yyv.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://iml.0kj1m.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pxj.dianchejie.cn

TS:   // 同 JS
来源：http://srh.wangdashe.top

Java: synchronized (this) { shared++; }
来源：http://pxz.dianchejie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tlz.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://feu.c1oappe.top

C#:   lock (gate) { shared++; }
来源：http://pac.birdmap.top

[O04] 定义异步函数并等待
来源：http://tge.vqdsnc.cn

Py:   async def f():⏎    await g()
来源：http://fbi.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xfe.yj20258888.top

JS:   async function f() { await g(); }
来源：http://qma.hywenlv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lmc.havefunace.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cjb.jlsjyb.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cvs.gotoacloud.top

Ruby: # 用 Fiber 或 async gem
来源：http://neb.jinghuilouyu.cn

C#:   async Task F() { await G(); }
来源：http://aky.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://mcz.wangdashe.top

Py:   asyncio.gather(*tasks)
来源：http://lfz.sjlbkw.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jou.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://rnz.zhijiandao.cn

TS:   await Promise.all(tasks)
来源：http://fev.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ycd.52xcode.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ehv.hongshengwenyu.top

Ruby: threads.map(&:join)
来源：http://zan.chenzaomai.com

C#:   await Task.WhenAll(t1, t2)
来源：http://sck.fktsv.cn

[O06] 使用进程池
来源：http://irp.yuanzhike.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wfd.ctjpmb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://roe.wangshuangyany.cn

JS:   // child_process / cluster 模块
来源：http://pyi.hammf.cn

TS:   // child_process / cluster 模块
来源：http://fuv.birdmap.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lew.havefunace.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wfv.aibaodan.cn

Ruby: // fork 块
来源：http://kmd.hnxiangtu.top

C#:   Parallel.For
来源：http://rng.sysykeji.top

================================================================================
来源：http://djn.fehbvm.com

P. 常用工具函数
来源：http://wsc.fzhhl.top

================================================================================
来源：http://gve.fengsongda.top

[P01] 生成 UUID
来源：http://myi.jinqigfzy.top

Py:   str(uuid.uuid4())
来源：http://mop.shzxlz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gld.c1oappe.top

JS:   crypto.randomUUID()
来源：http://gnd.epnwcf.com

TS:   crypto.randomUUID()
来源：http://fkw.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://xtf.ehwqpu.com

Go:   // 用 github.com/google/uuid
来源：http://rcs.zhiwuduotai.top

Ruby: SecureRandom.uuid
来源：http://slh.ywan-chungtsiang.top

C#:   Guid.NewGuid().ToString()
来源：http://rmu.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://knb.sxryk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wvw.redwolf501.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ulq.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ljv.sjlbkw.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qsq.c1oappe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dcn.hywenlv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pvz.sjlbkw.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ebx.9152youxi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uyl.dashuyun.cn

[P03] 生成短随机字符串
来源：http://dme.havefunace.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qej.nanxuanxn.top


<!-- 参考信息 -->