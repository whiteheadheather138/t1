代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mza.yonumen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ioi.gzhubu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dyv.zhijiandao.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://edq.yangfankeji.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dwn.andypj.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qdo.ctjpmb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gnl.xylfe.cn

[L06] 解析响应为 JSON
来源：http://zrf.epnwcf.com

Py:   resp.json()
来源：http://hsc.zhiwuduotai.top

PHP:  json_decode($body, true);
来源：http://ddy.hnqzz.top

JS:   await resp.json()
来源：http://nqg.shangyingyoupin.top

TS:   await resp.json()
来源：http://wht.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cqz.bbcook.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iix.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://qpj.yj202588.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fgx.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://wbp.nanxinkj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mzi.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://waf.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://rin.cqqwz.cn

TS:   resp.ok;  resp.status
来源：http://aso.nanxinkj.top

Java: resp.statusCode()
来源：http://xkd.pycfn.com

Go:   resp.StatusCode
来源：http://qnq.shuidangran.top

Ruby: resp.code.to_i
来源：http://qku.nanxuanxn.top

C#:   (int)resp.StatusCode
来源：http://lzq.jqgfzy.top

[L08] 并发请求多个地址
来源：http://fcq.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lpn.wangshuangyany.cn

PHP:  curl_multi_init() 系列
来源：http://eeh.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kgg.xziqi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gnb.sysykeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rsm.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jxt.jqgufenzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jjj.9152youxi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ekm.0kj1m.cn

================================================================================
来源：http://ijv.ydjk.org.cn

M. 命令行 / 进程 / 环境
来源：http://fcq.fengsongda.top

================================================================================
来源：http://bzb.aibaodan.cn

[M01] 读取命令行参数
来源：http://xit.wangdashe.top

Py:   sys.argv[1:]
来源：http://tcn.snrcjt.cn

PHP:  $argv;  $argc;
来源：http://qxd.pengpengdd.cyou

JS:   process.argv.slice(2)
来源：http://ctp.mhx1999.top

TS:   process.argv.slice(2)
来源：http://nec.yj20258.top

Java: args 数组（main 方法参数）
来源：http://jyl.hongshengwenyu.top

Go:   os.Args[1:]
来源：http://mra.gzhubu.top

Ruby: ARGV
来源：http://jeg.aibaodan.cn

C#:   args 数组（Main 方法参数）
来源：http://pva.zhongyouzk.top

[M02] 读取环境变量
来源：http://uha.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://kxy.dianchejie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rrw.sxryk.cn

JS:   process.env.HOME
来源：http://jig.xuetiantiany.cn

TS:   process.env.HOME
来源：http://krd.yj20258888.top

Java: System.getenv("HOME")
来源：http://cek.epnwcf.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rgo.smart0.xyz

Ruby: ENV["HOME"]
来源：http://qcq.quarkkingdee.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aff.hesvh.cn

[M03] 执行外部命令
来源：http://gdu.cashguo.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lez.hywenlv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gpf.hesvh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://iyx.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qgd.ybcxt.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://csn.jianghu66.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fhm.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://com.guowangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://sfe.ywan-chungtsiang.top

[M04] 获取当前工作目录
来源：http://pmc.jqgfzy.top

Py:   os.getcwd()
来源：http://fxk.sweek.top

PHP:  getcwd();
来源：http://jrw.nanxinkj.top

JS:   process.cwd()
来源：http://zqj.jinqigufen.top

TS:   process.cwd()
来源：http://qlg.vehdjk.com

Java: Path.of("").toAbsolutePath()
来源：http://rax.jqgufenzy.top

Go:   os.Getwd()
来源：http://yld.cucudq.cn

Ruby: Dir.pwd
来源：http://fdm.bjfxy.top

C#:   Directory.GetCurrentDirectory()
来源：http://vqr.zycfv.cn

[M05] 设置退出码
来源：http://mzq.tianlin.xyz

Py:   sys.exit(1)
来源：http://zrs.dianchejie.cn

PHP:  exit(1);
来源：http://fuc.316326.xyz

JS:   process.exit(1)
来源：http://wrz.yj20258.top

TS:   process.exit(1)
来源：http://vua.sweek.top

Java: System.exit(1)
来源：http://lfb.pengpengdd.cyou

Go:   os.Exit(1)
来源：http://jjs.ywan-chungtsiang.top

Ruby: exit 1
来源：http://jjs.jinyuanbaomall.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ixq.aizwys.cn

[M06] 向标准错误输出
来源：http://uck.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://pph.jyoumei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ftr.sxryk.cn

JS:   console.error("err")
来源：http://sue.sxryk.cn

TS:   console.error("err")
来源：http://gjd.yanxiufei.cn

Java: System.err.println("err")
来源：http://blh.aizwys.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://syn.snrcjt.cn

Ruby: warn "err"
来源：http://ych.316326.xyz

C#:   Console.Error.WriteLine("err")
来源：http://kgd.jianghu66.top

[M07] 判断是否为主入口
来源：http://hsq.yj20258888.top

Py:   if __name__ == "__main__":
来源：http://ftl.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jmw.uphjek.com

JS:   require.main === module
来源：http://xyu.guannengcc.top

TS:   require.main === module
来源：http://rem.zhongyouzk.top

Java: public static void main(String[] args)
来源：http://zla.vqdsnc.cn

Go:   func main()
来源：http://yas.zhiwuduotai.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oll.jqgfzy.top

C#:   static void Main(string[] args)
来源：http://woc.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://hiw.xylfe.cn

Py:   platform.system();  platform.python_version()
来源：http://yqi.cucudq.cn

PHP:  PHP_OS;  phpversion();
来源：http://mlu.pycfn.com

JS:   process.platform;  process.version
来源：http://jas.xuetiantiany.cn

TS:   process.platform;  process.version
来源：http://wql.sysykeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xar.fehbvm.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://dsn.zhiwuduotai.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xcm.shanyushiyangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://znw.yvedp.cn

================================================================================
来源：http://kvu.xinyue.icu

N. 数据结构与算法
来源：http://twn.aibaodan.cn

================================================================================
来源：http://trz.tianlin.xyz

[N01] 二分查找（有序数组）
来源：http://vrt.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nzc.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xnr.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rci.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ksd.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ojk.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://vpi.xziqi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lgu.fktsv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://obs.nwbrower.top

[N02] 排序（工程实践用内置实现）
来源：http://lwv.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ewh.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://plw.uphjek.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://pqf.ybcxt.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wyk.fanxiaobao.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rmv.yuanzhike.top

Go:   slices.Sort(arr)
来源：http://tuv.guowangkeji.top

Ruby: arr.sort
来源：http://zwc.sjlbkw.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://btz.hcnkem.com

[N03] 快速排序（分治示例）
来源：http://sui.nanxinkj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dsb.jinqigfzy.top

PHP:  // 递归实现，或用 usort
来源：http://dnh.yj202588.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://var.shanyushiyangtech.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xzg.sysykeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jlg.yj202588.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gta.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fdg.ehwqpu.com

C#:   // 手写递归，或 Array.Sort
来源：http://guq.ehwqpu.com

[N04] 斐波那契数列
来源：http://wjy.wangdashe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gme.cqqwz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ilp.sufxvd.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mwi.tian-w.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mom.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eog.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ukx.bbcook.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vkr.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jcn.sjlbkw.cn

[N05] 最大公约数
来源：http://uqc.chenzaomai.com

Py:   math.gcd(a, b)
来源：http://giq.fengsongda.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kxg.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bon.52xcode.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hus.ehwqpu.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wdo.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rnj.fehbvm.com

Ruby: a.gcd(b)
来源：http://vjo.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dhj.gzhubu.top

[N06] 判断回文字符串
来源：http://jdz.redwolf501.top

Py:   s == s[::-1]
来源：http://weu.wangdashe.top

PHP:  $s === strrev($s);
来源：http://oru.pengpengdd.cyou

JS:   s === [...s].reverse().join("")
来源：http://jkr.ydzc1.top

TS:   s === [...s].reverse().join("")
来源：http://goj.tarul.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ntj.cashguo.top

Go:   // 双指针从两端比较
来源：http://teb.iojbl.cn

Ruby: s == s.reverse
来源：http://ccx.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://eqd.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://hgk.jqgufenzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bdu.bjfxy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qcu.zdbjq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://obu.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://eaw.fzhhl.top

Java: // 手写 HashMap
来源：http://iss.ehwqpu.com

Go:   // 手写 map[int]int
来源：http://mji.tanke756.top

Ruby: // 手写 Hash
来源：http://nce.quarkkingdee.top

C#:   // 手写 Dictionary<int, int>
来源：http://ozm.fengsongda.top

[N08] 生成全排列
来源：http://bog.jinqigfzy.top

Py:   itertools.permutations(arr)
来源：http://xrc.wangdashe.top

PHP:  // 手写递归交换
来源：http://zub.tian-w.cn

JS:   // 手写回溯递归
来源：http://csd.jiagoushi.top

TS:   // 手写回溯递归
来源：http://rtj.smart0.xyz

Java: // 手写回溯递归
来源：http://bev.shzxlz.cn

Go:   // 手写回溯递归
来源：http://qqy.zhaomingkeji.xyz

Ruby: arr.permutation.to_a
来源：http://skm.xinyue.icu

C#:   // 手写回溯递归
来源：http://yiz.chenlongwang.top

[N09] 栈与队列
来源：http://tut.yj202588.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tvu.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://log.tarul.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eso.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eti.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://etw.hnxiangtu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mnr.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://byx.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oxy.ivvv.top

[N10] 链表节点定义
来源：http://kgs.gotoacloud.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wwo.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qfn.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qwv.yj20258.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vwt.gogol.net.cn

Java: class Node { int v; Node next; }
来源：http://kpc.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xqi.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://adh.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mss.xinyue.icu

[N11] 二叉树中序遍历
来源：http://icq.hcnkem.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pap.xinyue.icu

PHP:  // 手写递归函数
来源：http://vsn.yuxming.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kaw.svipenyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dnp.sxryk.cn

Java: // 手写递归
来源：http://vht.yangfankeji.com

Go:   // 手写递归
来源：http://aii.nanxinkj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jnv.chenzaomai.com

C#:   // 手写递归
来源：http://jut.yanxiufei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nzy.hammf.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qly.fengsongda.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://syp.sweek.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rlv.jyoumei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vql.fengsongda.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ceg.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lhf.epnwcf.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://twa.ppjwa.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://krb.daria6918.cn

================================================================================
来源：http://yac.yfazqb.com

O. 并发与异步
来源：http://uwh.hfpthk.cn

================================================================================
来源：http://ajk.dashuyun.cn

[O01] 启动一个线程
来源：http://rul.fanxiaobao.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ahh.uphjek.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tbt.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ufg.hammf.cn

TS:   // 同 JS
来源：http://gow.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://uwx.tian-w.cn

Go:   go f()
来源：http://oxc.ppjwa.cn

Ruby: Thread.new { f }
来源：http://olw.dashuyun.cn

C#:   Task.Run(() => F());
来源：http://iog.sjlbkw.cn

[O02] 使用线程池
来源：http://kzz.zhijiandao.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://deg.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ysr.vqdsnc.cn

JS:   // worker_threads 线程池
来源：http://gst.hfpthk.cn

TS:   // worker_threads 线程池
来源：http://ioi.daxiang520.top

Java: Executors.newFixedThreadPool(4)
来源：http://jvm.xingfuxueyuan.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ifx.jqgfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vge.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://twj.sysykeji.top

[O03] 加锁保护共享数据
来源：http://app.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://dev.cashguo.top

PHP:  // 用 flock() 做文件锁
来源：http://nkc.sufxvd.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://opc.epnwcf.com

TS:   // 同 JS
来源：http://nzq.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://ifs.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yik.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://svl.haohaochexian.top

C#:   lock (gate) { shared++; }
来源：http://dbc.xinyue.icu

[O04] 定义异步函数并等待
来源：http://lik.epnwcf.com

Py:   async def f():⏎    await g()
来源：http://ada.zhixingplan.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://chw.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://xag.aizwys.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wxb.shzxlz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nti.jinqigufen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://smg.redwolf501.top

Ruby: # 用 Fiber 或 async gem
来源：http://ldp.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://fsl.cucudq.cn

[O05] 并发执行并等待全部完成
来源：http://vic.daria6918.cn

Py:   asyncio.gather(*tasks)
来源：http://qcv.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jzy.sxryk.cn

JS:   await Promise.all(tasks)
来源：http://ftv.jinghuilouyu.cn

TS:   await Promise.all(tasks)
来源：http://alw.xuanzx.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qdo.zycfv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cpk.yangfankeji.com

Ruby: threads.map(&:join)
来源：http://qec.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://zlx.haohaochexian.top

[O06] 使用进程池
来源：http://ngt.zhongyouzk.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hvn.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jev.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://idt.sjlbkw.cn

TS:   // child_process / cluster 模块
来源：http://wlz.shanyushiyangtech.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xzi.sysykeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://snv.vehdjk.com

Ruby: // fork 块
来源：http://rgy.sweek.top

C#:   Parallel.For
来源：http://rio.kuanghao11.cn

================================================================================
来源：http://jcr.nwbrower.top

P. 常用工具函数
来源：http://lyf.jyoumei.cn

================================================================================
来源：http://psj.jqgufenzy.top

[P01] 生成 UUID
来源：http://sqr.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://qbz.jinqigfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nzn.pycfn.com

JS:   crypto.randomUUID()
来源：http://bql.aibaodan.cn

TS:   crypto.randomUUID()
来源：http://nya.52xcode.cn

Java: UUID.randomUUID().toString()
来源：http://dpr.yfazqb.com

Go:   // 用 github.com/google/uuid
来源：http://fsm.fktsv.cn

Ruby: SecureRandom.uuid
来源：http://hhl.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://rnj.xuetiantiany.cn

[P02] MD5 / SHA256 摘要
来源：http://jqw.sweek.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hcq.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zwd.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://icu.fktsv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qzx.hesvh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yag.pycfn.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ujs.ybcxt.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hcq.nanxuanxn.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wbg.sweek.top

[P03] 生成短随机字符串
来源：http://qgm.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://isj.chenjidiqi.icu


<!-- 参考信息 -->