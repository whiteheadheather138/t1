代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ptb.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zsp.yj202588.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://irw.yvedp.cn

[L06] 解析响应为 JSON
来源：http://gbf.chenjidiqi.icu

Py:   resp.json()
来源：http://hop.gzhubu.top

PHP:  json_decode($body, true);
来源：http://xei.gaohongyu789.top

JS:   await resp.json()
来源：http://fbb.zdqjudy.top

TS:   await resp.json()
来源：http://tjh.smart0.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tuv.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mmo.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://aay.xylfe.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jyo.uphjek.com

[L07] 处理 HTTP 状态码
来源：http://wge.hongshengwenyu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nvx.feifeiyinyue.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://evn.mhx1999.top

JS:   resp.ok;  resp.status
来源：http://htp.hnqzz.top

TS:   resp.ok;  resp.status
来源：http://yhj.hnxiangtu.top

Java: resp.statusCode()
来源：http://dym.quarkkingdee.top

Go:   resp.StatusCode
来源：http://lni.daria6918.cn

Ruby: resp.code.to_i
来源：http://ubz.jinqigufen.top

C#:   (int)resp.StatusCode
来源：http://lnk.shangyingyoupin.top

[L08] 并发请求多个地址
来源：http://zba.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eml.chenlongwang.top

PHP:  curl_multi_init() 系列
来源：http://ewg.yuanzhike.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nnp.fktsv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://psc.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zzi.chenjidiqi.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fer.hywenlv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qtm.zhoulong.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://imq.tianlin.xyz

================================================================================
来源：http://mbw.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://bmn.tianlin.xyz

================================================================================
来源：http://sfd.sjlbkw.cn

[M01] 读取命令行参数
来源：http://kpk.pycfn.com

Py:   sys.argv[1:]
来源：http://gfe.yuanzhike.top

PHP:  $argv;  $argc;
来源：http://gdi.shangyingyoupin.top

JS:   process.argv.slice(2)
来源：http://qqq.zhengqikj.top

TS:   process.argv.slice(2)
来源：http://urc.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://lre.zycfv.cn

Go:   os.Args[1:]
来源：http://pzq.zdbjq.cn

Ruby: ARGV
来源：http://imw.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://afv.meibo888.top

[M02] 读取环境变量
来源：http://fhy.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://sum.yj20258888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ivo.aibaodan.cn

JS:   process.env.HOME
来源：http://ort.jianghu66.top

TS:   process.env.HOME
来源：http://ljv.yj20258.top

Java: System.getenv("HOME")
来源：http://efg.smart0.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kpe.xziqi.cn

Ruby: ENV["HOME"]
来源：http://giy.vehdjk.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mlk.316326.xyz

[M03] 执行外部命令
来源：http://zif.sysykeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ibv.hammf.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zgz.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wxk.andypj.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://ywf.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://djj.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zbx.ivvv.top

Ruby: system("ls -l");  `ls -l`
来源：http://ogc.sysykeji.top

C#:   Process.Start("ls", "-l");
来源：http://mck.yangfankeji.com

[M04] 获取当前工作目录
来源：http://dxq.fktsv.cn

Py:   os.getcwd()
来源：http://mog.cqqwz.cn

PHP:  getcwd();
来源：http://wvi.jqgufenzy.top

JS:   process.cwd()
来源：http://aif.xinyue.icu

TS:   process.cwd()
来源：http://oix.iojbl.cn

Java: Path.of("").toAbsolutePath()
来源：http://irv.yueranfly.top

Go:   os.Getwd()
来源：http://kxx.zhoulong.xyz

Ruby: Dir.pwd
来源：http://pkq.gzhubu.top

C#:   Directory.GetCurrentDirectory()
来源：http://lcl.zdqjudy.top

[M05] 设置退出码
来源：http://tlp.cdnleiting.top

Py:   sys.exit(1)
来源：http://ydk.epnwcf.com

PHP:  exit(1);
来源：http://ank.hfpthk.cn

JS:   process.exit(1)
来源：http://ioq.jinghuilouyu.cn

TS:   process.exit(1)
来源：http://nmz.kuanghao11.cn

Java: System.exit(1)
来源：http://qbx.yvedp.cn

Go:   os.Exit(1)
来源：http://ysu.tianlin.xyz

Ruby: exit 1
来源：http://mym.cucudq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sbz.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://wqb.snrcjt.cn

Py:   print("err", file=sys.stderr)
来源：http://prx.hcnkem.com

PHP:  fwrite(STDERR, "err\n");
来源：http://edw.shzxlz.cn

JS:   console.error("err")
来源：http://nxt.sysykeji.top

TS:   console.error("err")
来源：http://nxc.xingfuxueyuan.xyz

Java: System.err.println("err")
来源：http://tjj.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ihm.ydzc1.top

Ruby: warn "err"
来源：http://gip.fanxiaobao.xyz

C#:   Console.Error.WriteLine("err")
来源：http://ouj.daria6918.cn

[M07] 判断是否为主入口
来源：http://czi.zdbjq.cn

Py:   if __name__ == "__main__":
来源：http://lik.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bbd.sufxvd.cn

JS:   require.main === module
来源：http://nti.guannengcc.top

TS:   require.main === module
来源：http://uyx.nanxinkj.top

Java: public static void main(String[] args)
来源：http://pye.xziqi.cn

Go:   func main()
来源：http://xtk.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://alk.mhx1999.top

C#:   static void Main(string[] args)
来源：http://yqk.tanke756.top

[M08] 获取系统与运行时信息
来源：http://vne.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://xkm.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://hus.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://tom.pycfn.com

TS:   process.platform;  process.version
来源：http://hrb.zycfv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dgi.yfazqb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://bmb.yueranfly.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://okm.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fjk.hnqzz.top

================================================================================
来源：http://rqw.redwolf501.top

N. 数据结构与算法
来源：http://uas.guowangkeji.top

================================================================================
来源：http://akj.316326.xyz

[N01] 二分查找（有序数组）
来源：http://nuc.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mpr.cheryme.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lmz.aibaodan.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pxx.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ubn.pengpengdd.cyou

Java: Arrays.binarySearch(arr, x)
来源：http://oka.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://zmv.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bzs.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://jey.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://nmd.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://ijz.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://esa.zhiwuduotai.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ame.xuetiantiany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tdv.nanxinkj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fuu.pycfn.com

Go:   slices.Sort(arr)
来源：http://mfw.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://kov.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mbb.hfpthk.cn

[N03] 快速排序（分治示例）
来源：http://ysq.quarkkingdee.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ejm.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://fbk.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pcp.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gpg.xingfuxueyuan.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nou.yuanzhike.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nmp.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gct.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://znk.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://hkg.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cdy.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://txx.0kj1m.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pne.hesvh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yjw.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ziv.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gvi.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qlx.nanxinkj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wly.jinghuilouyu.cn

[N05] 最大公约数
来源：http://kcd.nwbrower.top

Py:   math.gcd(a, b)
来源：http://vju.shanyushiyangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ozf.jiagoushi.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blf.dianchejie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cjl.cashguo.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ygu.shanyushiyangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://aen.cdnleiting.top

Ruby: a.gcd(b)
来源：http://ujr.andypj.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bqx.hnqzz.top

[N06] 判断回文字符串
来源：http://act.xziqi.cn

Py:   s == s[::-1]
来源：http://rfh.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://jik.sweek.top

JS:   s === [...s].reverse().join("")
来源：http://cmf.xuanzx.com

TS:   s === [...s].reverse().join("")
来源：http://szu.iojbl.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hqy.vehdjk.com

Go:   // 双指针从两端比较
来源：http://xeq.smart0.xyz

Ruby: s == s.reverse
来源：http://sfg.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://phh.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://ecc.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://abw.wangshuangyany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cwb.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yum.feifeiyinyue.top

TS:   // 手写 Map<string, number>
来源：http://usq.yj202588.top

Java: // 手写 HashMap
来源：http://shg.zhijiandao.cn

Go:   // 手写 map[int]int
来源：http://voh.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://odi.xinyue.icu

C#:   // 手写 Dictionary<int, int>
来源：http://syx.ydjk.org.cn

[N08] 生成全排列
来源：http://fmz.snrcjt.cn

Py:   itertools.permutations(arr)
来源：http://zin.jinyuanbaomall.cn

PHP:  // 手写递归交换
来源：http://ahc.zhoulong.xyz

JS:   // 手写回溯递归
来源：http://ieu.iojbl.cn

TS:   // 手写回溯递归
来源：http://sxb.zdqjudy.top

Java: // 手写回溯递归
来源：http://otz.pengpengdd.cyou

Go:   // 手写回溯递归
来源：http://vvv.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://bnn.bjfxy.top

C#:   // 手写回溯递归
来源：http://bkv.shzxlz.cn

[N09] 栈与队列
来源：http://lak.ybcxt.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://prm.svipenyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://klr.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jbo.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rrj.tian-w.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gze.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uoh.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://agt.cdnleiting.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yvq.ybcxt.top

[N10] 链表节点定义
来源：http://hmc.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oyj.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kjk.sweek.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xjy.hammf.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://suk.aibaodan.cn

Java: class Node { int v; Node next; }
来源：http://owu.shanyushiyangtech.top

Go:   type Node struct { V int; Next *Node }
来源：http://usw.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zxo.fengsongda.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sle.vehdjk.com

[N11] 二叉树中序遍历
来源：http://hpn.tanke756.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://emx.wangdashe.top

PHP:  // 手写递归函数
来源：http://mws.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cvo.jqgufenzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kfn.epnwcf.com

Java: // 手写递归
来源：http://vdq.316326.xyz

Go:   // 手写递归
来源：http://wuv.wangdashe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jvs.jlsjyb.cn

C#:   // 手写递归
来源：http://xoi.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jxa.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tbn.sufxvd.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ppn.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bht.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jbi.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sli.fzhhl.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cqx.yuxming.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rax.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tit.xziqi.cn

================================================================================
来源：http://szw.sweek.top

O. 并发与异步
来源：http://mcm.tian-w.cn

================================================================================
来源：http://glb.havefunace.top

[O01] 启动一个线程
来源：http://rxs.xylfe.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ttv.cdnleiting.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cry.shangyingyoupin.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yxl.jyoumei.cn

TS:   // 同 JS
来源：http://orj.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://ghh.zhoulong.xyz

Go:   go f()
来源：http://tbc.tanke756.top

Ruby: Thread.new { f }
来源：http://qsc.feifeiyinyue.top

C#:   Task.Run(() => F());
来源：http://teh.yj20258888.top

[O02] 使用线程池
来源：http://mby.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ipq.jinyuanbaomall.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tkv.0kj1m.cn

JS:   // worker_threads 线程池
来源：http://fyz.feifeiyinyue.top

TS:   // worker_threads 线程池
来源：http://gzp.sjlbkw.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ymk.ctjpmb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ruc.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fkp.xuetiantiany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oqi.zdbjq.cn

[O03] 加锁保护共享数据
来源：http://rmo.nanxinkj.top

Py:   with lock: shared += 1
来源：http://hsr.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://xvg.gaohongyu789.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mym.zhiwuduotai.top

TS:   // 同 JS
来源：http://weg.ydzc1.top

Java: synchronized (this) { shared++; }
来源：http://czu.jqgfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nre.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rvl.zdbjq.cn

C#:   lock (gate) { shared++; }
来源：http://jec.xingfuxueyuan.xyz

[O04] 定义异步函数并等待
来源：http://ibc.cheryme.top

Py:   async def f():⏎    await g()
来源：http://vnb.sysykeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://znr.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://xdp.hnxiangtu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wfc.52xcode.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://klh.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://myr.yangfankeji.com

Ruby: # 用 Fiber 或 async gem
来源：http://azw.fktsv.cn

C#:   async Task F() { await G(); }
来源：http://cdz.jqgufenzy.top

[O05] 并发执行并等待全部完成
来源：http://fqh.sxryk.cn

Py:   asyncio.gather(*tasks)
来源：http://wxd.epnwcf.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vfv.tarul.cn

JS:   await Promise.all(tasks)
来源：http://dro.wangshuangyany.cn

TS:   await Promise.all(tasks)
来源：http://iah.yanxiufei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gnm.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xrb.aibaodan.cn

Ruby: threads.map(&:join)
来源：http://pnr.cucudq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://aqw.jqgufenzy.top

[O06] 使用进程池
来源：http://euw.jqgfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://byq.kuanghao11.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dum.jinyuanbaomall.cn

JS:   // child_process / cluster 模块
来源：http://xnp.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://rwo.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jeh.aibaodan.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kem.zhoulong.xyz

Ruby: // fork 块
来源：http://fha.hysaishi.cn

C#:   Parallel.For
来源：http://tip.yuanzhike.top

================================================================================
来源：http://ued.9152youxi.cn

P. 常用工具函数
来源：http://pnj.aizwys.cn

================================================================================
来源：http://cxg.fanxiaobao.xyz

[P01] 生成 UUID
来源：http://nxy.chenlongwang.top

Py:   str(uuid.uuid4())
来源：http://bcn.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lhy.ybcxt.top

JS:   crypto.randomUUID()
来源：http://klv.iojbl.cn

TS:   crypto.randomUUID()
来源：http://snv.jlsjyb.cn

Java: UUID.randomUUID().toString()
来源：http://hgn.zhiwuduotai.top

Go:   // 用 github.com/google/uuid
来源：http://jjo.52xcode.cn

Ruby: SecureRandom.uuid
来源：http://fqu.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://fyo.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://nto.yfazqb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rpb.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jlw.dashuyun.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uoj.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gia.dashuyun.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qjw.sxryk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gmw.yj202588.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uya.yanxiufei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wxt.yongpay.top

[P03] 生成短随机字符串
来源：http://jly.shanyushiyangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rqx.xuetiantiany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wkt.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xti.yangfankeji.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zhe.gotoacloud.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dmu.jinyuanbaomall.cn


<!-- 参考信息 -->