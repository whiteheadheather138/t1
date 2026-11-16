代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nof.jinghuilouyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lkg.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ixa.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ktx.shanyushiyangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mlf.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://swo.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wqt.hywenlv.cn

[L06] 解析响应为 JSON
来源：http://bwx.cashguo.top

Py:   resp.json()
来源：http://ajf.hammf.cn

PHP:  json_decode($body, true);
来源：http://erj.tanke756.top

JS:   await resp.json()
来源：http://inx.zhijiandao.cn

TS:   await resp.json()
来源：http://bgy.hammf.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kfs.chenlongwang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://npg.ppjwa.cn

Ruby: JSON.parse(resp.body)
来源：http://trz.fengsongda.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yun.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://mnp.tian-w.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ewh.hywenlv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gcy.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://ymm.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://aky.sweek.top

Java: resp.statusCode()
来源：http://roe.hnqzz.top

Go:   resp.StatusCode
来源：http://zvm.zhaomingkeji.xyz

Ruby: resp.code.to_i
来源：http://vtd.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://ztv.shzxlz.cn

[L08] 并发请求多个地址
来源：http://cdw.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jyy.yj20258.top

PHP:  curl_multi_init() 系列
来源：http://jqb.smart0.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fum.haohaochexian.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zmc.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hiy.uphjek.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rlh.zhijiandao.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qhg.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://trk.jlsjyb.cn

================================================================================
来源：http://rsg.zdqjudy.top

M. 命令行 / 进程 / 环境
来源：http://rzr.xuetiantiany.cn

================================================================================
来源：http://dqw.redwolf501.top

[M01] 读取命令行参数
来源：http://tzp.zhijiandao.cn

Py:   sys.argv[1:]
来源：http://fmd.hammf.cn

PHP:  $argv;  $argc;
来源：http://jic.tanke756.top

JS:   process.argv.slice(2)
来源：http://svn.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://buq.shangyingyoupin.top

Java: args 数组（main 方法参数）
来源：http://yyy.jinqigufen.top

Go:   os.Args[1:]
来源：http://lde.ybcxt.top

Ruby: ARGV
来源：http://jki.hywenlv.cn

C#:   args 数组（Main 方法参数）
来源：http://jab.zhongyouzk.top

[M02] 读取环境变量
来源：http://srz.tanke756.top

Py:   os.environ.get("HOME")
来源：http://oof.hysaishi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://spc.xuetiantiany.cn

JS:   process.env.HOME
来源：http://afa.tanke756.top

TS:   process.env.HOME
来源：http://yrc.havefunace.top

Java: System.getenv("HOME")
来源：http://ywy.jlsjyb.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wlo.bbcook.cn

Ruby: ENV["HOME"]
来源：http://cct.nanxinkj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cxs.c1oappe.top

[M03] 执行外部命令
来源：http://hsb.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uuf.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zys.yanxiufei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://evf.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yss.shanyushiyangtech.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xzg.sjlbkw.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ujy.zhiwuduotai.top

Ruby: system("ls -l");  `ls -l`
来源：http://vbx.zdbjq.cn

C#:   Process.Start("ls", "-l");
来源：http://oed.yvedp.cn

[M04] 获取当前工作目录
来源：http://qid.jinqigfzy.top

Py:   os.getcwd()
来源：http://ssw.fzhhl.top

PHP:  getcwd();
来源：http://erb.xuetiantiany.cn

JS:   process.cwd()
来源：http://str.feifeiyinyue.top

TS:   process.cwd()
来源：http://xxj.ppjwa.cn

Java: Path.of("").toAbsolutePath()
来源：http://ale.havefunace.top

Go:   os.Getwd()
来源：http://pvk.nwbrower.top

Ruby: Dir.pwd
来源：http://vrb.yj202588.top

C#:   Directory.GetCurrentDirectory()
来源：http://uaj.meibo888.top

[M05] 设置退出码
来源：http://vnn.ydzc1.top

Py:   sys.exit(1)
来源：http://smm.shanyushiyangkeji.top

PHP:  exit(1);
来源：http://ufk.hfpthk.cn

JS:   process.exit(1)
来源：http://ekg.hammf.cn

TS:   process.exit(1)
来源：http://pmd.jiagoushi.top

Java: System.exit(1)
来源：http://jut.chenlongwang.top

Go:   os.Exit(1)
来源：http://kan.hnxiangtu.top

Ruby: exit 1
来源：http://fmj.xuetiantiany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xwt.andypj.xyz

[M06] 向标准错误输出
来源：http://tdq.yj202588.top

Py:   print("err", file=sys.stderr)
来源：http://xls.zhijiandao.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qik.aizwys.cn

JS:   console.error("err")
来源：http://jgu.jinqigfzy.top

TS:   console.error("err")
来源：http://uvf.jinqigufen.top

Java: System.err.println("err")
来源：http://jrl.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xdm.quarkkingdee.top

Ruby: warn "err"
来源：http://mey.vehdjk.com

C#:   Console.Error.WriteLine("err")
来源：http://ont.jinqigufen.top

[M07] 判断是否为主入口
来源：http://fga.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://ojf.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kte.sufxvd.cn

JS:   require.main === module
来源：http://jmi.zhiwuduotai.top

TS:   require.main === module
来源：http://jrz.fktsv.cn

Java: public static void main(String[] args)
来源：http://fir.guowangkeji.top

Go:   func main()
来源：http://agp.guowangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zwz.yj20258.top

C#:   static void Main(string[] args)
来源：http://xqd.hongshengwenyu.top

[M08] 获取系统与运行时信息
来源：http://sct.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://qrz.xingfuxueyuan.xyz

PHP:  PHP_OS;  phpversion();
来源：http://bew.nwbrower.top

JS:   process.platform;  process.version
来源：http://jpv.c1oappe.top

TS:   process.platform;  process.version
来源：http://pde.cheryme.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hto.smart0.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://qji.jqgfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qez.snrcjt.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://axl.feifeiyinyue.top

================================================================================
来源：http://pqm.hysaishi.cn

N. 数据结构与算法
来源：http://rrd.hfpthk.cn

================================================================================
来源：http://msu.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://fab.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://svb.yj202588.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cqd.xylfe.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pso.shanyushiyangtech.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pxy.svipenyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://krc.guannengcc.top

Go:   sort.SearchInts(arr, x)
来源：http://usg.aibaodan.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://koi.vehdjk.com

C#:   Array.BinarySearch(arr, x)
来源：http://sdw.bjfxy.top

[N02] 排序（工程实践用内置实现）
来源：http://cor.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://evr.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dng.chenjidiqi.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://tgl.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ght.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cxp.yuanzhike.top

Go:   slices.Sort(arr)
来源：http://wse.hnxiangtu.top

Ruby: arr.sort
来源：http://zhb.epnwcf.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://sni.yj20258888.top

[N03] 快速排序（分治示例）
来源：http://gub.hysaishi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pqr.hysaishi.cn

PHP:  // 递归实现，或用 usort
来源：http://lhv.ivvv.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kdi.zdqjudy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wjg.yfazqb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ogu.hammf.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rlp.sufxvd.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tfr.cdnleiting.top

C#:   // 手写递归，或 Array.Sort
来源：http://dkc.jinqigfzy.top

[N04] 斐波那契数列
来源：http://wla.cucudq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zfk.zhaomingkeji.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yiu.fehbvm.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rtq.yongpay.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xxz.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ixl.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kie.hfpthk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mxm.zhongyouzk.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nyl.yfazqb.com

[N05] 最大公约数
来源：http://kwk.snrcjt.cn

Py:   math.gcd(a, b)
来源：http://bqn.cucudq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vfu.zhengqikj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://urq.xuetiantiany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lej.shangyingyoupin.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jfi.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bpx.birdmap.top

Ruby: a.gcd(b)
来源：http://azk.yj202588.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pnc.zdbjq.cn

[N06] 判断回文字符串
来源：http://ocq.hywenlv.cn

Py:   s == s[::-1]
来源：http://yyt.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://zoe.hywenlv.cn

JS:   s === [...s].reverse().join("")
来源：http://yxt.cheryme.top

TS:   s === [...s].reverse().join("")
来源：http://gov.hesvh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ong.chenlongwang.top

Go:   // 双指针从两端比较
来源：http://vda.nwbrower.top

Ruby: s == s.reverse
来源：http://rkh.ivvv.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mfi.jqgufenzy.top

[N07] 两数之和（返回下标）
来源：http://gkg.ydjk.org.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ilr.cucudq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bpj.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://com.hnqzz.top

TS:   // 手写 Map<string, number>
来源：http://slk.cucudq.cn

Java: // 手写 HashMap
来源：http://rvf.havefunace.top

Go:   // 手写 map[int]int
来源：http://lfr.yangfankeji.com

Ruby: // 手写 Hash
来源：http://mqu.hywenlv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zpt.0kj1m.cn

[N08] 生成全排列
来源：http://scq.ydjk.org.cn

Py:   itertools.permutations(arr)
来源：http://sfl.xziqi.cn

PHP:  // 手写递归交换
来源：http://uml.svipenyu.cn

JS:   // 手写回溯递归
来源：http://vbc.zycfv.cn

TS:   // 手写回溯递归
来源：http://ntd.chenjidiqi.icu

Java: // 手写回溯递归
来源：http://oly.xingfuxueyuan.xyz

Go:   // 手写回溯递归
来源：http://ovt.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://lwr.meibo888.top

C#:   // 手写回溯递归
来源：http://erf.tanke756.top

[N09] 栈与队列
来源：http://gpe.c1oappe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oag.hesvh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uqt.xuanzx.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://use.hnqzz.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oss.yueranfly.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ckh.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uta.cheryme.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jsa.meibo888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vos.mhx1999.top

[N10] 链表节点定义
来源：http://mux.xuanzx.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://spj.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jxe.jqgfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://elf.yj20258.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jxd.snrcjt.cn

Java: class Node { int v; Node next; }
来源：http://oti.vqdsnc.cn

Go:   type Node struct { V int; Next *Node }
来源：http://enn.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tky.smart0.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://pqh.smart0.xyz

[N11] 二叉树中序遍历
来源：http://etn.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://reg.yangfankeji.com

PHP:  // 手写递归函数
来源：http://xtz.zycfv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://asd.ydjk.org.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rjf.jinyuanbaomall.cn

Java: // 手写递归
来源：http://jsk.ybcxt.top

Go:   // 手写递归
来源：http://apu.jlsjyb.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hfx.chenjidiqi.icu

C#:   // 手写递归
来源：http://tob.guowangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zgd.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mnm.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mdx.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cip.yangfankeji.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kny.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qcm.yj202588.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sed.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sdn.aibaodan.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sre.shangyingyoupin.top

================================================================================
来源：http://uit.zdbjq.cn

O. 并发与异步
来源：http://yme.jianghu66.top

================================================================================
来源：http://rdx.redwolf501.top

[O01] 启动一个线程
来源：http://pfp.fanxiaobao.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ymc.yfazqb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://svx.gogol.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jty.chenlongwang.top

TS:   // 同 JS
来源：http://wef.shangyingyoupin.top

Java: new Thread(() -> f()).start()
来源：http://pru.hesvh.cn

Go:   go f()
来源：http://xor.ydjk.org.cn

Ruby: Thread.new { f }
来源：http://inu.jinghuilouyu.cn

C#:   Task.Run(() => F());
来源：http://qjs.jinghuilouyu.cn

[O02] 使用线程池
来源：http://wyl.zdbjq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ynm.ydjk.org.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rnq.uphjek.com

JS:   // worker_threads 线程池
来源：http://bpn.sxryk.cn

TS:   // worker_threads 线程池
来源：http://yyl.yonumen.top

Java: Executors.newFixedThreadPool(4)
来源：http://aps.shanyushiyangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://psr.hnxiangtu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ujl.hesvh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gkb.chenlongwang.top

[O03] 加锁保护共享数据
来源：http://yld.hammf.cn

Py:   with lock: shared += 1
来源：http://rdw.zhoulong.xyz

PHP:  // 用 flock() 做文件锁
来源：http://wnj.ivvv.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mjq.zhijiandao.cn

TS:   // 同 JS
来源：http://npx.hnqzz.top

Java: synchronized (this) { shared++; }
来源：http://ono.fzhhl.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dyw.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wxw.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://nrc.zycfv.cn

[O04] 定义异步函数并等待
来源：http://scl.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://adt.zycfv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zsp.yuanzhike.top

JS:   async function f() { await g(); }
来源：http://bab.jinqigfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jnn.shuidangran.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gdl.jiagoushi.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lnx.wangdashe.top

Ruby: # 用 Fiber 或 async gem
来源：http://bud.jianghu66.top

C#:   async Task F() { await G(); }
来源：http://hog.shanyushiyangkeji.top

[O05] 并发执行并等待全部完成
来源：http://qiu.zhongyouzk.top

Py:   asyncio.gather(*tasks)
来源：http://iqs.hammf.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mtk.shanyushiyangkeji.top

JS:   await Promise.all(tasks)
来源：http://ghd.svipenyu.cn

TS:   await Promise.all(tasks)
来源：http://cue.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xhw.daxiang520.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zqu.jyoumei.cn

Ruby: threads.map(&:join)
来源：http://zyu.zdbjq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bko.yonumen.top

[O06] 使用进程池
来源：http://ayy.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ezt.cdnleiting.top

PHP:  // pcntl_fork 或多进程队列
来源：http://iey.bbcook.cn

JS:   // child_process / cluster 模块
来源：http://zmo.epnwcf.com

TS:   // child_process / cluster 模块
来源：http://kvm.haohaochexian.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rje.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cug.epnwcf.com

Ruby: // fork 块
来源：http://vaq.mhx1999.top

C#:   Parallel.For
来源：http://rjs.hesvh.cn

================================================================================
来源：http://nyi.zhiwuduotai.top

P. 常用工具函数
来源：http://jci.cdnleiting.top

================================================================================
来源：http://gmy.yj20258888.top

[P01] 生成 UUID
来源：http://iom.zhoulong.xyz

Py:   str(uuid.uuid4())
来源：http://dck.fengsongda.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pgo.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://sil.sxryk.cn

TS:   crypto.randomUUID()
来源：http://yhf.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://uql.52xcode.cn

Go:   // 用 github.com/google/uuid
来源：http://pzj.cashguo.top

Ruby: SecureRandom.uuid
来源：http://bsn.nwbrower.top

C#:   Guid.NewGuid().ToString()
来源：http://vxb.hammf.cn

[P02] MD5 / SHA256 摘要
来源：http://jei.yueranfly.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pwv.bjfxy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lnl.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zdn.daria6918.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zzu.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cxz.fktsv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://szn.nanxuanxn.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zdk.smart0.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ffq.zhoulong.xyz

[P03] 生成短随机字符串
来源：http://fmk.sweek.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://axk.cheryme.top


<!-- 参考信息 -->