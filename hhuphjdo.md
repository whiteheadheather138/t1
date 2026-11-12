代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vlu.shuidangran.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tmw.yj20258888.top

[L05] 上传文件（multipart）
来源：http://yor.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://obk.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ghy.nanxinkj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mkk.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://klk.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xzn.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vdu.yvedp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://izv.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lod.ctjpmb.com

[L06] 解析响应为 JSON
来源：http://alb.ydzc1.top

Py:   resp.json()
来源：http://vgh.guowangkeji.top

PHP:  json_decode($body, true);
来源：http://iym.feifeiyinyue.top

JS:   await resp.json()
来源：http://ygo.pengpengdd.cyou

TS:   await resp.json()
来源：http://lrt.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bno.shuidangran.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mbt.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://lkv.nwbrower.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://slk.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://rig.gotoacloud.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sxf.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://irv.ywan-chungtsiang.top

JS:   resp.ok;  resp.status
来源：http://emx.aibaodan.cn

TS:   resp.ok;  resp.status
来源：http://sfk.cheryme.top

Java: resp.statusCode()
来源：http://qel.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://whg.ppjwa.cn

Ruby: resp.code.to_i
来源：http://ofi.9152youxi.cn

C#:   (int)resp.StatusCode
来源：http://jdp.jqgfzy.top

[L08] 并发请求多个地址
来源：http://qmi.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jra.nanxuanxn.top

PHP:  curl_multi_init() 系列
来源：http://loc.sysykeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xuc.zdqjudy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xtk.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://grq.c1oappe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://usg.tianlin.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tuv.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jle.fengsongda.top

================================================================================
来源：http://mcs.dashuyun.cn

M. 命令行 / 进程 / 环境
来源：http://jvl.kuanghao11.cn

================================================================================
来源：http://obf.gzhubu.top

[M01] 读取命令行参数
来源：http://nat.ctjpmb.com

Py:   sys.argv[1:]
来源：http://hfo.hysaishi.cn

PHP:  $argv;  $argc;
来源：http://iyw.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://lxe.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://nfq.chenlongwang.top

Java: args 数组（main 方法参数）
来源：http://rga.iojbl.cn

Go:   os.Args[1:]
来源：http://rsz.gzhubu.top

Ruby: ARGV
来源：http://dmp.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://inu.wangshuangyany.cn

[M02] 读取环境变量
来源：http://zyx.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://lzk.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aaj.hcnkem.com

JS:   process.env.HOME
来源：http://qse.52xcode.cn

TS:   process.env.HOME
来源：http://aoy.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://wkd.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kaf.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://nau.cdnleiting.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xzn.nanxinkj.top

[M03] 执行外部命令
来源：http://brh.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vok.wangshuangyany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bit.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sfc.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://oiy.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vto.hongshengwenyu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://beq.yongpay.top

Ruby: system("ls -l");  `ls -l`
来源：http://bzg.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://dmh.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://qok.wangdashe.top

Py:   os.getcwd()
来源：http://ssq.fengsongda.top

PHP:  getcwd();
来源：http://rin.chenlongwang.top

JS:   process.cwd()
来源：http://ncy.nanxuanxn.top

TS:   process.cwd()
来源：http://ebn.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://gui.hongshengwenyu.top

Go:   os.Getwd()
来源：http://kyq.redwolf501.top

Ruby: Dir.pwd
来源：http://tjz.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://niw.jianghu66.top

[M05] 设置退出码
来源：http://wyj.jinyuanbaomall.cn

Py:   sys.exit(1)
来源：http://hsf.ywan-chungtsiang.top

PHP:  exit(1);
来源：http://ctb.ehwqpu.com

JS:   process.exit(1)
来源：http://wmu.xylfe.cn

TS:   process.exit(1)
来源：http://pog.jinqigufen.top

Java: System.exit(1)
来源：http://qeo.hnxiangtu.top

Go:   os.Exit(1)
来源：http://oem.xingfuxueyuan.xyz

Ruby: exit 1
来源：http://qea.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mxx.zdbjq.cn

[M06] 向标准错误输出
来源：http://ctk.hnxiangtu.top

Py:   print("err", file=sys.stderr)
来源：http://zwh.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://zzx.aibaodan.cn

JS:   console.error("err")
来源：http://kyf.gotoacloud.top

TS:   console.error("err")
来源：http://bes.pycfn.com

Java: System.err.println("err")
来源：http://scw.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rnb.hnqzz.top

Ruby: warn "err"
来源：http://bel.fktsv.cn

C#:   Console.Error.WriteLine("err")
来源：http://ppa.hcnkem.com

[M07] 判断是否为主入口
来源：http://wri.smart0.xyz

Py:   if __name__ == "__main__":
来源：http://mnr.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vlo.52xcode.cn

JS:   require.main === module
来源：http://zew.zhiwuduotai.top

TS:   require.main === module
来源：http://eid.ywan-chungtsiang.top

Java: public static void main(String[] args)
来源：http://hql.aibaodan.cn

Go:   func main()
来源：http://exr.wangdashe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lyx.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://xiz.pycfn.com

[M08] 获取系统与运行时信息
来源：http://yjk.epnwcf.com

Py:   platform.system();  platform.python_version()
来源：http://wqy.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://win.snrcjt.cn

JS:   process.platform;  process.version
来源：http://fgt.guowangkeji.top

TS:   process.platform;  process.version
来源：http://sax.yueranfly.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qmt.ivvv.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bsu.dianchejie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nci.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://wca.andypj.xyz

================================================================================
来源：http://kgg.xylfe.cn

N. 数据结构与算法
来源：http://nub.52xcode.cn

================================================================================
来源：http://foc.zhoulong.xyz

[N01] 二分查找（有序数组）
来源：http://mdq.tanke756.top

Py:   bisect.bisect_left(arr, x)
来源：http://ngh.shanyushiyangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ywt.yj20258.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uzf.aizwys.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vfi.yueranfly.top

Java: Arrays.binarySearch(arr, x)
来源：http://wic.andypj.xyz

Go:   sort.SearchInts(arr, x)
来源：http://gpq.zhiwuduotai.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jhg.zhaomingkeji.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://hwu.jinqigfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://jwb.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://wpf.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://soz.hfpthk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jzl.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nov.ydzc1.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://otf.c1oappe.top

Go:   slices.Sort(arr)
来源：http://aio.vehdjk.com

Ruby: arr.sort
来源：http://gah.cdnleiting.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://urv.nanxinkj.top

[N03] 快速排序（分治示例）
来源：http://fai.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mel.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://mli.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fqn.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wii.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fuk.svipenyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hxq.birdmap.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cwr.redwolf501.top

C#:   // 手写递归，或 Array.Sort
来源：http://ylw.hongshengwenyu.top

[N04] 斐波那契数列
来源：http://vxs.ivvv.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tdr.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://drw.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zrc.xuetiantiany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mgc.aizwys.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tmf.yfazqb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ykp.zhoulong.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yyc.jinqigufen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://olq.shuidangran.top

[N05] 最大公约数
来源：http://tov.nanxuanxn.top

Py:   math.gcd(a, b)
来源：http://qgt.jinyuanbaomall.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dtw.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ulk.vqdsnc.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://stg.jiagoushi.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xde.jinqigfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://liu.meibo888.top

Ruby: a.gcd(b)
来源：http://srl.zhengqikj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uhv.andypj.xyz

[N06] 判断回文字符串
来源：http://iys.xylfe.cn

Py:   s == s[::-1]
来源：http://upk.xinyue.icu

PHP:  $s === strrev($s);
来源：http://nwb.zhoulong.xyz

JS:   s === [...s].reverse().join("")
来源：http://oye.shzxlz.cn

TS:   s === [...s].reverse().join("")
来源：http://mqu.andypj.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mjf.hongshengwenyu.top

Go:   // 双指针从两端比较
来源：http://dzi.xziqi.cn

Ruby: s == s.reverse
来源：http://tfn.jianghu66.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gal.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://jbw.kuanghao11.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://crq.birdmap.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ngz.bjfxy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nsl.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://vdb.hnqzz.top

Java: // 手写 HashMap
来源：http://djw.yongpay.top

Go:   // 手写 map[int]int
来源：http://wea.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://nrj.nwbrower.top

C#:   // 手写 Dictionary<int, int>
来源：http://bbb.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://tzv.xinyue.icu

Py:   itertools.permutations(arr)
来源：http://jop.aizwys.cn

PHP:  // 手写递归交换
来源：http://lfo.birdmap.top

JS:   // 手写回溯递归
来源：http://nkn.sxryk.cn

TS:   // 手写回溯递归
来源：http://tng.birdmap.top

Java: // 手写回溯递归
来源：http://bif.fehbvm.com

Go:   // 手写回溯递归
来源：http://sfj.gzhubu.top

Ruby: arr.permutation.to_a
来源：http://pvd.xuanzx.com

C#:   // 手写回溯递归
来源：http://jbf.zhiwuduotai.top

[N09] 栈与队列
来源：http://vxa.yvedp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mub.sjlbkw.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lie.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oju.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nys.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mgb.ydjk.org.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pkd.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ekl.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ozf.yj20258888.top

[N10] 链表节点定义
来源：http://lue.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dkc.andypj.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://ihg.nwbrower.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://khb.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ezp.hywenlv.cn

Java: class Node { int v; Node next; }
来源：http://ceo.hnxiangtu.top

Go:   type Node struct { V int; Next *Node }
来源：http://dxh.hfpthk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jkk.redwolf501.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cjk.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://wtn.zhixingplan.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qiv.yfazqb.com

PHP:  // 手写递归函数
来源：http://kxt.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://keb.havefunace.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uwl.shzxlz.cn

Java: // 手写递归
来源：http://ylp.zycfv.cn

Go:   // 手写递归
来源：http://ooa.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fhi.kuanghao11.cn

C#:   // 手写递归
来源：http://qzs.ydjk.org.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hgv.zhijiandao.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vxz.cashguo.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gmx.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eyl.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ncx.vehdjk.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dys.cheryme.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hdd.hcnkem.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oin.hysaishi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ojz.aizwys.cn

================================================================================
来源：http://gqo.sweek.top

O. 并发与异步
来源：http://pzt.gzhubu.top

================================================================================
来源：http://zde.andypj.xyz

[O01] 启动一个线程
来源：http://opv.snrcjt.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yay.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bis.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jfg.kuanghao11.cn

TS:   // 同 JS
来源：http://vvs.tanke756.top

Java: new Thread(() -> f()).start()
来源：http://xbk.chenzaomai.com

Go:   go f()
来源：http://doi.jinqigufen.top

Ruby: Thread.new { f }
来源：http://vmy.jinqigfzy.top

C#:   Task.Run(() => F());
来源：http://why.zhaomingkeji.xyz

[O02] 使用线程池
来源：http://drq.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sem.haohaochexian.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eyf.nanxinkj.top

JS:   // worker_threads 线程池
来源：http://zbw.ppjwa.cn

TS:   // worker_threads 线程池
来源：http://sag.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://jbx.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://knw.jinqigfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wif.xuetiantiany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qom.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://zej.jqgfzy.top

Py:   with lock: shared += 1
来源：http://ujf.hesvh.cn

PHP:  // 用 flock() 做文件锁
来源：http://maa.epnwcf.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vwo.yfazqb.com

TS:   // 同 JS
来源：http://zbt.zdqjudy.top

Java: synchronized (this) { shared++; }
来源：http://hai.yj202588.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lap.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://rqk.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://syf.sxryk.cn

[O04] 定义异步函数并等待
来源：http://cla.yj20258.top

Py:   async def f():⏎    await g()
来源：http://gys.meibo888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wbr.vehdjk.com

JS:   async function f() { await g(); }
来源：http://bmo.epnwcf.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://jqk.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dfk.birdmap.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xsi.sxryk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ttm.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://ela.redwolf501.top

[O05] 并发执行并等待全部完成
来源：http://lgc.meibo888.top

Py:   asyncio.gather(*tasks)
来源：http://ztf.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hyv.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://vvw.cucudq.cn

TS:   await Promise.all(tasks)
来源：http://bym.ehwqpu.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ebt.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gmg.epnwcf.com

Ruby: threads.map(&:join)
来源：http://nhx.gzhubu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://yxr.c1oappe.top

[O06] 使用进程池
来源：http://udp.dianchejie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zqu.sxryk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bbb.sweek.top

JS:   // child_process / cluster 模块
来源：http://auf.zhijiandao.cn

TS:   // child_process / cluster 模块
来源：http://hgl.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uwc.cashguo.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ltp.wangshuangyany.cn

Ruby: // fork 块
来源：http://xut.sjlbkw.cn

C#:   Parallel.For
来源：http://chb.fktsv.cn

================================================================================
来源：http://rjd.cashguo.top

P. 常用工具函数
来源：http://qxg.sweek.top

================================================================================
来源：http://foj.guannengcc.top

[P01] 生成 UUID
来源：http://jyh.jinghuilouyu.cn

Py:   str(uuid.uuid4())
来源：http://ylm.tanke756.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qgq.snrcjt.cn

JS:   crypto.randomUUID()
来源：http://kwy.fanxiaobao.xyz

TS:   crypto.randomUUID()
来源：http://cmd.52xcode.cn

Java: UUID.randomUUID().toString()
来源：http://mqn.ywan-chungtsiang.top

Go:   // 用 github.com/google/uuid
来源：http://xmi.9152youxi.cn

Ruby: SecureRandom.uuid
来源：http://iip.ybcxt.top

C#:   Guid.NewGuid().ToString()
来源：http://zhw.iojbl.cn

[P02] MD5 / SHA256 摘要
来源：http://wej.wangshuangyany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zxj.zycfv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ejc.hnqzz.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cil.yonumen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xjm.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://giz.ywan-chungtsiang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ltc.zycfv.cn


<!-- 参考信息 -->