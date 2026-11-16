代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oqx.9152youxi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sed.zhaomingkeji.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qxq.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sbq.jinghuilouyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pfh.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dxc.nanxinkj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ksp.jianghu66.top

[L06] 解析响应为 JSON
来源：http://zyq.shzxlz.cn

Py:   resp.json()
来源：http://euc.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://dcy.ctjpmb.com

JS:   await resp.json()
来源：http://omi.birdmap.top

TS:   await resp.json()
来源：http://dbh.daxiang520.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oyp.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cpq.jinqigufen.top

Ruby: JSON.parse(resp.body)
来源：http://hbz.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ama.jinqigufen.top

[L07] 处理 HTTP 状态码
来源：http://rle.aizwys.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hyd.meibo888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gul.jlsjyb.cn

JS:   resp.ok;  resp.status
来源：http://iwm.uphjek.com

TS:   resp.ok;  resp.status
来源：http://ncm.ehwqpu.com

Java: resp.statusCode()
来源：http://fsf.yvedp.cn

Go:   resp.StatusCode
来源：http://rgt.yueranfly.top

Ruby: resp.code.to_i
来源：http://xnq.hesvh.cn

C#:   (int)resp.StatusCode
来源：http://raw.ydjk.org.cn

[L08] 并发请求多个地址
来源：http://amc.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://weq.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://eyn.shangyingyoupin.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://svd.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tnp.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://njl.hysaishi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rjz.316326.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yep.cdnleiting.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hte.chenlongwang.top

================================================================================
来源：http://hkx.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://bmn.gzhubu.top

================================================================================
来源：http://kmh.epnwcf.com

[M01] 读取命令行参数
来源：http://qqp.snrcjt.cn

Py:   sys.argv[1:]
来源：http://tiv.hywenlv.cn

PHP:  $argv;  $argc;
来源：http://wii.fzhhl.top

JS:   process.argv.slice(2)
来源：http://byz.cucudq.cn

TS:   process.argv.slice(2)
来源：http://vtv.cdnleiting.top

Java: args 数组（main 方法参数）
来源：http://rxm.ehwqpu.com

Go:   os.Args[1:]
来源：http://pbm.fengsongda.top

Ruby: ARGV
来源：http://xdg.zhengqikj.top

C#:   args 数组（Main 方法参数）
来源：http://bek.bjfxy.top

[M02] 读取环境变量
来源：http://nbw.yueranfly.top

Py:   os.environ.get("HOME")
来源：http://cjp.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fbj.zhaomingkeji.xyz

JS:   process.env.HOME
来源：http://wvf.zdqjudy.top

TS:   process.env.HOME
来源：http://xoy.haohaochexian.top

Java: System.getenv("HOME")
来源：http://zvx.smart0.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://svr.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://gsj.jiagoushi.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hlu.hongshengwenyu.top

[M03] 执行外部命令
来源：http://szs.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zqv.gogol.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iyc.fanxiaobao.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://koi.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xio.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pof.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xdw.ivvv.top

Ruby: system("ls -l");  `ls -l`
来源：http://sgr.jinqigfzy.top

C#:   Process.Start("ls", "-l");
来源：http://usl.yj20258.top

[M04] 获取当前工作目录
来源：http://ywf.ivvv.top

Py:   os.getcwd()
来源：http://gcx.9152youxi.cn

PHP:  getcwd();
来源：http://nff.hesvh.cn

JS:   process.cwd()
来源：http://cza.zdbjq.cn

TS:   process.cwd()
来源：http://fjr.yanxiufei.cn

Java: Path.of("").toAbsolutePath()
来源：http://iqe.zdqjudy.top

Go:   os.Getwd()
来源：http://apy.jinqigfzy.top

Ruby: Dir.pwd
来源：http://zba.xylfe.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wps.ydzc1.top

[M05] 设置退出码
来源：http://qyq.yongpay.top

Py:   sys.exit(1)
来源：http://for.daxiang520.top

PHP:  exit(1);
来源：http://ccu.zhixingplan.top

JS:   process.exit(1)
来源：http://owi.hywenlv.cn

TS:   process.exit(1)
来源：http://pah.jinqigfzy.top

Java: System.exit(1)
来源：http://mqx.cheryme.top

Go:   os.Exit(1)
来源：http://jva.birdmap.top

Ruby: exit 1
来源：http://jvw.9152youxi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sud.fehbvm.com

[M06] 向标准错误输出
来源：http://hlj.hywenlv.cn

Py:   print("err", file=sys.stderr)
来源：http://pry.shangyingyoupin.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qyc.ydjk.org.cn

JS:   console.error("err")
来源：http://gsb.zhaomingkeji.xyz

TS:   console.error("err")
来源：http://qzs.xziqi.cn

Java: System.err.println("err")
来源：http://csa.yangfankeji.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ygy.pengpengdd.cyou

Ruby: warn "err"
来源：http://vmg.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://xoq.fengsongda.top

[M07] 判断是否为主入口
来源：http://ahb.chenzaomai.com

Py:   if __name__ == "__main__":
来源：http://yum.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tgf.quarkkingdee.top

JS:   require.main === module
来源：http://fzi.quarkkingdee.top

TS:   require.main === module
来源：http://zjf.ehwqpu.com

Java: public static void main(String[] args)
来源：http://sqo.jiagoushi.top

Go:   func main()
来源：http://dgv.jianghu66.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ouc.ydzc1.top

C#:   static void Main(string[] args)
来源：http://ekq.c1oappe.top

[M08] 获取系统与运行时信息
来源：http://osl.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://jda.bjfxy.top

PHP:  PHP_OS;  phpversion();
来源：http://uzq.wangdashe.top

JS:   process.platform;  process.version
来源：http://cpt.tianlin.xyz

TS:   process.platform;  process.version
来源：http://bwl.ehwqpu.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dlm.daria6918.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vpl.ehwqpu.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tfe.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://znp.gogol.net.cn

================================================================================
来源：http://std.kuanghao11.cn

N. 数据结构与算法
来源：http://clz.cheryme.top

================================================================================
来源：http://fov.mhx1999.top

[N01] 二分查找（有序数组）
来源：http://tfy.zhengqikj.top

Py:   bisect.bisect_left(arr, x)
来源：http://dda.shzxlz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rye.9152youxi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://omh.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xek.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jhy.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://ejw.yuanzhike.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vou.xylfe.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lbb.yongpay.top

[N02] 排序（工程实践用内置实现）
来源：http://jeh.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://dkn.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zqm.hammf.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zxs.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yfd.sxryk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gyt.nwbrower.top

Go:   slices.Sort(arr)
来源：http://qzp.chenlongwang.top

Ruby: arr.sort
来源：http://dal.jlsjyb.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hpd.ppjwa.cn

[N03] 快速排序（分治示例）
来源：http://tuu.fzhhl.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ugj.fengsongda.top

PHP:  // 递归实现，或用 usort
来源：http://lco.fktsv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://elb.yj20258888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mhb.ppjwa.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aky.fktsv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rvu.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gpa.wangdashe.top

C#:   // 手写递归，或 Array.Sort
来源：http://rbg.xylfe.cn

[N04] 斐波那契数列
来源：http://mue.tarul.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jwv.zhengqikj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wiv.tianlin.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nht.svipenyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://riy.fengsongda.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rqw.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wsj.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xow.zhaomingkeji.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oan.jiagoushi.top

[N05] 最大公约数
来源：http://wjj.yonumen.top

Py:   math.gcd(a, b)
来源：http://nef.epnwcf.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://phx.ybcxt.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://csv.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zzr.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rsa.pycfn.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mdu.sweek.top

Ruby: a.gcd(b)
来源：http://dcm.kuanghao11.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wif.guowangkeji.top

[N06] 判断回文字符串
来源：http://ans.chenzaomai.com

Py:   s == s[::-1]
来源：http://elf.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://vss.shzxlz.cn

JS:   s === [...s].reverse().join("")
来源：http://guq.ydjk.org.cn

TS:   s === [...s].reverse().join("")
来源：http://jde.bbcook.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dpn.aizwys.cn

Go:   // 双指针从两端比较
来源：http://wlx.chenjidiqi.icu

Ruby: s == s.reverse
来源：http://sbw.yvedp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jzq.yuanzhike.top

[N07] 两数之和（返回下标）
来源：http://aud.dianchejie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fll.ivvv.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ema.zhengqikj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yot.mhx1999.top

TS:   // 手写 Map<string, number>
来源：http://sni.tian-w.cn

Java: // 手写 HashMap
来源：http://yps.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://dnp.pycfn.com

Ruby: // 手写 Hash
来源：http://rxn.shzxlz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://aul.zhixingplan.top

[N08] 生成全排列
来源：http://uea.dashuyun.cn

Py:   itertools.permutations(arr)
来源：http://alb.cucudq.cn

PHP:  // 手写递归交换
来源：http://ysp.smart0.xyz

JS:   // 手写回溯递归
来源：http://ydz.shanyushiyangtech.top

TS:   // 手写回溯递归
来源：http://frd.chenlongwang.top

Java: // 手写回溯递归
来源：http://sej.epnwcf.com

Go:   // 手写回溯递归
来源：http://mfx.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://tmj.snrcjt.cn

C#:   // 手写回溯递归
来源：http://fqz.vqdsnc.cn

[N09] 栈与队列
来源：http://zua.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aig.fzhhl.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ghu.tarul.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xzt.jinghuilouyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bha.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aof.wangshuangyany.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ztx.9152youxi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gxs.yj202588.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mqu.zycfv.cn

[N10] 链表节点定义
来源：http://tay.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pui.fengsongda.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uwd.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pdn.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tda.yangfankeji.com

Java: class Node { int v; Node next; }
来源：http://tql.sjlbkw.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qzv.shzxlz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://buq.c1oappe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://oxb.yj202588.top

[N11] 二叉树中序遍历
来源：http://szp.iojbl.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mus.nanxuanxn.top

PHP:  // 手写递归函数
来源：http://eqw.cashguo.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nam.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ska.uphjek.com

Java: // 手写递归
来源：http://hmy.yj202588.top

Go:   // 手写递归
来源：http://kad.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jol.c1oappe.top

C#:   // 手写递归
来源：http://vso.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://osy.gaohongyu789.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oln.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://znc.aizwys.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zui.jianghu66.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rmm.xziqi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cir.daria6918.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dlh.iojbl.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cga.gzhubu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cgu.sysykeji.top

================================================================================
来源：http://voe.fehbvm.com

O. 并发与异步
来源：http://ieb.52xcode.cn

================================================================================
来源：http://pni.sxryk.cn

[O01] 启动一个线程
来源：http://tgp.guowangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kob.epnwcf.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://siw.mhx1999.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nxw.fanxiaobao.xyz

TS:   // 同 JS
来源：http://hsg.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://nvz.shanyushiyangtech.top

Go:   go f()
来源：http://sel.yuanzhike.top

Ruby: Thread.new { f }
来源：http://prb.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://qyv.daria6918.cn

[O02] 使用线程池
来源：http://gft.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lav.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ajp.fengsongda.top

JS:   // worker_threads 线程池
来源：http://vhh.havefunace.top

TS:   // worker_threads 线程池
来源：http://wgo.jiagoushi.top

Java: Executors.newFixedThreadPool(4)
来源：http://nhp.chenlongwang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yir.hcnkem.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fxb.hnqzz.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nzp.wangdashe.top

[O03] 加锁保护共享数据
来源：http://oea.316326.xyz

Py:   with lock: shared += 1
来源：http://cle.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://gmf.gaohongyu789.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://krb.pengpengdd.cyou

TS:   // 同 JS
来源：http://hnv.fzhhl.top

Java: synchronized (this) { shared++; }
来源：http://vhu.meibo888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yrc.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lgi.hysaishi.cn

C#:   lock (gate) { shared++; }
来源：http://riw.chenzaomai.com

[O04] 定义异步函数并等待
来源：http://hgp.yj20258888.top

Py:   async def f():⏎    await g()
来源：http://pgu.cashguo.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jll.shzxlz.cn

JS:   async function f() { await g(); }
来源：http://iye.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://eaq.yfazqb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hug.tianlin.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kaa.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://vtv.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://dcw.sysykeji.top

[O05] 并发执行并等待全部完成
来源：http://ake.ydjk.org.cn

Py:   asyncio.gather(*tasks)
来源：http://vhw.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jpc.dianchejie.cn

JS:   await Promise.all(tasks)
来源：http://juo.tian-w.cn

TS:   await Promise.all(tasks)
来源：http://byp.yuxming.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iwr.guannengcc.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dau.cqqwz.cn

Ruby: threads.map(&:join)
来源：http://rou.yvedp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xju.pycfn.com

[O06] 使用进程池
来源：http://vdh.ybcxt.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mrc.hnxiangtu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zil.fzhhl.top

JS:   // child_process / cluster 模块
来源：http://jpw.zhaomingkeji.xyz

TS:   // child_process / cluster 模块
来源：http://isa.jinqigfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qzw.kuanghao11.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qzc.hnqzz.top

Ruby: // fork 块
来源：http://dau.haohaochexian.top

C#:   Parallel.For
来源：http://vry.havefunace.top

================================================================================
来源：http://uaw.andypj.xyz

P. 常用工具函数
来源：http://csx.ctjpmb.com

================================================================================
来源：http://ibj.hysaishi.cn

[P01] 生成 UUID
来源：http://qkx.nanxinkj.top

Py:   str(uuid.uuid4())
来源：http://nky.hysaishi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tgl.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://jqg.bbcook.cn

TS:   crypto.randomUUID()
来源：http://rfd.birdmap.top

Java: UUID.randomUUID().toString()
来源：http://iot.birdmap.top

Go:   // 用 github.com/google/uuid
来源：http://tlc.wangdashe.top

Ruby: SecureRandom.uuid
来源：http://cuh.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://klb.cqqwz.cn

[P02] MD5 / SHA256 摘要
来源：http://aff.zhengqikj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jzs.hysaishi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yer.andypj.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ybf.nanxuanxn.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ljr.fehbvm.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://acw.0kj1m.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jma.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://onh.yj202588.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gwn.jqgufenzy.top

[P03] 生成短随机字符串
来源：http://xrq.yonumen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://shv.zhaomingkeji.xyz


<!-- 参考信息 -->