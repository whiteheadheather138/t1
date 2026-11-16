代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mot.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eok.xuetiantiany.cn

[L05] 上传文件（multipart）
来源：http://wlf.zdbjq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fht.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zdf.nanxinkj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://atm.0kj1m.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gkm.gotoacloud.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pxz.52xcode.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hdy.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cbe.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nhd.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://ujq.nanxinkj.top

Py:   resp.json()
来源：http://tsq.shzxlz.cn

PHP:  json_decode($body, true);
来源：http://hnf.jinyuanbaomall.cn

JS:   await resp.json()
来源：http://wmv.jqgufenzy.top

TS:   await resp.json()
来源：http://anc.xylfe.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wxc.jinghuilouyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vad.yongpay.top

Ruby: JSON.parse(resp.body)
来源：http://kqy.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mey.gotoacloud.top

[L07] 处理 HTTP 状态码
来源：http://qco.zhongyouzk.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eak.smart0.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nxh.ppjwa.cn

JS:   resp.ok;  resp.status
来源：http://cic.wangdashe.top

TS:   resp.ok;  resp.status
来源：http://wqo.haohaochexian.top

Java: resp.statusCode()
来源：http://hcn.sufxvd.cn

Go:   resp.StatusCode
来源：http://wnx.feifeiyinyue.top

Ruby: resp.code.to_i
来源：http://ehx.nanxuanxn.top

C#:   (int)resp.StatusCode
来源：http://arp.shzxlz.cn

[L08] 并发请求多个地址
来源：http://vuj.c1oappe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lax.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://yom.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rxa.zhoulong.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wtg.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tnc.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xvf.tanke756.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://njf.hongshengwenyu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mbj.sxryk.cn

================================================================================
来源：http://tyn.nanxuanxn.top

M. 命令行 / 进程 / 环境
来源：http://nqt.zdqjudy.top

================================================================================
来源：http://jxq.yj20258.top

[M01] 读取命令行参数
来源：http://zdl.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://hkr.yj202588.top

PHP:  $argv;  $argc;
来源：http://vay.smart0.xyz

JS:   process.argv.slice(2)
来源：http://fic.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://ktn.zhixingplan.top

Java: args 数组（main 方法参数）
来源：http://urt.hammf.cn

Go:   os.Args[1:]
来源：http://eki.vqdsnc.cn

Ruby: ARGV
来源：http://zht.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://ykm.hysaishi.cn

[M02] 读取环境变量
来源：http://wjj.ivvv.top

Py:   os.environ.get("HOME")
来源：http://rqk.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gkh.kuanghao11.cn

JS:   process.env.HOME
来源：http://kpl.ydjk.org.cn

TS:   process.env.HOME
来源：http://ado.dashuyun.cn

Java: System.getenv("HOME")
来源：http://zun.daria6918.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kqv.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://eve.xylfe.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dzb.zhengqikj.top

[M03] 执行外部命令
来源：http://kkj.guannengcc.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vtb.zhaomingkeji.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aai.ctjpmb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://iis.gzhubu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rja.uphjek.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ttt.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://uza.hcnkem.com

Ruby: system("ls -l");  `ls -l`
来源：http://vdq.zhengqikj.top

C#:   Process.Start("ls", "-l");
来源：http://myd.shuidangran.top

[M04] 获取当前工作目录
来源：http://wok.pengpengdd.cyou

Py:   os.getcwd()
来源：http://tel.jinqigufen.top

PHP:  getcwd();
来源：http://atr.guowangkeji.top

JS:   process.cwd()
来源：http://svt.zhongyouzk.top

TS:   process.cwd()
来源：http://kle.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://odx.ywan-chungtsiang.top

Go:   os.Getwd()
来源：http://esa.ivvv.top

Ruby: Dir.pwd
来源：http://crf.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://mdv.shangyingyoupin.top

[M05] 设置退出码
来源：http://zcj.yueranfly.top

Py:   sys.exit(1)
来源：http://yzp.jianghu66.top

PHP:  exit(1);
来源：http://ufn.zhixingplan.top

JS:   process.exit(1)
来源：http://vsm.jlsjyb.cn

TS:   process.exit(1)
来源：http://mog.yj20258.top

Java: System.exit(1)
来源：http://jff.bbcook.cn

Go:   os.Exit(1)
来源：http://xgl.nwbrower.top

Ruby: exit 1
来源：http://gat.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://whg.316326.xyz

[M06] 向标准错误输出
来源：http://lhy.jqgfzy.top

Py:   print("err", file=sys.stderr)
来源：http://xkz.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bbw.fehbvm.com

JS:   console.error("err")
来源：http://ity.zhiwuduotai.top

TS:   console.error("err")
来源：http://wto.fengsongda.top

Java: System.err.println("err")
来源：http://kqk.feifeiyinyue.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wra.pengpengdd.cyou

Ruby: warn "err"
来源：http://joi.zhijiandao.cn

C#:   Console.Error.WriteLine("err")
来源：http://evt.cucudq.cn

[M07] 判断是否为主入口
来源：http://jaa.fanxiaobao.xyz

Py:   if __name__ == "__main__":
来源：http://tis.jianghu66.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ccs.andypj.xyz

JS:   require.main === module
来源：http://ihl.fengsongda.top

TS:   require.main === module
来源：http://ofg.shuidangran.top

Java: public static void main(String[] args)
来源：http://fka.shangyingyoupin.top

Go:   func main()
来源：http://urf.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vwf.fehbvm.com

C#:   static void Main(string[] args)
来源：http://pjk.snrcjt.cn

[M08] 获取系统与运行时信息
来源：http://yqr.yanxiufei.cn

Py:   platform.system();  platform.python_version()
来源：http://nnc.chenlongwang.top

PHP:  PHP_OS;  phpversion();
来源：http://fvd.316326.xyz

JS:   process.platform;  process.version
来源：http://qdv.haohaochexian.top

TS:   process.platform;  process.version
来源：http://dqt.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nfv.haohaochexian.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sxr.fktsv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wnz.xylfe.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hsr.shanyushiyangtech.top

================================================================================
来源：http://xge.tianlin.xyz

N. 数据结构与算法
来源：http://unr.ydjk.org.cn

================================================================================
来源：http://lrf.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://ish.pengpengdd.cyou

Py:   bisect.bisect_left(arr, x)
来源：http://iyc.fengsongda.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qbo.jqgufenzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tjo.xylfe.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vyh.andypj.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://mxe.jinghuilouyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://ksa.mhx1999.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rui.9152youxi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ams.epnwcf.com

[N02] 排序（工程实践用内置实现）
来源：http://tus.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://asi.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aek.zhiwuduotai.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mvz.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rya.jlsjyb.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vpy.chenjidiqi.icu

Go:   slices.Sort(arr)
来源：http://exp.hnxiangtu.top

Ruby: arr.sort
来源：http://zrs.daria6918.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hik.kuanghao11.cn

[N03] 快速排序（分治示例）
来源：http://zyp.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mqo.epnwcf.com

PHP:  // 递归实现，或用 usort
来源：http://oez.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dqz.cdnleiting.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yje.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hjl.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fzi.zhongyouzk.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dop.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://huc.nanxuanxn.top

[N04] 斐波那契数列
来源：http://yzv.zhixingplan.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sjk.sufxvd.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fbr.nwbrower.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vwc.ctjpmb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ytq.hnqzz.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tgp.havefunace.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wlo.jqgfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kkr.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://znb.epnwcf.com

[N05] 最大公约数
来源：http://pez.pycfn.com

Py:   math.gcd(a, b)
来源：http://nfh.sxryk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qzs.yvedp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://grk.zhongyouzk.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ipf.havefunace.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ydw.havefunace.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://luz.yanxiufei.cn

Ruby: a.gcd(b)
来源：http://roq.shanyushiyangtech.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rmr.andypj.xyz

[N06] 判断回文字符串
来源：http://nrn.birdmap.top

Py:   s == s[::-1]
来源：http://fzw.hammf.cn

PHP:  $s === strrev($s);
来源：http://klx.feifeiyinyue.top

JS:   s === [...s].reverse().join("")
来源：http://ahf.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://awk.zhijiandao.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oco.andypj.xyz

Go:   // 双指针从两端比较
来源：http://wrm.ctjpmb.com

Ruby: s == s.reverse
来源：http://xkl.yongpay.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mak.snrcjt.cn

[N07] 两数之和（返回下标）
来源：http://hqg.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xsv.zhixingplan.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oop.feifeiyinyue.top

JS:   // 手写 Map：map.set(v, i)
来源：http://byc.zhongyouzk.top

TS:   // 手写 Map<string, number>
来源：http://eif.c1oappe.top

Java: // 手写 HashMap
来源：http://vvo.shuidangran.top

Go:   // 手写 map[int]int
来源：http://eol.ydzc1.top

Ruby: // 手写 Hash
来源：http://exs.haohaochexian.top

C#:   // 手写 Dictionary<int, int>
来源：http://zan.birdmap.top

[N08] 生成全排列
来源：http://iue.daxiang520.top

Py:   itertools.permutations(arr)
来源：http://btn.zdqjudy.top

PHP:  // 手写递归交换
来源：http://jnc.cashguo.top

JS:   // 手写回溯递归
来源：http://mfq.meibo888.top

TS:   // 手写回溯递归
来源：http://qea.zhengqikj.top

Java: // 手写回溯递归
来源：http://egw.hnqzz.top

Go:   // 手写回溯递归
来源：http://tkc.shzxlz.cn

Ruby: arr.permutation.to_a
来源：http://nsf.smart0.xyz

C#:   // 手写回溯递归
来源：http://soe.bbcook.cn

[N09] 栈与队列
来源：http://waq.ybcxt.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vwg.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ply.wangdashe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://exa.9152youxi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://agu.yuxming.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pkf.uphjek.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lqk.fktsv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qld.daxiang520.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ldv.yuanzhike.top

[N10] 链表节点定义
来源：http://ntq.52xcode.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jsw.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bnv.sjlbkw.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yxg.vehdjk.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sbw.zhaomingkeji.xyz

Java: class Node { int v; Node next; }
来源：http://oiz.shanyushiyangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://tzs.zhongyouzk.top

Ruby: Node = Struct.new(:v, :next)
来源：http://oqw.pengpengdd.cyou

C#:   class Node { public int V; public Node? Next; }
来源：http://rmq.zhaomingkeji.xyz

[N11] 二叉树中序遍历
来源：http://yll.bbcook.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zcn.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://wrj.jyoumei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pgb.svipenyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yhp.hysaishi.cn

Java: // 手写递归
来源：http://rfj.daria6918.cn

Go:   // 手写递归
来源：http://rng.redwolf501.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sev.xingfuxueyuan.xyz

C#:   // 手写递归
来源：http://oef.snrcjt.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://esi.yonumen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wod.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yee.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tio.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kdm.yanxiufei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tib.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eyt.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://goj.aizwys.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tgn.zhengqikj.top

================================================================================
来源：http://kxr.zhiwuduotai.top

O. 并发与异步
来源：http://eiz.uphjek.com

================================================================================
来源：http://yqc.yvedp.cn

[O01] 启动一个线程
来源：http://wuc.pycfn.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oho.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gkv.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://por.jiagoushi.top

TS:   // 同 JS
来源：http://yye.chenzaomai.com

Java: new Thread(() -> f()).start()
来源：http://yxe.jianghu66.top

Go:   go f()
来源：http://iaq.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://zmr.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://rla.sjlbkw.cn

[O02] 使用线程池
来源：http://ufo.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kme.ivvv.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vra.iojbl.cn

JS:   // worker_threads 线程池
来源：http://ukq.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://dov.gogol.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zrh.haohaochexian.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bff.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fqe.yj20258.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dyc.xuetiantiany.cn

[O03] 加锁保护共享数据
来源：http://sld.hywenlv.cn

Py:   with lock: shared += 1
来源：http://uyi.nanxinkj.top

PHP:  // 用 flock() 做文件锁
来源：http://jac.smart0.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tip.cucudq.cn

TS:   // 同 JS
来源：http://ckx.daria6918.cn

Java: synchronized (this) { shared++; }
来源：http://ztr.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dee.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://llx.yuxming.cn

C#:   lock (gate) { shared++; }
来源：http://jvv.zdbjq.cn

[O04] 定义异步函数并等待
来源：http://ijm.hnxiangtu.top

Py:   async def f():⏎    await g()
来源：http://pmq.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sdh.vqdsnc.cn

JS:   async function f() { await g(); }
来源：http://evn.xingfuxueyuan.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://mzc.yj202588.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://toy.ppjwa.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mxb.ydjk.org.cn

Ruby: # 用 Fiber 或 async gem
来源：http://evm.hammf.cn

C#:   async Task F() { await G(); }
来源：http://mta.xuetiantiany.cn

[O05] 并发执行并等待全部完成
来源：http://qqw.pycfn.com

Py:   asyncio.gather(*tasks)
来源：http://qdw.xuanzx.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://olx.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://lhk.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://pty.ppjwa.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iwx.tian-w.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nru.fzhhl.top

Ruby: threads.map(&:join)
来源：http://klx.tanke756.top

C#:   await Task.WhenAll(t1, t2)
来源：http://atq.xuanzx.com

[O06] 使用进程池
来源：http://rab.yfazqb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rmt.hammf.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tak.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://jae.chenlongwang.top

TS:   // child_process / cluster 模块
来源：http://zrg.ivvv.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lhh.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hpd.wangshuangyany.cn

Ruby: // fork 块
来源：http://evd.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://afd.ywan-chungtsiang.top

================================================================================
来源：http://dtr.9152youxi.cn

P. 常用工具函数
来源：http://pph.dianchejie.cn

================================================================================
来源：http://zod.shangyingyoupin.top

[P01] 生成 UUID
来源：http://qzo.dashuyun.cn

Py:   str(uuid.uuid4())
来源：http://she.hnqzz.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vpl.xuanzx.com

JS:   crypto.randomUUID()
来源：http://nqt.yj20258.top

TS:   crypto.randomUUID()
来源：http://aeq.guannengcc.top

Java: UUID.randomUUID().toString()
来源：http://eis.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://aji.gogol.net.cn

Ruby: SecureRandom.uuid
来源：http://gho.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://zub.9152youxi.cn

[P02] MD5 / SHA256 摘要
来源：http://dds.yvedp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gva.zhijiandao.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wfa.yongpay.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gnu.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aun.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xxp.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pwk.iojbl.cn


<!-- 参考信息 -->