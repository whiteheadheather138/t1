代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rua.feifeiyinyue.top

[L04] 设置超时
来源：http://vtt.dianchejie.cn

Py:   requests.get(url, timeout=5)
来源：http://fvq.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cxm.birdmap.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mdo.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lik.bjfxy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tcl.iojbl.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://beu.chenlongwang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vru.yonumen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://maa.cashguo.top

[L05] 上传文件（multipart）
来源：http://caw.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jyc.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mtc.fehbvm.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qfe.zycfv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://add.sysykeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jnu.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hew.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lci.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dhj.hammf.cn

[L06] 解析响应为 JSON
来源：http://exk.hammf.cn

Py:   resp.json()
来源：http://vze.xuanzx.com

PHP:  json_decode($body, true);
来源：http://xuw.xylfe.cn

JS:   await resp.json()
来源：http://rgy.ybcxt.top

TS:   await resp.json()
来源：http://dju.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fma.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tbu.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://bqw.sxryk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gnx.zdbjq.cn

[L07] 处理 HTTP 状态码
来源：http://kqe.jinqigufen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ure.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mea.cdnleiting.top

JS:   resp.ok;  resp.status
来源：http://mdd.tianlin.xyz

TS:   resp.ok;  resp.status
来源：http://hkr.ppjwa.cn

Java: resp.statusCode()
来源：http://qke.nwbrower.top

Go:   resp.StatusCode
来源：http://dvm.svipenyu.cn

Ruby: resp.code.to_i
来源：http://nut.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://sxy.sysykeji.top

[L08] 并发请求多个地址
来源：http://qke.ywan-chungtsiang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nof.yfazqb.com

PHP:  curl_multi_init() 系列
来源：http://oaq.aibaodan.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xdh.xingfuxueyuan.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nlo.jlsjyb.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bof.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pkk.hesvh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mih.ehwqpu.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tqo.jqgfzy.top

================================================================================
来源：http://vpu.hcnkem.com

M. 命令行 / 进程 / 环境
来源：http://ppr.nanxinkj.top

================================================================================
来源：http://sbs.yuanzhike.top

[M01] 读取命令行参数
来源：http://zuw.zdqjudy.top

Py:   sys.argv[1:]
来源：http://uef.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://peo.zycfv.cn

JS:   process.argv.slice(2)
来源：http://trs.shuidangran.top

TS:   process.argv.slice(2)
来源：http://yod.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://twb.c1oappe.top

Go:   os.Args[1:]
来源：http://wli.hysaishi.cn

Ruby: ARGV
来源：http://usk.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://jar.redwolf501.top

[M02] 读取环境变量
来源：http://njm.aibaodan.cn

Py:   os.environ.get("HOME")
来源：http://bfl.zdqjudy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tcv.hesvh.cn

JS:   process.env.HOME
来源：http://slo.wangdashe.top

TS:   process.env.HOME
来源：http://eex.yfazqb.com

Java: System.getenv("HOME")
来源：http://kuh.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rqc.vehdjk.com

Ruby: ENV["HOME"]
来源：http://jyn.bjfxy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kbo.shuidangran.top

[M03] 执行外部命令
来源：http://qod.ydjk.org.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://akx.fktsv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bvv.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cjp.zdqjudy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://klp.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eha.sweek.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hvf.dashuyun.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xbe.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://lzn.cdnleiting.top

[M04] 获取当前工作目录
来源：http://uym.aibaodan.cn

Py:   os.getcwd()
来源：http://zbt.zdqjudy.top

PHP:  getcwd();
来源：http://zoi.quarkkingdee.top

JS:   process.cwd()
来源：http://yeg.yj20258888.top

TS:   process.cwd()
来源：http://wav.ydjk.org.cn

Java: Path.of("").toAbsolutePath()
来源：http://yus.cucudq.cn

Go:   os.Getwd()
来源：http://sox.yj202588.top

Ruby: Dir.pwd
来源：http://sxi.hesvh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rls.tian-w.cn

[M05] 设置退出码
来源：http://gyl.birdmap.top

Py:   sys.exit(1)
来源：http://gpk.hesvh.cn

PHP:  exit(1);
来源：http://llo.hesvh.cn

JS:   process.exit(1)
来源：http://bns.dianchejie.cn

TS:   process.exit(1)
来源：http://rax.yvedp.cn

Java: System.exit(1)
来源：http://dtc.hywenlv.cn

Go:   os.Exit(1)
来源：http://ltc.iojbl.cn

Ruby: exit 1
来源：http://bcz.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://klu.zhiwuduotai.top

[M06] 向标准错误输出
来源：http://epr.cqqwz.cn

Py:   print("err", file=sys.stderr)
来源：http://rfg.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kcu.ywan-chungtsiang.top

JS:   console.error("err")
来源：http://hhm.hnxiangtu.top

TS:   console.error("err")
来源：http://xdi.redwolf501.top

Java: System.err.println("err")
来源：http://bdf.bjfxy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kke.zhongyouzk.top

Ruby: warn "err"
来源：http://vdx.gzhubu.top

C#:   Console.Error.WriteLine("err")
来源：http://szp.fengsongda.top

[M07] 判断是否为主入口
来源：http://rsb.316326.xyz

Py:   if __name__ == "__main__":
来源：http://aek.ywan-chungtsiang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pnk.cucudq.cn

JS:   require.main === module
来源：http://ker.cdnleiting.top

TS:   require.main === module
来源：http://ogu.shuidangran.top

Java: public static void main(String[] args)
来源：http://dzt.hongshengwenyu.top

Go:   func main()
来源：http://ebg.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xvr.xziqi.cn

C#:   static void Main(string[] args)
来源：http://vwu.hesvh.cn

[M08] 获取系统与运行时信息
来源：http://caj.0kj1m.cn

Py:   platform.system();  platform.python_version()
来源：http://iaq.jqgfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://buz.chenlongwang.top

JS:   process.platform;  process.version
来源：http://mkz.zdqjudy.top

TS:   process.platform;  process.version
来源：http://ioe.9152youxi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fhi.tian-w.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://igz.epnwcf.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vbo.hysaishi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yif.pycfn.com

================================================================================
来源：http://baa.gzhubu.top

N. 数据结构与算法
来源：http://kcd.jqgfzy.top

================================================================================
来源：http://oyo.ybcxt.top

[N01] 二分查找（有序数组）
来源：http://vyq.sufxvd.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mhg.0kj1m.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yin.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://moo.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ryh.xuetiantiany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qzt.bjfxy.top

Go:   sort.SearchInts(arr, x)
来源：http://wwk.zycfv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://osp.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://mqb.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://vbe.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://fjw.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gwi.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fyw.sweek.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rzr.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://reh.dashuyun.cn

Go:   slices.Sort(arr)
来源：http://ulf.snrcjt.cn

Ruby: arr.sort
来源：http://scz.svipenyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://crv.svipenyu.cn

[N03] 快速排序（分治示例）
来源：http://prc.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zue.cheryme.top

PHP:  // 递归实现，或用 usort
来源：http://uwn.hnqzz.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zwn.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cpo.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bux.ivvv.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dfs.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ruh.hongshengwenyu.top

C#:   // 手写递归，或 Array.Sort
来源：http://njd.cqqwz.cn

[N04] 斐波那契数列
来源：http://pei.cheryme.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fwe.52xcode.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pdp.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dzn.cashguo.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ovt.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://weo.cqqwz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uls.fehbvm.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bnl.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lri.xziqi.cn

[N05] 最大公约数
来源：http://hzt.xinyue.icu

Py:   math.gcd(a, b)
来源：http://lxu.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vel.nanxinkj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wnb.tianlin.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://soa.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://huo.havefunace.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xko.dashuyun.cn

Ruby: a.gcd(b)
来源：http://tkw.yanxiufei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jza.guannengcc.top

[N06] 判断回文字符串
来源：http://qsl.ehwqpu.com

Py:   s == s[::-1]
来源：http://icr.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://mov.cucudq.cn

JS:   s === [...s].reverse().join("")
来源：http://ibn.sufxvd.cn

TS:   s === [...s].reverse().join("")
来源：http://tev.ehwqpu.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ote.0kj1m.cn

Go:   // 双指针从两端比较
来源：http://qqy.zhiwuduotai.top

Ruby: s == s.reverse
来源：http://beo.fehbvm.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://urj.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://fcp.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bdc.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xdw.tarul.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ylm.iojbl.cn

TS:   // 手写 Map<string, number>
来源：http://jyc.cheryme.top

Java: // 手写 HashMap
来源：http://kqa.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://izf.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://qsw.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://zuy.bjfxy.top

[N08] 生成全排列
来源：http://bzi.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://idr.smart0.xyz

PHP:  // 手写递归交换
来源：http://cie.yvedp.cn

JS:   // 手写回溯递归
来源：http://zcm.ydjk.org.cn

TS:   // 手写回溯递归
来源：http://juf.fzhhl.top

Java: // 手写回溯递归
来源：http://wmo.gogol.net.cn

Go:   // 手写回溯递归
来源：http://mpl.ydzc1.top

Ruby: arr.permutation.to_a
来源：http://gmn.zdbjq.cn

C#:   // 手写回溯递归
来源：http://fxi.kuanghao11.cn

[N09] 栈与队列
来源：http://rrs.xinyue.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xlb.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nwj.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nqj.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://faf.shangyingyoupin.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://goi.aibaodan.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://woo.cdnleiting.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://frh.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nrr.xuetiantiany.cn

[N10] 链表节点定义
来源：http://cpm.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ucf.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://igv.iojbl.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ioi.jqgfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vzi.yonumen.top

Java: class Node { int v; Node next; }
来源：http://ovr.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://stw.daria6918.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jqp.bbcook.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ysk.birdmap.top

[N11] 二叉树中序遍历
来源：http://qeh.jqgfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yfm.fktsv.cn

PHP:  // 手写递归函数
来源：http://bzu.iojbl.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tal.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hlo.sweek.top

Java: // 手写递归
来源：http://hki.fanxiaobao.xyz

Go:   // 手写递归
来源：http://omt.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zyd.aibaodan.cn

C#:   // 手写递归
来源：http://kcr.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kuj.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aee.tarul.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lfo.hywenlv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://svs.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rlk.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rvh.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hxq.yanxiufei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mvl.tanke756.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kze.sxryk.cn

================================================================================
来源：http://onk.vqdsnc.cn

O. 并发与异步
来源：http://hru.sufxvd.cn

================================================================================
来源：http://mxr.bjfxy.top

[O01] 启动一个线程
来源：http://wfa.nwbrower.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bjx.52xcode.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vko.hnxiangtu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pdu.gogol.net.cn

TS:   // 同 JS
来源：http://pkf.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://prr.yongpay.top

Go:   go f()
来源：http://ute.smart0.xyz

Ruby: Thread.new { f }
来源：http://axi.birdmap.top

C#:   Task.Run(() => F());
来源：http://lfv.pengpengdd.cyou

[O02] 使用线程池
来源：http://fjv.birdmap.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hfl.jinyuanbaomall.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://erb.jinghuilouyu.cn

JS:   // worker_threads 线程池
来源：http://bru.xingfuxueyuan.xyz

TS:   // worker_threads 线程池
来源：http://qfz.yangfankeji.com

Java: Executors.newFixedThreadPool(4)
来源：http://hxb.zhengqikj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dme.hnxiangtu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nem.zdqjudy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vjr.pycfn.com

[O03] 加锁保护共享数据
来源：http://lru.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://xlj.jinyuanbaomall.cn

PHP:  // 用 flock() 做文件锁
来源：http://ozb.uphjek.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cok.epnwcf.com

TS:   // 同 JS
来源：http://gke.sjlbkw.cn

Java: synchronized (this) { shared++; }
来源：http://aly.fzhhl.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hhg.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zkq.mhx1999.top

C#:   lock (gate) { shared++; }
来源：http://onl.birdmap.top

[O04] 定义异步函数并等待
来源：http://gjy.jianghu66.top

Py:   async def f():⏎    await g()
来源：http://tsz.shzxlz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dhk.redwolf501.top

JS:   async function f() { await g(); }
来源：http://bln.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://blk.316326.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mpa.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://khk.hammf.cn

Ruby: # 用 Fiber 或 async gem
来源：http://coz.daxiang520.top

C#:   async Task F() { await G(); }
来源：http://lkl.zhengqikj.top

[O05] 并发执行并等待全部完成
来源：http://whh.xuetiantiany.cn

Py:   asyncio.gather(*tasks)
来源：http://wzv.bbcook.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bhl.dianchejie.cn

JS:   await Promise.all(tasks)
来源：http://ave.zhixingplan.top

TS:   await Promise.all(tasks)
来源：http://wda.dashuyun.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zas.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vqo.zhoulong.xyz

Ruby: threads.map(&:join)
来源：http://nhw.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rwb.yj20258888.top

[O06] 使用进程池
来源：http://rzm.andypj.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mlp.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uwi.xylfe.cn

JS:   // child_process / cluster 模块
来源：http://csk.jqgfzy.top

TS:   // child_process / cluster 模块
来源：http://sik.daxiang520.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://djc.gogol.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yrs.zhongyouzk.top

Ruby: // fork 块
来源：http://qbe.zhongyouzk.top

C#:   Parallel.For
来源：http://ihn.zhongyouzk.top

================================================================================
来源：http://fvo.9152youxi.cn

P. 常用工具函数
来源：http://zmd.kuanghao11.cn

================================================================================
来源：http://qbj.iojbl.cn

[P01] 生成 UUID
来源：http://vwt.ppjwa.cn

Py:   str(uuid.uuid4())
来源：http://vtl.yueranfly.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://she.shanyushiyangkeji.top

JS:   crypto.randomUUID()
来源：http://pvq.dashuyun.cn

TS:   crypto.randomUUID()
来源：http://wjg.sysykeji.top

Java: UUID.randomUUID().toString()
来源：http://xpg.dianchejie.cn

Go:   // 用 github.com/google/uuid
来源：http://omi.shanyushiyangkeji.top

Ruby: SecureRandom.uuid
来源：http://wqf.andypj.xyz


<!-- 参考信息 -->