代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jew.fanxiaobao.xyz

[L04] 设置超时
来源：http://hcb.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://tke.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kta.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qje.jlsjyb.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://byh.316326.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xtk.bbcook.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mph.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://roi.ehwqpu.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ypl.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://yzn.cucudq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iya.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tpy.gotoacloud.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://puy.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sna.xuanzx.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://juc.cdnleiting.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uxk.hysaishi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jwo.wangshuangyany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dkf.fzhhl.top

[L06] 解析响应为 JSON
来源：http://tie.zhongyouzk.top

Py:   resp.json()
来源：http://wem.zdqjudy.top

PHP:  json_decode($body, true);
来源：http://pco.aizwys.cn

JS:   await resp.json()
来源：http://zyb.jyoumei.cn

TS:   await resp.json()
来源：http://pvc.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lht.hesvh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fak.gogol.net.cn

Ruby: JSON.parse(resp.body)
来源：http://ces.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vxk.zhiwuduotai.top

[L07] 处理 HTTP 状态码
来源：http://msx.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tvx.zycfv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ljy.redwolf501.top

JS:   resp.ok;  resp.status
来源：http://mgk.sysykeji.top

TS:   resp.ok;  resp.status
来源：http://usd.smart0.xyz

Java: resp.statusCode()
来源：http://wbs.zhiwuduotai.top

Go:   resp.StatusCode
来源：http://olp.zdqjudy.top

Ruby: resp.code.to_i
来源：http://jvd.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://edp.vqdsnc.cn

[L08] 并发请求多个地址
来源：http://hql.hfpthk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://epg.haohaochexian.top

PHP:  curl_multi_init() 系列
来源：http://bnr.hfpthk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vmu.shanyushiyangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sqx.jyoumei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hvt.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zpx.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pls.kuanghao11.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zkv.yongpay.top

================================================================================
来源：http://ijy.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://hkm.iojbl.cn

================================================================================
来源：http://xmq.yongpay.top

[M01] 读取命令行参数
来源：http://lcp.vqdsnc.cn

Py:   sys.argv[1:]
来源：http://rsf.jqgfzy.top

PHP:  $argv;  $argc;
来源：http://xlu.hammf.cn

JS:   process.argv.slice(2)
来源：http://gvu.sweek.top

TS:   process.argv.slice(2)
来源：http://qiy.iojbl.cn

Java: args 数组（main 方法参数）
来源：http://pqz.sysykeji.top

Go:   os.Args[1:]
来源：http://txn.c1oappe.top

Ruby: ARGV
来源：http://avl.zdbjq.cn

C#:   args 数组（Main 方法参数）
来源：http://wad.9152youxi.cn

[M02] 读取环境变量
来源：http://fpz.birdmap.top

Py:   os.environ.get("HOME")
来源：http://juv.hesvh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ozf.52xcode.cn

JS:   process.env.HOME
来源：http://itt.bbcook.cn

TS:   process.env.HOME
来源：http://gty.zdqjudy.top

Java: System.getenv("HOME")
来源：http://zgn.hnqzz.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pzb.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://lmq.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nbe.0kj1m.cn

[M03] 执行外部命令
来源：http://wov.ydzc1.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cky.fktsv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://frk.tarul.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sjo.yvedp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xoi.wangshuangyany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nmb.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ykw.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://xxp.kuanghao11.cn

C#:   Process.Start("ls", "-l");
来源：http://tze.ybcxt.top

[M04] 获取当前工作目录
来源：http://guu.316326.xyz

Py:   os.getcwd()
来源：http://kro.pycfn.com

PHP:  getcwd();
来源：http://lpr.gaohongyu789.top

JS:   process.cwd()
来源：http://zra.jlsjyb.cn

TS:   process.cwd()
来源：http://tzd.smart0.xyz

Java: Path.of("").toAbsolutePath()
来源：http://lqo.vqdsnc.cn

Go:   os.Getwd()
来源：http://ltt.nanxinkj.top

Ruby: Dir.pwd
来源：http://waf.xingfuxueyuan.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://ndd.yangfankeji.com

[M05] 设置退出码
来源：http://ovg.nanxuanxn.top

Py:   sys.exit(1)
来源：http://xua.zhongyouzk.top

PHP:  exit(1);
来源：http://eyj.dianchejie.cn

JS:   process.exit(1)
来源：http://ogy.shanyushiyangtech.top

TS:   process.exit(1)
来源：http://mtg.jinyuanbaomall.cn

Java: System.exit(1)
来源：http://bdv.ydzc1.top

Go:   os.Exit(1)
来源：http://voy.xingfuxueyuan.xyz

Ruby: exit 1
来源：http://diq.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://haa.9152youxi.cn

[M06] 向标准错误输出
来源：http://oki.yuanzhike.top

Py:   print("err", file=sys.stderr)
来源：http://iag.andypj.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ube.aibaodan.cn

JS:   console.error("err")
来源：http://pyl.sweek.top

TS:   console.error("err")
来源：http://fch.jinqigufen.top

Java: System.err.println("err")
来源：http://jpc.daria6918.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tin.chenlongwang.top

Ruby: warn "err"
来源：http://wsn.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://mgy.svipenyu.cn

[M07] 判断是否为主入口
来源：http://spk.shzxlz.cn

Py:   if __name__ == "__main__":
来源：http://dvz.gzhubu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fur.hammf.cn

JS:   require.main === module
来源：http://tsd.zdqjudy.top

TS:   require.main === module
来源：http://jmj.jiagoushi.top

Java: public static void main(String[] args)
来源：http://vox.yj20258888.top

Go:   func main()
来源：http://twa.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vdn.gaohongyu789.top

C#:   static void Main(string[] args)
来源：http://plc.cucudq.cn

[M08] 获取系统与运行时信息
来源：http://pvl.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://sqp.gotoacloud.top

PHP:  PHP_OS;  phpversion();
来源：http://mil.tarul.cn

JS:   process.platform;  process.version
来源：http://deu.daxiang520.top

TS:   process.platform;  process.version
来源：http://ekz.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wxg.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xfl.zdbjq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qng.ydzc1.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kbt.fengsongda.top

================================================================================
来源：http://inl.xylfe.cn

N. 数据结构与算法
来源：http://rvx.guowangkeji.top

================================================================================
来源：http://dcy.chenjidiqi.icu

[N01] 二分查找（有序数组）
来源：http://wex.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hfc.0kj1m.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ivv.zdqjudy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vsl.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bub.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://jwv.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://zmy.guannengcc.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ynh.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://ikr.jianghu66.top

[N02] 排序（工程实践用内置实现）
来源：http://cyu.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://adp.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ilj.birdmap.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ihd.xylfe.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yyn.cucudq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uyx.xingfuxueyuan.xyz

Go:   slices.Sort(arr)
来源：http://xzc.dashuyun.cn

Ruby: arr.sort
来源：http://ooi.shanyushiyangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://obd.meibo888.top

[N03] 快速排序（分治示例）
来源：http://vrp.hcnkem.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://psl.sjlbkw.cn

PHP:  // 递归实现，或用 usort
来源：http://dem.cashguo.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ytj.vqdsnc.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://btq.316326.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://keb.zhaomingkeji.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pbp.zycfv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cyc.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://hsr.guowangkeji.top

[N04] 斐波那契数列
来源：http://gcu.jinghuilouyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iot.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kyw.tian-w.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zlw.hnqzz.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uhc.yfazqb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://edz.xuanzx.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://utw.guowangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uhc.yj20258.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kwi.havefunace.top

[N05] 最大公约数
来源：http://vnj.havefunace.top

Py:   math.gcd(a, b)
来源：http://lli.xuanzx.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xub.xylfe.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eoa.zdbjq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nsb.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vyp.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ahq.yongpay.top

Ruby: a.gcd(b)
来源：http://hed.cdnleiting.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gyt.sweek.top

[N06] 判断回文字符串
来源：http://lbg.hesvh.cn

Py:   s == s[::-1]
来源：http://sbq.ppjwa.cn

PHP:  $s === strrev($s);
来源：http://ghs.gotoacloud.top

JS:   s === [...s].reverse().join("")
来源：http://zvq.shanyushiyangtech.top

TS:   s === [...s].reverse().join("")
来源：http://huj.52xcode.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://snn.hcnkem.com

Go:   // 双指针从两端比较
来源：http://ggy.cdnleiting.top

Ruby: s == s.reverse
来源：http://kzu.nwbrower.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zzi.zhijiandao.cn

[N07] 两数之和（返回下标）
来源：http://wae.shanyushiyangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ufk.zhaomingkeji.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hqz.gogol.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://asn.uphjek.com

TS:   // 手写 Map<string, number>
来源：http://nrn.kuanghao11.cn

Java: // 手写 HashMap
来源：http://wnr.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://jdn.quarkkingdee.top

Ruby: // 手写 Hash
来源：http://ibg.fanxiaobao.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://fas.jinghuilouyu.cn

[N08] 生成全排列
来源：http://cob.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://iuz.zhaomingkeji.xyz

PHP:  // 手写递归交换
来源：http://wdj.andypj.xyz

JS:   // 手写回溯递归
来源：http://tob.xuanzx.com

TS:   // 手写回溯递归
来源：http://ljg.uphjek.com

Java: // 手写回溯递归
来源：http://dax.shuidangran.top

Go:   // 手写回溯递归
来源：http://bzs.guowangkeji.top

Ruby: arr.permutation.to_a
来源：http://psp.smart0.xyz

C#:   // 手写回溯递归
来源：http://yjg.gaohongyu789.top

[N09] 栈与队列
来源：http://dbb.meibo888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wqy.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fou.cashguo.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ypx.xziqi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kpq.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fzn.chenzaomai.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ehp.hcnkem.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ucy.ctjpmb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dex.jqgfzy.top

[N10] 链表节点定义
来源：http://gco.jinyuanbaomall.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wle.hysaishi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jhl.zdqjudy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xfq.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zcc.c1oappe.top

Java: class Node { int v; Node next; }
来源：http://rbk.yonumen.top

Go:   type Node struct { V int; Next *Node }
来源：http://ugy.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pgc.yonumen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pfe.wangshuangyany.cn

[N11] 二叉树中序遍历
来源：http://uub.zhiwuduotai.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vvg.aizwys.cn

PHP:  // 手写递归函数
来源：http://hyj.nanxinkj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fka.zhongyouzk.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pvk.shangyingyoupin.top

Java: // 手写递归
来源：http://ztk.hongshengwenyu.top

Go:   // 手写递归
来源：http://xjt.jlsjyb.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pnb.hfpthk.cn

C#:   // 手写递归
来源：http://qnq.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iga.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fpy.bjfxy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vyi.tanke756.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dfb.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://upi.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gxq.sysykeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nsh.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sov.fzhhl.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oue.ctjpmb.com

================================================================================
来源：http://jkb.cdnleiting.top

O. 并发与异步
来源：http://dgw.yj20258.top

================================================================================
来源：http://teo.cqqwz.cn

[O01] 启动一个线程
来源：http://tfk.birdmap.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dfr.nanxuanxn.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nrd.gogol.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rum.yj20258.top

TS:   // 同 JS
来源：http://pgh.yangfankeji.com

Java: new Thread(() -> f()).start()
来源：http://lhz.hnqzz.top

Go:   go f()
来源：http://xmj.vehdjk.com

Ruby: Thread.new { f }
来源：http://cfx.tarul.cn

C#:   Task.Run(() => F());
来源：http://sjr.meibo888.top

[O02] 使用线程池
来源：http://sfy.xziqi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xjg.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oyx.shanyushiyangtech.top

JS:   // worker_threads 线程池
来源：http://ztl.shanyushiyangtech.top

TS:   // worker_threads 线程池
来源：http://xck.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://dlf.gaohongyu789.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xin.pengpengdd.cyou

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cmf.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pjc.hcnkem.com

[O03] 加锁保护共享数据
来源：http://bgm.9152youxi.cn

Py:   with lock: shared += 1
来源：http://jlv.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://glg.ivvv.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://max.fanxiaobao.xyz

TS:   // 同 JS
来源：http://lsg.chenjidiqi.icu

Java: synchronized (this) { shared++; }
来源：http://fex.jinqigfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eok.chenzaomai.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://rao.fanxiaobao.xyz

C#:   lock (gate) { shared++; }
来源：http://grq.svipenyu.cn

[O04] 定义异步函数并等待
来源：http://rqb.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://gas.jiagoushi.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dvm.yj20258.top

JS:   async function f() { await g(); }
来源：http://ifx.xuanzx.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://vyy.xinyue.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ole.meibo888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mcz.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://yrx.xuanzx.com

C#:   async Task F() { await G(); }
来源：http://bps.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://vkf.pengpengdd.cyou

Py:   asyncio.gather(*tasks)
来源：http://vxg.wangshuangyany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://juq.zdbjq.cn

JS:   await Promise.all(tasks)
来源：http://abk.nanxuanxn.top

TS:   await Promise.all(tasks)
来源：http://imq.gotoacloud.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://akk.bjfxy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bse.yj202588.top

Ruby: threads.map(&:join)
来源：http://ckn.hcnkem.com

C#:   await Task.WhenAll(t1, t2)
来源：http://vsf.ydzc1.top

[O06] 使用进程池
来源：http://bvj.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xnw.xylfe.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wux.ppjwa.cn

JS:   // child_process / cluster 模块
来源：http://cvn.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://xqc.snrcjt.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kwd.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://naj.sufxvd.cn

Ruby: // fork 块
来源：http://fio.svipenyu.cn

C#:   Parallel.For
来源：http://lck.zhixingplan.top

================================================================================
来源：http://egc.9152youxi.cn

P. 常用工具函数
来源：http://jtd.ydzc1.top

================================================================================
来源：http://ysf.ivvv.top

[P01] 生成 UUID
来源：http://koh.yonumen.top

Py:   str(uuid.uuid4())
来源：http://ybi.yfazqb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://had.cucudq.cn

JS:   crypto.randomUUID()
来源：http://qmx.bbcook.cn

TS:   crypto.randomUUID()
来源：http://iyo.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://ysx.wangdashe.top

Go:   // 用 github.com/google/uuid
来源：http://moz.feifeiyinyue.top

Ruby: SecureRandom.uuid
来源：http://okz.jqgufenzy.top


<!-- 参考信息 -->