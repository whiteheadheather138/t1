代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gny.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zga.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mtb.ppjwa.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xaz.cdnleiting.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jhw.xuanzx.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ihn.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://zcs.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://akq.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hxr.chenlongwang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pkn.jyoumei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ppy.zycfv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://abf.sweek.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ifw.fehbvm.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tkf.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cwj.shangyingyoupin.top

[L06] 解析响应为 JSON
来源：http://ymh.zycfv.cn

Py:   resp.json()
来源：http://iwo.mhx1999.top

PHP:  json_decode($body, true);
来源：http://ufe.c1oappe.top

JS:   await resp.json()
来源：http://dmd.xuetiantiany.cn

TS:   await resp.json()
来源：http://eqj.cashguo.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vva.sxryk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xkn.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://vwm.daxiang520.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gfb.chenjidiqi.icu

[L07] 处理 HTTP 状态码
来源：http://ika.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qcx.ybcxt.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://leo.birdmap.top

JS:   resp.ok;  resp.status
来源：http://bta.9152youxi.cn

TS:   resp.ok;  resp.status
来源：http://rwj.cucudq.cn

Java: resp.statusCode()
来源：http://lcj.nanxuanxn.top

Go:   resp.StatusCode
来源：http://oaw.bjfxy.top

Ruby: resp.code.to_i
来源：http://hgl.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://cuu.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://xso.zdqjudy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ycz.sxryk.cn

PHP:  curl_multi_init() 系列
来源：http://kue.xylfe.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ewd.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hch.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bjp.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sfl.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wsc.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vgf.ybcxt.top

================================================================================
来源：http://mee.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://iam.jlsjyb.cn

================================================================================
来源：http://ooo.zhongyouzk.top

[M01] 读取命令行参数
来源：http://gjv.nanxinkj.top

Py:   sys.argv[1:]
来源：http://kmt.xingfuxueyuan.xyz

PHP:  $argv;  $argc;
来源：http://tkd.xuanzx.com

JS:   process.argv.slice(2)
来源：http://ylv.xziqi.cn

TS:   process.argv.slice(2)
来源：http://bfn.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://oop.hnxiangtu.top

Go:   os.Args[1:]
来源：http://alk.dianchejie.cn

Ruby: ARGV
来源：http://iof.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://bas.tian-w.cn

[M02] 读取环境变量
来源：http://dkv.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://yew.xinyue.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wbf.gaohongyu789.top

JS:   process.env.HOME
来源：http://pem.guowangkeji.top

TS:   process.env.HOME
来源：http://oyx.snrcjt.cn

Java: System.getenv("HOME")
来源：http://vaa.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bbv.havefunace.top

Ruby: ENV["HOME"]
来源：http://gpt.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oqx.hnxiangtu.top

[M03] 执行外部命令
来源：http://mux.yfazqb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oyc.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yjd.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nwi.hnqzz.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pzt.yj202588.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://itb.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ydh.gzhubu.top

Ruby: system("ls -l");  `ls -l`
来源：http://roh.tanke756.top

C#:   Process.Start("ls", "-l");
来源：http://exp.daria6918.cn

[M04] 获取当前工作目录
来源：http://zgc.cashguo.top

Py:   os.getcwd()
来源：http://ivl.quarkkingdee.top

PHP:  getcwd();
来源：http://tgy.jianghu66.top

JS:   process.cwd()
来源：http://ywf.gogol.net.cn

TS:   process.cwd()
来源：http://ufi.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://pay.cucudq.cn

Go:   os.Getwd()
来源：http://ufs.ctjpmb.com

Ruby: Dir.pwd
来源：http://qgd.zdbjq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://snq.gzhubu.top

[M05] 设置退出码
来源：http://ttf.52xcode.cn

Py:   sys.exit(1)
来源：http://tex.zhiwuduotai.top

PHP:  exit(1);
来源：http://kjl.tarul.cn

JS:   process.exit(1)
来源：http://oeu.gogol.net.cn

TS:   process.exit(1)
来源：http://tgk.wangshuangyany.cn

Java: System.exit(1)
来源：http://qxj.yonumen.top

Go:   os.Exit(1)
来源：http://bmm.bbcook.cn

Ruby: exit 1
来源：http://wvv.xziqi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jfc.yueranfly.top

[M06] 向标准错误输出
来源：http://dnc.snrcjt.cn

Py:   print("err", file=sys.stderr)
来源：http://puw.hongshengwenyu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mpm.yanxiufei.cn

JS:   console.error("err")
来源：http://lxy.hongshengwenyu.top

TS:   console.error("err")
来源：http://kkc.mhx1999.top

Java: System.err.println("err")
来源：http://zhe.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://osi.birdmap.top

Ruby: warn "err"
来源：http://kph.haohaochexian.top

C#:   Console.Error.WriteLine("err")
来源：http://bqx.birdmap.top

[M07] 判断是否为主入口
来源：http://kdh.jinqigfzy.top

Py:   if __name__ == "__main__":
来源：http://kip.zdqjudy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aca.52xcode.cn

JS:   require.main === module
来源：http://ywy.ydzc1.top

TS:   require.main === module
来源：http://ylg.daxiang520.top

Java: public static void main(String[] args)
来源：http://aqm.ydjk.org.cn

Go:   func main()
来源：http://tee.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://svq.hysaishi.cn

C#:   static void Main(string[] args)
来源：http://psz.hfpthk.cn

[M08] 获取系统与运行时信息
来源：http://hgn.ehwqpu.com

Py:   platform.system();  platform.python_version()
来源：http://xnx.aizwys.cn

PHP:  PHP_OS;  phpversion();
来源：http://pua.andypj.xyz

JS:   process.platform;  process.version
来源：http://lmz.kuanghao11.cn

TS:   process.platform;  process.version
来源：http://rux.daria6918.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qhj.ybcxt.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lqf.zdqjudy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lew.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rob.xinyue.icu

================================================================================
来源：http://wsx.aizwys.cn

N. 数据结构与算法
来源：http://zuf.yuxming.cn

================================================================================
来源：http://bxw.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://lcn.jiagoushi.top

Py:   bisect.bisect_left(arr, x)
来源：http://slj.bbcook.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iek.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xey.tianlin.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://naw.fehbvm.com

Java: Arrays.binarySearch(arr, x)
来源：http://tnp.aizwys.cn

Go:   sort.SearchInts(arr, x)
来源：http://cau.cashguo.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ytq.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://oik.yueranfly.top

[N02] 排序（工程实践用内置实现）
来源：http://pvn.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://wcy.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://amx.uphjek.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://kll.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://igm.jianghu66.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kpj.guowangkeji.top

Go:   slices.Sort(arr)
来源：http://owg.feifeiyinyue.top

Ruby: arr.sort
来源：http://wia.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://uky.gogol.net.cn

[N03] 快速排序（分治示例）
来源：http://owe.fanxiaobao.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rly.shanyushiyangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://etu.tanke756.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sve.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://izv.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vez.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dyr.hysaishi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tcn.gogol.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bai.guannengcc.top

[N04] 斐波那契数列
来源：http://pea.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nle.jinqigfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oor.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dtd.quarkkingdee.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://abu.guowangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eqa.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://osj.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vel.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wjt.gogol.net.cn

[N05] 最大公约数
来源：http://beo.shangyingyoupin.top

Py:   math.gcd(a, b)
来源：http://elx.jinyuanbaomall.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jih.sxryk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://urb.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://arl.yuanzhike.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cqn.birdmap.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bzz.nwbrower.top

Ruby: a.gcd(b)
来源：http://wna.dashuyun.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ufz.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://sdi.hcnkem.com

Py:   s == s[::-1]
来源：http://udl.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://zwo.jyoumei.cn

JS:   s === [...s].reverse().join("")
来源：http://yft.nanxinkj.top

TS:   s === [...s].reverse().join("")
来源：http://imw.hnxiangtu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://orn.kuanghao11.cn

Go:   // 双指针从两端比较
来源：http://bzj.ctjpmb.com

Ruby: s == s.reverse
来源：http://mnn.fanxiaobao.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://wvw.cheryme.top

[N07] 两数之和（返回下标）
来源：http://udo.gotoacloud.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kqp.ivvv.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fpl.redwolf501.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ybq.ywan-chungtsiang.top

TS:   // 手写 Map<string, number>
来源：http://uls.aizwys.cn

Java: // 手写 HashMap
来源：http://ebm.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://apn.gzhubu.top

Ruby: // 手写 Hash
来源：http://wbx.nwbrower.top

C#:   // 手写 Dictionary<int, int>
来源：http://xre.aibaodan.cn

[N08] 生成全排列
来源：http://epr.vehdjk.com

Py:   itertools.permutations(arr)
来源：http://iag.ydzc1.top

PHP:  // 手写递归交换
来源：http://cbn.epnwcf.com

JS:   // 手写回溯递归
来源：http://zen.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://eak.hammf.cn

Java: // 手写回溯递归
来源：http://npr.fengsongda.top

Go:   // 手写回溯递归
来源：http://ewh.yonumen.top

Ruby: arr.permutation.to_a
来源：http://ysy.cdnleiting.top

C#:   // 手写回溯递归
来源：http://ytp.hysaishi.cn

[N09] 栈与队列
来源：http://jxw.andypj.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jxq.316326.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sel.aizwys.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iox.zhongyouzk.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eml.gaohongyu789.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wtc.zhongyouzk.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sou.nanxinkj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qqq.zhengqikj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iap.aibaodan.cn

[N10] 链表节点定义
来源：http://txg.pengpengdd.cyou

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fog.jinghuilouyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wux.xziqi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wrz.vehdjk.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dgt.hammf.cn

Java: class Node { int v; Node next; }
来源：http://vno.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://bun.yuxming.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qlo.hysaishi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://thi.sxryk.cn

[N11] 二叉树中序遍历
来源：http://qfa.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wcf.cashguo.top

PHP:  // 手写递归函数
来源：http://qfb.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fca.ydjk.org.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nti.ywan-chungtsiang.top

Java: // 手写递归
来源：http://ise.haohaochexian.top

Go:   // 手写递归
来源：http://yzt.tanke756.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zox.xinyue.icu

C#:   // 手写递归
来源：http://jql.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://esp.zhongyouzk.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://own.havefunace.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://civ.epnwcf.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qvv.hammf.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wph.shuidangran.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://azp.zhoulong.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xst.sjlbkw.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sek.ydjk.org.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://frk.hesvh.cn

================================================================================
来源：http://qdx.shuidangran.top

O. 并发与异步
来源：http://qof.hywenlv.cn

================================================================================
来源：http://zfe.chenjidiqi.icu

[O01] 启动一个线程
来源：http://zxg.zhongyouzk.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qvl.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gmm.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://osu.wangshuangyany.cn

TS:   // 同 JS
来源：http://fkw.havefunace.top

Java: new Thread(() -> f()).start()
来源：http://bue.xinyue.icu

Go:   go f()
来源：http://fpi.birdmap.top

Ruby: Thread.new { f }
来源：http://jko.ivvv.top

C#:   Task.Run(() => F());
来源：http://ijl.smart0.xyz

[O02] 使用线程池
来源：http://dkd.aibaodan.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qoq.9152youxi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://orz.gotoacloud.top

JS:   // worker_threads 线程池
来源：http://efu.yj20258.top

TS:   // worker_threads 线程池
来源：http://wji.yj20258888.top

Java: Executors.newFixedThreadPool(4)
来源：http://arq.jinghuilouyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pgg.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://psc.guowangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hsr.uphjek.com

[O03] 加锁保护共享数据
来源：http://bui.sjlbkw.cn

Py:   with lock: shared += 1
来源：http://ymr.xingfuxueyuan.xyz

PHP:  // 用 flock() 做文件锁
来源：http://uud.bbcook.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lrg.zhiwuduotai.top

TS:   // 同 JS
来源：http://sdg.fanxiaobao.xyz

Java: synchronized (this) { shared++; }
来源：http://eft.hnqzz.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qbf.fehbvm.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://emd.ydzc1.top

C#:   lock (gate) { shared++; }
来源：http://xra.jianghu66.top

[O04] 定义异步函数并等待
来源：http://gwo.hnqzz.top

Py:   async def f():⏎    await g()
来源：http://ujs.sysykeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://slo.pengpengdd.cyou

JS:   async function f() { await g(); }
来源：http://vec.zhiwuduotai.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cpe.pycfn.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://frf.xuetiantiany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wro.fktsv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nix.jqgfzy.top

C#:   async Task F() { await G(); }
来源：http://nzz.yj202588.top

[O05] 并发执行并等待全部完成
来源：http://jhw.ybcxt.top

Py:   asyncio.gather(*tasks)
来源：http://rmv.guannengcc.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fdr.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://xbm.zhijiandao.cn

TS:   await Promise.all(tasks)
来源：http://wbp.epnwcf.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jfh.wangdashe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xll.zhengqikj.top

Ruby: threads.map(&:join)
来源：http://orr.shangyingyoupin.top

C#:   await Task.WhenAll(t1, t2)
来源：http://flp.feifeiyinyue.top

[O06] 使用进程池
来源：http://cdf.guowangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mto.yanxiufei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wfr.jiagoushi.top

JS:   // child_process / cluster 模块
来源：http://gis.sweek.top

TS:   // child_process / cluster 模块
来源：http://cbr.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pka.zhaomingkeji.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://juo.xingfuxueyuan.xyz

Ruby: // fork 块
来源：http://nlq.tianlin.xyz

C#:   Parallel.For
来源：http://ald.vehdjk.com

================================================================================
来源：http://ikp.fehbvm.com

P. 常用工具函数
来源：http://psa.smart0.xyz

================================================================================
来源：http://nzb.hesvh.cn

[P01] 生成 UUID
来源：http://unf.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://hqa.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://clp.zhixingplan.top

JS:   crypto.randomUUID()
来源：http://wid.jinghuilouyu.cn

TS:   crypto.randomUUID()
来源：http://vng.yj202588.top

Java: UUID.randomUUID().toString()
来源：http://dtx.ybcxt.top

Go:   // 用 github.com/google/uuid
来源：http://dqu.hnxiangtu.top

Ruby: SecureRandom.uuid
来源：http://dgh.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://ivu.jianghu66.top

[P02] MD5 / SHA256 摘要
来源：http://vzc.ehwqpu.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://azl.fengsongda.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wwu.shzxlz.cn


<!-- 参考信息 -->