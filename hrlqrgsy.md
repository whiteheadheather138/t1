代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lka.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bcs.aizwys.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ygw.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fsn.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nob.ppjwa.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://isb.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://udx.hesvh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xce.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://svy.xingfuxueyuan.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://txi.vehdjk.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gsn.ctjpmb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xss.kuanghao11.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://udg.ydzc1.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bqx.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oto.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://kyw.jqgufenzy.top

Py:   resp.json()
来源：http://vjb.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://fwq.yuanzhike.top

JS:   await resp.json()
来源：http://tcn.meibo888.top

TS:   await resp.json()
来源：http://rdl.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xhh.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kmm.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://oqi.tian-w.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ktw.vehdjk.com

[L07] 处理 HTTP 状态码
来源：http://cvu.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zmh.hammf.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ciz.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://axk.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://pwp.yuanzhike.top

Java: resp.statusCode()
来源：http://vuf.shanyushiyangkeji.top

Go:   resp.StatusCode
来源：http://cct.jinqigufen.top

Ruby: resp.code.to_i
来源：http://nla.yuxming.cn

C#:   (int)resp.StatusCode
来源：http://qpd.9152youxi.cn

[L08] 并发请求多个地址
来源：http://xci.sjlbkw.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vai.cucudq.cn

PHP:  curl_multi_init() 系列
来源：http://lhy.wangshuangyany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bvp.ppjwa.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fvq.shanyushiyangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zbi.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://six.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iyp.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cdv.ydjk.org.cn

================================================================================
来源：http://cmh.cdnleiting.top

M. 命令行 / 进程 / 环境
来源：http://tqq.ybcxt.top

================================================================================
来源：http://qha.yj20258888.top

[M01] 读取命令行参数
来源：http://bri.ybcxt.top

Py:   sys.argv[1:]
来源：http://rup.epnwcf.com

PHP:  $argv;  $argc;
来源：http://uwt.ywan-chungtsiang.top

JS:   process.argv.slice(2)
来源：http://daw.guowangkeji.top

TS:   process.argv.slice(2)
来源：http://jhf.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://fvb.jqgfzy.top

Go:   os.Args[1:]
来源：http://lda.hesvh.cn

Ruby: ARGV
来源：http://tya.kuanghao11.cn

C#:   args 数组（Main 方法参数）
来源：http://ihe.zhengqikj.top

[M02] 读取环境变量
来源：http://uqp.ydjk.org.cn

Py:   os.environ.get("HOME")
来源：http://miz.jinqigfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eyq.shanyushiyangtech.top

JS:   process.env.HOME
来源：http://nsm.ehwqpu.com

TS:   process.env.HOME
来源：http://hvw.birdmap.top

Java: System.getenv("HOME")
来源：http://sow.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zys.epnwcf.com

Ruby: ENV["HOME"]
来源：http://ike.haohaochexian.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://deb.zhengqikj.top

[M03] 执行外部命令
来源：http://kou.pycfn.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sdg.mhx1999.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cvk.chenjidiqi.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://tya.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://puz.smart0.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dag.jinqigufen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://tee.redwolf501.top

Ruby: system("ls -l");  `ls -l`
来源：http://xgl.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://oah.mhx1999.top

[M04] 获取当前工作目录
来源：http://gyn.52xcode.cn

Py:   os.getcwd()
来源：http://knp.zhoulong.xyz

PHP:  getcwd();
来源：http://cfq.sweek.top

JS:   process.cwd()
来源：http://idq.tian-w.cn

TS:   process.cwd()
来源：http://jaa.shuidangran.top

Java: Path.of("").toAbsolutePath()
来源：http://yal.hcnkem.com

Go:   os.Getwd()
来源：http://cam.bbcook.cn

Ruby: Dir.pwd
来源：http://eyd.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hda.tian-w.cn

[M05] 设置退出码
来源：http://mza.shanyushiyangkeji.top

Py:   sys.exit(1)
来源：http://tfu.cucudq.cn

PHP:  exit(1);
来源：http://chx.jinqigufen.top

JS:   process.exit(1)
来源：http://mlg.tian-w.cn

TS:   process.exit(1)
来源：http://khq.zhijiandao.cn

Java: System.exit(1)
来源：http://uqw.pengpengdd.cyou

Go:   os.Exit(1)
来源：http://iue.shangyingyoupin.top

Ruby: exit 1
来源：http://mgd.fehbvm.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rdn.daxiang520.top

[M06] 向标准错误输出
来源：http://tbu.jyoumei.cn

Py:   print("err", file=sys.stderr)
来源：http://pew.meibo888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tiv.jinghuilouyu.cn

JS:   console.error("err")
来源：http://klp.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://ycz.jlsjyb.cn

Java: System.err.println("err")
来源：http://fpc.xuetiantiany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ggp.gzhubu.top

Ruby: warn "err"
来源：http://knr.havefunace.top

C#:   Console.Error.WriteLine("err")
来源：http://zme.xinyue.icu

[M07] 判断是否为主入口
来源：http://jxt.tian-w.cn

Py:   if __name__ == "__main__":
来源：http://gmn.tanke756.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jbh.hammf.cn

JS:   require.main === module
来源：http://iby.bjfxy.top

TS:   require.main === module
来源：http://ctb.ywan-chungtsiang.top

Java: public static void main(String[] args)
来源：http://qbr.xylfe.cn

Go:   func main()
来源：http://zbv.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bqr.xylfe.cn

C#:   static void Main(string[] args)
来源：http://pdt.zhengqikj.top

[M08] 获取系统与运行时信息
来源：http://hpy.shuidangran.top

Py:   platform.system();  platform.python_version()
来源：http://osk.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://sfj.jqgfzy.top

JS:   process.platform;  process.version
来源：http://fru.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://cfv.ehwqpu.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hss.nanxinkj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://leh.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tta.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ykb.fzhhl.top

================================================================================
来源：http://bhg.fzhhl.top

N. 数据结构与算法
来源：http://izf.yangfankeji.com

================================================================================
来源：http://rmi.zhoulong.xyz

[N01] 二分查找（有序数组）
来源：http://mjp.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://ipr.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ysp.mhx1999.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wup.ybcxt.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zmd.andypj.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://nzf.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://lzk.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vrc.ivvv.top

C#:   Array.BinarySearch(arr, x)
来源：http://don.uphjek.com

[N02] 排序（工程实践用内置实现）
来源：http://sdw.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://ckk.shzxlz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://upf.hongshengwenyu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fjq.tanke756.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hqf.fzhhl.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rlp.cheryme.top

Go:   slices.Sort(arr)
来源：http://ipf.ydjk.org.cn

Ruby: arr.sort
来源：http://bwx.shanyushiyangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zqk.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://tlq.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://juu.xuanzx.com

PHP:  // 递归实现，或用 usort
来源：http://yin.ppjwa.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xoy.andypj.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hlp.fengsongda.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lym.svipenyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://juv.sysykeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yoj.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sqh.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://heq.aizwys.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://czr.tianlin.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rgb.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cwm.bjfxy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dve.daxiang520.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cqh.guannengcc.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mtl.ehwqpu.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ydd.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zlt.cqqwz.cn

[N05] 最大公约数
来源：http://zux.yvedp.cn

Py:   math.gcd(a, b)
来源：http://lnm.chenjidiqi.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vki.dianchejie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://joq.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://geq.cashguo.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fot.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tmz.hesvh.cn

Ruby: a.gcd(b)
来源：http://qmf.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mly.xuetiantiany.cn

[N06] 判断回文字符串
来源：http://jzq.tarul.cn

Py:   s == s[::-1]
来源：http://kje.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://xtk.gzhubu.top

JS:   s === [...s].reverse().join("")
来源：http://uat.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://yrr.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dfs.xuanzx.com

Go:   // 双指针从两端比较
来源：http://win.hywenlv.cn

Ruby: s == s.reverse
来源：http://zgm.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jaz.xylfe.cn

[N07] 两数之和（返回下标）
来源：http://hvs.chenjidiqi.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tek.jqgufenzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rto.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bwf.ivvv.top

TS:   // 手写 Map<string, number>
来源：http://ajq.cashguo.top

Java: // 手写 HashMap
来源：http://mgg.c1oappe.top

Go:   // 手写 map[int]int
来源：http://qrt.9152youxi.cn

Ruby: // 手写 Hash
来源：http://uiv.fktsv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://czr.jinyuanbaomall.cn

[N08] 生成全排列
来源：http://wat.hnqzz.top

Py:   itertools.permutations(arr)
来源：http://yce.gotoacloud.top

PHP:  // 手写递归交换
来源：http://alp.bjfxy.top

JS:   // 手写回溯递归
来源：http://vwe.dashuyun.cn

TS:   // 手写回溯递归
来源：http://wgb.hysaishi.cn

Java: // 手写回溯递归
来源：http://tfp.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://hjb.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://qhy.ybcxt.top

C#:   // 手写回溯递归
来源：http://wyd.ehwqpu.com

[N09] 栈与队列
来源：http://vfz.fengsongda.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iwq.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xpm.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hmd.jyoumei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://las.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://znz.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jee.zhijiandao.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fdo.xziqi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bmd.gotoacloud.top

[N10] 链表节点定义
来源：http://ryh.meibo888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zzu.cheryme.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dka.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ztk.yueranfly.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jzo.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://awf.hammf.cn

Go:   type Node struct { V int; Next *Node }
来源：http://meh.fktsv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://clt.gogol.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ace.hcnkem.com

[N11] 二叉树中序遍历
来源：http://eso.52xcode.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fkk.redwolf501.top

PHP:  // 手写递归函数
来源：http://gxj.daxiang520.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gzv.zhaomingkeji.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vwp.gotoacloud.top

Java: // 手写递归
来源：http://wlh.zycfv.cn

Go:   // 手写递归
来源：http://avg.fanxiaobao.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nza.nanxinkj.top

C#:   // 手写递归
来源：http://uxg.sjlbkw.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bpp.fanxiaobao.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hex.tian-w.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://trx.nanxinkj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ata.redwolf501.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ceq.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ugu.havefunace.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pei.daria6918.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vpw.shanyushiyangtech.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://igo.9152youxi.cn

================================================================================
来源：http://qzo.nanxinkj.top

O. 并发与异步
来源：http://lmj.iojbl.cn

================================================================================
来源：http://dso.jinqigufen.top

[O01] 启动一个线程
来源：http://vhn.yj20258.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mlt.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zbs.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qys.316326.xyz

TS:   // 同 JS
来源：http://eqy.chenlongwang.top

Java: new Thread(() -> f()).start()
来源：http://rwj.mhx1999.top

Go:   go f()
来源：http://ibm.chenlongwang.top

Ruby: Thread.new { f }
来源：http://crm.wangdashe.top

C#:   Task.Run(() => F());
来源：http://isr.svipenyu.cn

[O02] 使用线程池
来源：http://dls.pengpengdd.cyou

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sbd.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wbl.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://czj.feifeiyinyue.top

TS:   // worker_threads 线程池
来源：http://iwz.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://lux.guowangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ofe.fzhhl.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ixp.guowangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kwm.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://weh.gotoacloud.top

Py:   with lock: shared += 1
来源：http://ify.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://xnp.fktsv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jmf.yongpay.top

TS:   // 同 JS
来源：http://ttp.yvedp.cn

Java: synchronized (this) { shared++; }
来源：http://tox.guannengcc.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ilr.andypj.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://wyo.pengpengdd.cyou

C#:   lock (gate) { shared++; }
来源：http://ypp.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://ddf.zhijiandao.cn

Py:   async def f():⏎    await g()
来源：http://kwp.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ztw.redwolf501.top

JS:   async function f() { await g(); }
来源：http://tth.tian-w.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gql.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ojs.yvedp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jes.xinyue.icu

Ruby: # 用 Fiber 或 async gem
来源：http://yfi.yongpay.top

C#:   async Task F() { await G(); }
来源：http://bnr.chenlongwang.top

[O05] 并发执行并等待全部完成
来源：http://zlg.meibo888.top

Py:   asyncio.gather(*tasks)
来源：http://gnm.shzxlz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xny.sjlbkw.cn

JS:   await Promise.all(tasks)
来源：http://mzh.c1oappe.top

TS:   await Promise.all(tasks)
来源：http://rmn.hywenlv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tgz.epnwcf.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://phc.kuanghao11.cn

Ruby: threads.map(&:join)
来源：http://onv.hywenlv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ide.yj202588.top

[O06] 使用进程池
来源：http://orx.vqdsnc.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zhf.yangfankeji.com

PHP:  // pcntl_fork 或多进程队列
来源：http://dgb.yj20258888.top

JS:   // child_process / cluster 模块
来源：http://vkb.yj202588.top

TS:   // child_process / cluster 模块
来源：http://uhw.fzhhl.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ive.tanke756.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wnt.zhaomingkeji.xyz

Ruby: // fork 块
来源：http://yib.gzhubu.top

C#:   Parallel.For
来源：http://aye.yangfankeji.com

================================================================================
来源：http://ftk.c1oappe.top

P. 常用工具函数
来源：http://bmi.birdmap.top

================================================================================
来源：http://drp.jyoumei.cn

[P01] 生成 UUID
来源：http://uin.zdqjudy.top

Py:   str(uuid.uuid4())
来源：http://faf.gotoacloud.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rgp.hysaishi.cn

JS:   crypto.randomUUID()
来源：http://urz.smart0.xyz

TS:   crypto.randomUUID()
来源：http://rts.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://yij.xinyue.icu

Go:   // 用 github.com/google/uuid
来源：http://mhc.xinyue.icu

Ruby: SecureRandom.uuid
来源：http://gmj.chenlongwang.top

C#:   Guid.NewGuid().ToString()
来源：http://ecr.jiagoushi.top

[P02] MD5 / SHA256 摘要
来源：http://suh.shangyingyoupin.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ymi.yonumen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yjh.hesvh.cn


<!-- 参考信息 -->