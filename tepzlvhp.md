代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vck.zhoulong.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://otj.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jmr.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://feo.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://utp.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uae.ybcxt.top

[L05] 上传文件（multipart）
来源：http://gga.aibaodan.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hhq.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tcb.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://apm.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ufs.yvedp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mqj.9152youxi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xhp.zhaomingkeji.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gfh.gzhubu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aey.hcnkem.com

[L06] 解析响应为 JSON
来源：http://nse.zdqjudy.top

Py:   resp.json()
来源：http://xrk.svipenyu.cn

PHP:  json_decode($body, true);
来源：http://gtz.xuanzx.com

JS:   await resp.json()
来源：http://gnl.chenjidiqi.icu

TS:   await resp.json()
来源：http://oxp.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xvn.ywan-chungtsiang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ztb.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://jcc.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tkn.yueranfly.top

[L07] 处理 HTTP 状态码
来源：http://jhv.yvedp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oke.iojbl.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gbx.aizwys.cn

JS:   resp.ok;  resp.status
来源：http://nkl.zdqjudy.top

TS:   resp.ok;  resp.status
来源：http://dfc.pycfn.com

Java: resp.statusCode()
来源：http://ryr.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://hea.jianghu66.top

Ruby: resp.code.to_i
来源：http://xyr.tarul.cn

C#:   (int)resp.StatusCode
来源：http://azz.aibaodan.cn

[L08] 并发请求多个地址
来源：http://rzl.sufxvd.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yzr.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://kji.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xej.cucudq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gwg.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zox.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://poi.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zvk.cqqwz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mjz.jyoumei.cn

================================================================================
来源：http://zem.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://xiv.shzxlz.cn

================================================================================
来源：http://bok.ehwqpu.com

[M01] 读取命令行参数
来源：http://sej.xuanzx.com

Py:   sys.argv[1:]
来源：http://ayh.svipenyu.cn

PHP:  $argv;  $argc;
来源：http://nlr.yj20258.top

JS:   process.argv.slice(2)
来源：http://mqd.nwbrower.top

TS:   process.argv.slice(2)
来源：http://oho.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://klx.chenjidiqi.icu

Go:   os.Args[1:]
来源：http://cia.cdnleiting.top

Ruby: ARGV
来源：http://psn.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://tgr.kuanghao11.cn

[M02] 读取环境变量
来源：http://fbu.quarkkingdee.top

Py:   os.environ.get("HOME")
来源：http://jze.sxryk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gky.nwbrower.top

JS:   process.env.HOME
来源：http://xss.cheryme.top

TS:   process.env.HOME
来源：http://wkv.bjfxy.top

Java: System.getenv("HOME")
来源：http://kbt.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pjp.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://oqc.cdnleiting.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://whj.pengpengdd.cyou

[M03] 执行外部命令
来源：http://yby.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lvl.fehbvm.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zwx.xylfe.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dxe.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://kxg.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sdm.ybcxt.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vgu.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://pqx.gotoacloud.top

C#:   Process.Start("ls", "-l");
来源：http://jit.tian-w.cn

[M04] 获取当前工作目录
来源：http://twb.chenlongwang.top

Py:   os.getcwd()
来源：http://xhe.zhoulong.xyz

PHP:  getcwd();
来源：http://wac.xingfuxueyuan.xyz

JS:   process.cwd()
来源：http://dqu.tanke756.top

TS:   process.cwd()
来源：http://pea.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://zky.ehwqpu.com

Go:   os.Getwd()
来源：http://vte.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://viy.vqdsnc.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bws.gzhubu.top

[M05] 设置退出码
来源：http://dhq.hnqzz.top

Py:   sys.exit(1)
来源：http://agj.zycfv.cn

PHP:  exit(1);
来源：http://jrt.gogol.net.cn

JS:   process.exit(1)
来源：http://dxd.zhixingplan.top

TS:   process.exit(1)
来源：http://efh.xylfe.cn

Java: System.exit(1)
来源：http://jer.zdbjq.cn

Go:   os.Exit(1)
来源：http://zry.jinqigufen.top

Ruby: exit 1
来源：http://ker.zhongyouzk.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eda.cheryme.top

[M06] 向标准错误输出
来源：http://yvw.pengpengdd.cyou

Py:   print("err", file=sys.stderr)
来源：http://qzj.jyoumei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vzt.shanyushiyangtech.top

JS:   console.error("err")
来源：http://zoc.xylfe.cn

TS:   console.error("err")
来源：http://swx.yonumen.top

Java: System.err.println("err")
来源：http://mdw.guannengcc.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xlt.hysaishi.cn

Ruby: warn "err"
来源：http://zru.haohaochexian.top

C#:   Console.Error.WriteLine("err")
来源：http://pkr.cqqwz.cn

[M07] 判断是否为主入口
来源：http://qkv.yj202588.top

Py:   if __name__ == "__main__":
来源：http://yus.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bkl.gotoacloud.top

JS:   require.main === module
来源：http://mjw.sufxvd.cn

TS:   require.main === module
来源：http://sdd.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://voz.yonumen.top

Go:   func main()
来源：http://cys.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://igb.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://fxy.fehbvm.com

[M08] 获取系统与运行时信息
来源：http://lpv.yongpay.top

Py:   platform.system();  platform.python_version()
来源：http://kft.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://xdq.guannengcc.top

JS:   process.platform;  process.version
来源：http://kmr.jyoumei.cn

TS:   process.platform;  process.version
来源：http://eet.sxryk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xkc.ctjpmb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://jdy.hysaishi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://szp.jinqigfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://sqt.yonumen.top

================================================================================
来源：http://dfj.shzxlz.cn

N. 数据结构与算法
来源：http://ooz.ydjk.org.cn

================================================================================
来源：http://gsy.cdnleiting.top

[N01] 二分查找（有序数组）
来源：http://qbu.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zfo.yj202588.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jqd.fzhhl.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lut.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ieg.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://osq.cheryme.top

Go:   sort.SearchInts(arr, x)
来源：http://trp.aibaodan.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lth.shuidangran.top

C#:   Array.BinarySearch(arr, x)
来源：http://lvt.gotoacloud.top

[N02] 排序（工程实践用内置实现）
来源：http://ikn.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://tas.cdnleiting.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pkl.aibaodan.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://onq.jqgfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ywm.jqgufenzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kyt.yvedp.cn

Go:   slices.Sort(arr)
来源：http://nmx.daria6918.cn

Ruby: arr.sort
来源：http://xtp.dashuyun.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://haf.yuxming.cn

[N03] 快速排序（分治示例）
来源：http://foo.pycfn.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ixm.ctjpmb.com

PHP:  // 递归实现，或用 usort
来源：http://mdh.cqqwz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uio.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ima.pengpengdd.cyou

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fxx.cucudq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://csf.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fis.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://guz.iojbl.cn

[N04] 斐波那契数列
来源：http://znu.ivvv.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oza.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zwy.ppjwa.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bem.tianlin.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uss.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://obj.uphjek.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hzy.tianlin.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://srr.zdbjq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wsu.hongshengwenyu.top

[N05] 最大公约数
来源：http://qik.redwolf501.top

Py:   math.gcd(a, b)
来源：http://pem.jianghu66.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yis.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cfo.redwolf501.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xro.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ald.316326.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mqy.dashuyun.cn

Ruby: a.gcd(b)
来源：http://kek.yongpay.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lxi.yonumen.top

[N06] 判断回文字符串
来源：http://tji.chenzaomai.com

Py:   s == s[::-1]
来源：http://ihb.tian-w.cn

PHP:  $s === strrev($s);
来源：http://nfx.sjlbkw.cn

JS:   s === [...s].reverse().join("")
来源：http://fok.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://omo.daxiang520.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zpu.epnwcf.com

Go:   // 双指针从两端比较
来源：http://ehk.fehbvm.com

Ruby: s == s.reverse
来源：http://vny.sysykeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ihr.hcnkem.com

[N07] 两数之和（返回下标）
来源：http://bro.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://prt.nwbrower.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rav.jqgfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xuq.jiagoushi.top

TS:   // 手写 Map<string, number>
来源：http://rfb.zdqjudy.top

Java: // 手写 HashMap
来源：http://yjz.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://zvx.yuxming.cn

Ruby: // 手写 Hash
来源：http://zlw.cashguo.top

C#:   // 手写 Dictionary<int, int>
来源：http://hbg.ydjk.org.cn

[N08] 生成全排列
来源：http://ent.ctjpmb.com

Py:   itertools.permutations(arr)
来源：http://vgn.cdnleiting.top

PHP:  // 手写递归交换
来源：http://ohs.gaohongyu789.top

JS:   // 手写回溯递归
来源：http://ksv.jiagoushi.top

TS:   // 手写回溯递归
来源：http://iiq.vehdjk.com

Java: // 手写回溯递归
来源：http://jom.daria6918.cn

Go:   // 手写回溯递归
来源：http://daa.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://npl.jiagoushi.top

C#:   // 手写回溯递归
来源：http://rnc.ywan-chungtsiang.top

[N09] 栈与队列
来源：http://ees.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pfo.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jbu.snrcjt.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fqk.wangdashe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hed.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eun.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tds.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nfh.aibaodan.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pvv.hammf.cn

[N10] 链表节点定义
来源：http://rbu.jiagoushi.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qtk.aizwys.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oha.smart0.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zjd.birdmap.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hkz.zhiwuduotai.top

Java: class Node { int v; Node next; }
来源：http://aty.tian-w.cn

Go:   type Node struct { V int; Next *Node }
来源：http://emm.shzxlz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ske.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hfm.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://kxr.yj20258.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tqo.hywenlv.cn

PHP:  // 手写递归函数
来源：http://vak.shangyingyoupin.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vny.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zhh.guowangkeji.top

Java: // 手写递归
来源：http://iyl.nanxuanxn.top

Go:   // 手写递归
来源：http://cxu.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://waq.ppjwa.cn

C#:   // 手写递归
来源：http://uwi.fzhhl.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://esc.vehdjk.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iau.hesvh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ncf.redwolf501.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pjg.c1oappe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ybr.zhaomingkeji.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vmd.daxiang520.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kjh.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://alz.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gwz.tianlin.xyz

================================================================================
来源：http://lat.xylfe.cn

O. 并发与异步
来源：http://bmb.meibo888.top

================================================================================
来源：http://ijy.sufxvd.cn

[O01] 启动一个线程
来源：http://skr.jianghu66.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uyt.xuanzx.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mgc.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nfx.andypj.xyz

TS:   // 同 JS
来源：http://zah.jianghu66.top

Java: new Thread(() -> f()).start()
来源：http://bzn.yvedp.cn

Go:   go f()
来源：http://eyc.yangfankeji.com

Ruby: Thread.new { f }
来源：http://txs.sysykeji.top

C#:   Task.Run(() => F());
来源：http://bue.shzxlz.cn

[O02] 使用线程池
来源：http://crq.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eqe.wangdashe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xrr.jinqigufen.top

JS:   // worker_threads 线程池
来源：http://cuj.bjfxy.top

TS:   // worker_threads 线程池
来源：http://ptp.shuidangran.top

Java: Executors.newFixedThreadPool(4)
来源：http://ppv.sweek.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://six.dianchejie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ajv.gotoacloud.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ewi.tian-w.cn

[O03] 加锁保护共享数据
来源：http://ghp.jyoumei.cn

Py:   with lock: shared += 1
来源：http://jbw.aibaodan.cn

PHP:  // 用 flock() 做文件锁
来源：http://uqw.ppjwa.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://axr.shzxlz.cn

TS:   // 同 JS
来源：http://xae.shangyingyoupin.top

Java: synchronized (this) { shared++; }
来源：http://ztr.cqqwz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://euu.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://aoj.ctjpmb.com

C#:   lock (gate) { shared++; }
来源：http://bva.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://qug.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://wyw.dianchejie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xno.fktsv.cn

JS:   async function f() { await g(); }
来源：http://qdu.jiagoushi.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bhl.ydjk.org.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uan.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dwx.quarkkingdee.top

Ruby: # 用 Fiber 或 async gem
来源：http://awg.shanyushiyangkeji.top

C#:   async Task F() { await G(); }
来源：http://bvf.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://pkw.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://fbu.guannengcc.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bme.jinyuanbaomall.cn

JS:   await Promise.all(tasks)
来源：http://mah.hywenlv.cn

TS:   await Promise.all(tasks)
来源：http://vqh.nanxinkj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pmn.tarul.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nby.xylfe.cn

Ruby: threads.map(&:join)
来源：http://wul.shanyushiyangtech.top

C#:   await Task.WhenAll(t1, t2)
来源：http://suv.epnwcf.com

[O06] 使用进程池
来源：http://bpt.xuanzx.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xqf.xuanzx.com

PHP:  // pcntl_fork 或多进程队列
来源：http://vvo.jqgfzy.top

JS:   // child_process / cluster 模块
来源：http://xsh.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://vyx.gzhubu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ztf.iojbl.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fqt.gotoacloud.top

Ruby: // fork 块
来源：http://mwn.gotoacloud.top

C#:   Parallel.For
来源：http://gpu.316326.xyz

================================================================================
来源：http://gfd.yuxming.cn

P. 常用工具函数
来源：http://oss.shanyushiyangkeji.top

================================================================================
来源：http://lpp.9152youxi.cn

[P01] 生成 UUID
来源：http://zjs.tarul.cn

Py:   str(uuid.uuid4())
来源：http://hsq.havefunace.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vqd.yvedp.cn

JS:   crypto.randomUUID()
来源：http://soe.chenjidiqi.icu

TS:   crypto.randomUUID()
来源：http://jqn.jinqigfzy.top

Java: UUID.randomUUID().toString()
来源：http://iap.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://khc.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://xsr.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://hdf.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://lgu.iojbl.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tka.chenlongwang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://umm.yanxiufei.cn


<!-- 参考信息 -->