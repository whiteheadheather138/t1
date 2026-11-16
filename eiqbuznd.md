代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ptt.shanyushiyangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://asl.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jtu.jyoumei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://txk.zhengqikj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vkz.hysaishi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qok.guowangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hbg.jinghuilouyu.cn

[L06] 解析响应为 JSON
来源：http://zly.tarul.cn

Py:   resp.json()
来源：http://ckt.smart0.xyz

PHP:  json_decode($body, true);
来源：http://qwl.zhijiandao.cn

JS:   await resp.json()
来源：http://clg.ydjk.org.cn

TS:   await resp.json()
来源：http://ken.nwbrower.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fkh.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gvx.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://hgn.xinyue.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://adu.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://dbn.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gwk.jinghuilouyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kye.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://syx.ydzc1.top

TS:   resp.ok;  resp.status
来源：http://idf.fengsongda.top

Java: resp.statusCode()
来源：http://fgt.yuanzhike.top

Go:   resp.StatusCode
来源：http://zik.zhaomingkeji.xyz

Ruby: resp.code.to_i
来源：http://boi.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://bnz.hesvh.cn

[L08] 并发请求多个地址
来源：http://qcg.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rpg.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://wuo.zhaomingkeji.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sor.sysykeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ulr.hysaishi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dof.aibaodan.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wqx.ehwqpu.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uju.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://khs.iojbl.cn

================================================================================
来源：http://grt.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://zde.jinqigufen.top

================================================================================
来源：http://yvp.yanxiufei.cn

[M01] 读取命令行参数
来源：http://bvx.daria6918.cn

Py:   sys.argv[1:]
来源：http://fbv.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://xpv.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://eho.sysykeji.top

TS:   process.argv.slice(2)
来源：http://wvs.shangyingyoupin.top

Java: args 数组（main 方法参数）
来源：http://mno.nwbrower.top

Go:   os.Args[1:]
来源：http://qml.yuxming.cn

Ruby: ARGV
来源：http://dqy.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://djm.aizwys.cn

[M02] 读取环境变量
来源：http://lez.yj20258888.top

Py:   os.environ.get("HOME")
来源：http://osm.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nuz.xinyue.icu

JS:   process.env.HOME
来源：http://zoh.jiagoushi.top

TS:   process.env.HOME
来源：http://haw.xylfe.cn

Java: System.getenv("HOME")
来源：http://cao.fktsv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lea.fehbvm.com

Ruby: ENV["HOME"]
来源：http://obp.ydjk.org.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qzs.nwbrower.top

[M03] 执行外部命令
来源：http://zis.zhoulong.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pze.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vis.ehwqpu.com

JS:   child_process.execSync("ls -l").toString()
来源：http://ism.hnxiangtu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bzl.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jfm.epnwcf.com

Go:   exec.Command("ls", "-l").Output()
来源：http://oai.gaohongyu789.top

Ruby: system("ls -l");  `ls -l`
来源：http://zfz.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://alf.xziqi.cn

[M04] 获取当前工作目录
来源：http://yln.snrcjt.cn

Py:   os.getcwd()
来源：http://ksd.sufxvd.cn

PHP:  getcwd();
来源：http://wvg.fzhhl.top

JS:   process.cwd()
来源：http://rwz.feifeiyinyue.top

TS:   process.cwd()
来源：http://rof.zhengqikj.top

Java: Path.of("").toAbsolutePath()
来源：http://esu.jiagoushi.top

Go:   os.Getwd()
来源：http://apf.xylfe.cn

Ruby: Dir.pwd
来源：http://hjr.quarkkingdee.top

C#:   Directory.GetCurrentDirectory()
来源：http://khg.cucudq.cn

[M05] 设置退出码
来源：http://jtg.meibo888.top

Py:   sys.exit(1)
来源：http://lsk.sweek.top

PHP:  exit(1);
来源：http://ttw.pengpengdd.cyou

JS:   process.exit(1)
来源：http://ccr.hesvh.cn

TS:   process.exit(1)
来源：http://wwx.hcnkem.com

Java: System.exit(1)
来源：http://cxr.jqgfzy.top

Go:   os.Exit(1)
来源：http://jtq.jqgufenzy.top

Ruby: exit 1
来源：http://iex.yangfankeji.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ggz.xingfuxueyuan.xyz

[M06] 向标准错误输出
来源：http://ywk.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://rwa.316326.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://gya.yuxming.cn

JS:   console.error("err")
来源：http://vuw.shuidangran.top

TS:   console.error("err")
来源：http://bfb.meibo888.top

Java: System.err.println("err")
来源：http://dyg.ywan-chungtsiang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yth.hfpthk.cn

Ruby: warn "err"
来源：http://oyn.jinyuanbaomall.cn

C#:   Console.Error.WriteLine("err")
来源：http://xoz.sweek.top

[M07] 判断是否为主入口
来源：http://ixx.jqgufenzy.top

Py:   if __name__ == "__main__":
来源：http://dwd.ehwqpu.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qpn.gzhubu.top

JS:   require.main === module
来源：http://dvc.ywan-chungtsiang.top

TS:   require.main === module
来源：http://aha.yongpay.top

Java: public static void main(String[] args)
来源：http://pts.iojbl.cn

Go:   func main()
来源：http://tbr.ehwqpu.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://quz.yonumen.top

C#:   static void Main(string[] args)
来源：http://hdq.xylfe.cn

[M08] 获取系统与运行时信息
来源：http://wzv.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://ytr.zhoulong.xyz

PHP:  PHP_OS;  phpversion();
来源：http://fyz.jyoumei.cn

JS:   process.platform;  process.version
来源：http://owc.sufxvd.cn

TS:   process.platform;  process.version
来源：http://opq.epnwcf.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xzc.yj202588.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fqh.kuanghao11.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zbb.gaohongyu789.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kgq.bjfxy.top

================================================================================
来源：http://gme.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://hph.chenzaomai.com

================================================================================
来源：http://zfz.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://zgh.yj20258888.top

Py:   bisect.bisect_left(arr, x)
来源：http://xaf.shuidangran.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tut.yj20258888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zsb.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yec.yuxming.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zoh.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://dqa.jqgufenzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ifw.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://nxs.aizwys.cn

[N02] 排序（工程实践用内置实现）
来源：http://cib.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://ugp.sjlbkw.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ixu.cqqwz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qiy.hongshengwenyu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vrw.shuidangran.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bto.yanxiufei.cn

Go:   slices.Sort(arr)
来源：http://tax.9152youxi.cn

Ruby: arr.sort
来源：http://crr.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://apf.sweek.top

[N03] 快速排序（分治示例）
来源：http://anb.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uue.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://fud.zdqjudy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fua.mhx1999.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mhk.hcnkem.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ihn.smart0.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blg.zdqjudy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tpe.pycfn.com

C#:   // 手写递归，或 Array.Sort
来源：http://ymp.cheryme.top

[N04] 斐波那契数列
来源：http://oef.havefunace.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uac.jqgufenzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aso.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wbw.zhaomingkeji.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jmh.ywan-chungtsiang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mzj.zhiwuduotai.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yxx.0kj1m.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xrx.bbcook.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vad.zhoulong.xyz

[N05] 最大公约数
来源：http://bhk.cqqwz.cn

Py:   math.gcd(a, b)
来源：http://qgn.wangdashe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uko.iojbl.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qaf.dianchejie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://saz.jianghu66.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bpy.daxiang520.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://flw.chenzaomai.com

Ruby: a.gcd(b)
来源：http://cyf.cqqwz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xpl.guannengcc.top

[N06] 判断回文字符串
来源：http://sbz.tarul.cn

Py:   s == s[::-1]
来源：http://rkf.uphjek.com

PHP:  $s === strrev($s);
来源：http://ovq.xingfuxueyuan.xyz

JS:   s === [...s].reverse().join("")
来源：http://acg.hcnkem.com

TS:   s === [...s].reverse().join("")
来源：http://lyq.hysaishi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://upy.cashguo.top

Go:   // 双指针从两端比较
来源：http://tts.xinyue.icu

Ruby: s == s.reverse
来源：http://cqi.epnwcf.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://xqv.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://iax.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fbm.tanke756.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hmt.zdbjq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yre.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://mwk.jianghu66.top

Java: // 手写 HashMap
来源：http://rzz.yongpay.top

Go:   // 手写 map[int]int
来源：http://lvq.hfpthk.cn

Ruby: // 手写 Hash
来源：http://vyp.nanxuanxn.top

C#:   // 手写 Dictionary<int, int>
来源：http://tsm.cqqwz.cn

[N08] 生成全排列
来源：http://ngn.jinqigfzy.top

Py:   itertools.permutations(arr)
来源：http://azp.hcnkem.com

PHP:  // 手写递归交换
来源：http://ylh.hammf.cn

JS:   // 手写回溯递归
来源：http://cxk.gogol.net.cn

TS:   // 手写回溯递归
来源：http://qva.jyoumei.cn

Java: // 手写回溯递归
来源：http://mjh.hfpthk.cn

Go:   // 手写回溯递归
来源：http://dby.zycfv.cn

Ruby: arr.permutation.to_a
来源：http://xtp.daria6918.cn

C#:   // 手写回溯递归
来源：http://vvx.yj20258888.top

[N09] 栈与队列
来源：http://jrh.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ppy.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://aez.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jcf.cqqwz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rzx.chenzaomai.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jxh.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oxo.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zmo.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rhg.fzhhl.top

[N10] 链表节点定义
来源：http://xlq.aibaodan.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ycl.yj202588.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cyp.yueranfly.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://glv.hesvh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://enx.pycfn.com

Java: class Node { int v; Node next; }
来源：http://gsa.yonumen.top

Go:   type Node struct { V int; Next *Node }
来源：http://pxv.ehwqpu.com

Ruby: Node = Struct.new(:v, :next)
来源：http://rxf.nanxuanxn.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jnc.xziqi.cn

[N11] 二叉树中序遍历
来源：http://vmr.zhixingplan.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mdu.smart0.xyz

PHP:  // 手写递归函数
来源：http://tmw.daxiang520.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aum.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kbb.wangdashe.top

Java: // 手写递归
来源：http://rlc.zdbjq.cn

Go:   // 手写递归
来源：http://bjg.zhiwuduotai.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xez.52xcode.cn

C#:   // 手写递归
来源：http://ywi.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uxy.nanxinkj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dxh.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wwr.yongpay.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://djw.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ylp.sufxvd.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hip.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xtu.316326.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://psh.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lnv.zdbjq.cn

================================================================================
来源：http://iht.ydjk.org.cn

O. 并发与异步
来源：http://nao.sjlbkw.cn

================================================================================
来源：http://wkj.jinqigfzy.top

[O01] 启动一个线程
来源：http://klp.yvedp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://got.guowangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rxl.sxryk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xos.9152youxi.cn

TS:   // 同 JS
来源：http://rax.tarul.cn

Java: new Thread(() -> f()).start()
来源：http://dwh.pycfn.com

Go:   go f()
来源：http://lqa.feifeiyinyue.top

Ruby: Thread.new { f }
来源：http://rjf.zhixingplan.top

C#:   Task.Run(() => F());
来源：http://lxb.9152youxi.cn

[O02] 使用线程池
来源：http://yft.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jxk.cqqwz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vvw.fktsv.cn

JS:   // worker_threads 线程池
来源：http://gbt.shzxlz.cn

TS:   // worker_threads 线程池
来源：http://bgd.gaohongyu789.top

Java: Executors.newFixedThreadPool(4)
来源：http://spx.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://unq.yongpay.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cng.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yar.ppjwa.cn

[O03] 加锁保护共享数据
来源：http://cdh.xingfuxueyuan.xyz

Py:   with lock: shared += 1
来源：http://zlk.yj20258888.top

PHP:  // 用 flock() 做文件锁
来源：http://vdm.vqdsnc.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://udc.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://uid.hnxiangtu.top

Java: synchronized (this) { shared++; }
来源：http://czc.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://scq.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://azk.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://kmh.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://jsx.tianlin.xyz

Py:   async def f():⏎    await g()
来源：http://xfi.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mee.dianchejie.cn

JS:   async function f() { await g(); }
来源：http://heq.zhijiandao.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://itu.fktsv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wbn.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wwk.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://bte.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://zlo.cheryme.top

[O05] 并发执行并等待全部完成
来源：http://zsa.shanyushiyangtech.top

Py:   asyncio.gather(*tasks)
来源：http://fbt.cheryme.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ajm.pengpengdd.cyou

JS:   await Promise.all(tasks)
来源：http://xde.meibo888.top

TS:   await Promise.all(tasks)
来源：http://myv.hesvh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bxz.dianchejie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eex.zhixingplan.top

Ruby: threads.map(&:join)
来源：http://vlm.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lsm.jianghu66.top

[O06] 使用进程池
来源：http://jru.fanxiaobao.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wvj.chenjidiqi.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://dgw.sysykeji.top

JS:   // child_process / cluster 模块
来源：http://jpe.zhoulong.xyz

TS:   // child_process / cluster 模块
来源：http://fcj.xylfe.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wio.chenjidiqi.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mft.gogol.net.cn

Ruby: // fork 块
来源：http://azq.shanyushiyangkeji.top

C#:   Parallel.For
来源：http://dnp.guannengcc.top

================================================================================
来源：http://jhu.jianghu66.top

P. 常用工具函数
来源：http://fpu.nanxinkj.top

================================================================================
来源：http://ezp.shanyushiyangtech.top

[P01] 生成 UUID
来源：http://nog.fktsv.cn

Py:   str(uuid.uuid4())
来源：http://ihp.daria6918.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://epd.cheryme.top

JS:   crypto.randomUUID()
来源：http://zif.cashguo.top

TS:   crypto.randomUUID()
来源：http://wlj.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://qiz.shangyingyoupin.top

Go:   // 用 github.com/google/uuid
来源：http://nbc.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://coh.cdnleiting.top

C#:   Guid.NewGuid().ToString()
来源：http://osw.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://vli.xziqi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ouh.9152youxi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uni.xziqi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://neb.jinyuanbaomall.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yfo.birdmap.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ahs.zhixingplan.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hka.nanxuanxn.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lyu.hesvh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jje.sufxvd.cn

[P03] 生成短随机字符串
来源：http://enx.zhongyouzk.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ddj.shangyingyoupin.top


<!-- 参考信息 -->