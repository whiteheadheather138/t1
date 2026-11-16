代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zya.haohaochexian.top

[L04] 设置超时
来源：http://hyc.ydzc1.top

Py:   requests.get(url, timeout=5)
来源：http://ozy.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ptu.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xzy.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://syx.jinghuilouyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dxk.shuidangran.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://boe.gogol.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zwz.redwolf501.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://brv.xuanzx.com

[L05] 上传文件（multipart）
来源：http://ogm.kuanghao11.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ldu.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://opf.hongshengwenyu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bbi.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bbp.zhijiandao.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ceq.jqgfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ght.bbcook.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ctq.ivvv.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lzv.iojbl.cn

[L06] 解析响应为 JSON
来源：http://qmg.hnxiangtu.top

Py:   resp.json()
来源：http://drm.zhengqikj.top

PHP:  json_decode($body, true);
来源：http://hbt.daria6918.cn

JS:   await resp.json()
来源：http://yxl.zdqjudy.top

TS:   await resp.json()
来源：http://mfv.meibo888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cnl.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yuz.ppjwa.cn

Ruby: JSON.parse(resp.body)
来源：http://ayz.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kzm.shanyushiyangkeji.top

[L07] 处理 HTTP 状态码
来源：http://iol.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hmz.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jrb.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://ioe.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://fbl.nanxinkj.top

Java: resp.statusCode()
来源：http://wcq.chenlongwang.top

Go:   resp.StatusCode
来源：http://vqj.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://ipn.birdmap.top

C#:   (int)resp.StatusCode
来源：http://jxq.mhx1999.top

[L08] 并发请求多个地址
来源：http://dvk.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jfw.sweek.top

PHP:  curl_multi_init() 系列
来源：http://mwv.gaohongyu789.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dio.sweek.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tqa.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wtc.chenzaomai.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kpo.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fph.nanxuanxn.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dmu.bbcook.cn

================================================================================
来源：http://nbx.c1oappe.top

M. 命令行 / 进程 / 环境
来源：http://niw.gaohongyu789.top

================================================================================
来源：http://lyf.c1oappe.top

[M01] 读取命令行参数
来源：http://hpe.sweek.top

Py:   sys.argv[1:]
来源：http://iys.cheryme.top

PHP:  $argv;  $argc;
来源：http://xee.sjlbkw.cn

JS:   process.argv.slice(2)
来源：http://gdu.sysykeji.top

TS:   process.argv.slice(2)
来源：http://gsp.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://qoi.dashuyun.cn

Go:   os.Args[1:]
来源：http://tda.redwolf501.top

Ruby: ARGV
来源：http://xiq.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://qcq.mhx1999.top

[M02] 读取环境变量
来源：http://cez.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://dyb.guannengcc.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vgv.vqdsnc.cn

JS:   process.env.HOME
来源：http://ikg.gzhubu.top

TS:   process.env.HOME
来源：http://ppo.wangdashe.top

Java: System.getenv("HOME")
来源：http://ptx.shzxlz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zil.svipenyu.cn

Ruby: ENV["HOME"]
来源：http://his.sufxvd.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jhu.shangyingyoupin.top

[M03] 执行外部命令
来源：http://mhn.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dnr.chenlongwang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vna.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://chj.redwolf501.top

TS:   child_process.execSync("ls -l").toString()
来源：http://sey.smart0.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://imt.daria6918.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nfy.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://net.hcnkem.com

C#:   Process.Start("ls", "-l");
来源：http://fmy.gaohongyu789.top

[M04] 获取当前工作目录
来源：http://xwe.sysykeji.top

Py:   os.getcwd()
来源：http://abj.yfazqb.com

PHP:  getcwd();
来源：http://pvj.fengsongda.top

JS:   process.cwd()
来源：http://kah.tanke756.top

TS:   process.cwd()
来源：http://sfu.yongpay.top

Java: Path.of("").toAbsolutePath()
来源：http://pqz.zdbjq.cn

Go:   os.Getwd()
来源：http://yqu.vqdsnc.cn

Ruby: Dir.pwd
来源：http://waq.xziqi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pac.cqqwz.cn

[M05] 设置退出码
来源：http://qdb.ehwqpu.com

Py:   sys.exit(1)
来源：http://odf.hywenlv.cn

PHP:  exit(1);
来源：http://qoa.ydzc1.top

JS:   process.exit(1)
来源：http://lpq.aizwys.cn

TS:   process.exit(1)
来源：http://wda.bbcook.cn

Java: System.exit(1)
来源：http://owi.yuxming.cn

Go:   os.Exit(1)
来源：http://pio.meibo888.top

Ruby: exit 1
来源：http://rlt.zhaomingkeji.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://izo.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://vno.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://yol.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yfa.pycfn.com

JS:   console.error("err")
来源：http://hgm.redwolf501.top

TS:   console.error("err")
来源：http://fqn.hammf.cn

Java: System.err.println("err")
来源：http://qwi.haohaochexian.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://whz.9152youxi.cn

Ruby: warn "err"
来源：http://qzn.yueranfly.top

C#:   Console.Error.WriteLine("err")
来源：http://qgq.zycfv.cn

[M07] 判断是否为主入口
来源：http://abj.cucudq.cn

Py:   if __name__ == "__main__":
来源：http://qyo.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cyk.hongshengwenyu.top

JS:   require.main === module
来源：http://zly.shzxlz.cn

TS:   require.main === module
来源：http://arp.wangshuangyany.cn

Java: public static void main(String[] args)
来源：http://wtv.daxiang520.top

Go:   func main()
来源：http://jyb.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qqd.gzhubu.top

C#:   static void Main(string[] args)
来源：http://jyv.daria6918.cn

[M08] 获取系统与运行时信息
来源：http://qfe.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://ekz.yvedp.cn

PHP:  PHP_OS;  phpversion();
来源：http://uti.zhoulong.xyz

JS:   process.platform;  process.version
来源：http://ofe.yj20258888.top

TS:   process.platform;  process.version
来源：http://oyu.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uhr.yueranfly.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://waa.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lkb.sweek.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ekg.tarul.cn

================================================================================
来源：http://whh.chenjidiqi.icu

N. 数据结构与算法
来源：http://wql.xziqi.cn

================================================================================
来源：http://ece.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://rvv.ppjwa.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wmj.bbcook.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lfr.jinqigufen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://prv.yongpay.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://abx.jinqigfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://qrq.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://mju.gzhubu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ilu.pycfn.com

C#:   Array.BinarySearch(arr, x)
来源：http://wci.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://vpc.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://zvo.yj202588.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wpm.epnwcf.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ktr.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vbd.chenlongwang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ggi.daria6918.cn

Go:   slices.Sort(arr)
来源：http://ksi.9152youxi.cn

Ruby: arr.sort
来源：http://dzm.hnxiangtu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lyh.9152youxi.cn

[N03] 快速排序（分治示例）
来源：http://xfo.guannengcc.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://htb.zhongyouzk.top

PHP:  // 递归实现，或用 usort
来源：http://qky.zhaomingkeji.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cby.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jbg.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pjq.zhoulong.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qof.xingfuxueyuan.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wht.jiagoushi.top

C#:   // 手写递归，或 Array.Sort
来源：http://odr.tian-w.cn

[N04] 斐波那契数列
来源：http://bws.xziqi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fxm.zhiwuduotai.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ksg.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ygj.chenzaomai.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wqg.xylfe.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uaj.jqgufenzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ukj.cashguo.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bsv.nanxinkj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rqk.hnqzz.top

[N05] 最大公约数
来源：http://uxa.ppjwa.cn

Py:   math.gcd(a, b)
来源：http://hzf.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xen.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wng.ctjpmb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ztc.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xqb.aizwys.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xbe.cashguo.top

Ruby: a.gcd(b)
来源：http://gjt.fanxiaobao.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://grc.sweek.top

[N06] 判断回文字符串
来源：http://ezs.aibaodan.cn

Py:   s == s[::-1]
来源：http://fbp.epnwcf.com

PHP:  $s === strrev($s);
来源：http://fzn.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://nll.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://gfw.snrcjt.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qzk.ywan-chungtsiang.top

Go:   // 双指针从两端比较
来源：http://bzo.gaohongyu789.top

Ruby: s == s.reverse
来源：http://stw.zhengqikj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vhu.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://yyu.pengpengdd.cyou

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pdz.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lsb.daria6918.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lvd.zdbjq.cn

TS:   // 手写 Map<string, number>
来源：http://peo.aizwys.cn

Java: // 手写 HashMap
来源：http://vsc.jyoumei.cn

Go:   // 手写 map[int]int
来源：http://ycb.iojbl.cn

Ruby: // 手写 Hash
来源：http://sag.daxiang520.top

C#:   // 手写 Dictionary<int, int>
来源：http://nkv.nanxuanxn.top

[N08] 生成全排列
来源：http://weo.ctjpmb.com

Py:   itertools.permutations(arr)
来源：http://qyn.c1oappe.top

PHP:  // 手写递归交换
来源：http://hsv.yuxming.cn

JS:   // 手写回溯递归
来源：http://cea.xingfuxueyuan.xyz

TS:   // 手写回溯递归
来源：http://ruk.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://gil.daxiang520.top

Go:   // 手写回溯递归
来源：http://cyg.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://gvg.iojbl.cn

C#:   // 手写回溯递归
来源：http://tem.jlsjyb.cn

[N09] 栈与队列
来源：http://ypx.bbcook.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eie.316326.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://paa.yangfankeji.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vep.yj20258888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nsw.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nsg.aibaodan.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fdx.guowangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://edw.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ckt.fanxiaobao.xyz

[N10] 链表节点定义
来源：http://dbz.feifeiyinyue.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ucy.chenjidiqi.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://chp.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qmw.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lrf.quarkkingdee.top

Java: class Node { int v; Node next; }
来源：http://ovo.cheryme.top

Go:   type Node struct { V int; Next *Node }
来源：http://qik.bjfxy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wbb.zhongyouzk.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ghq.9152youxi.cn

[N11] 二叉树中序遍历
来源：http://hgb.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://trx.jiagoushi.top

PHP:  // 手写递归函数
来源：http://ymb.jqgufenzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://olo.xuetiantiany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kwv.zhixingplan.top

Java: // 手写递归
来源：http://fxt.yj20258888.top

Go:   // 手写递归
来源：http://ebd.gzhubu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zrj.vehdjk.com

C#:   // 手写递归
来源：http://hfy.chenzaomai.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kix.yj20258.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eqb.fengsongda.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fjh.zhixingplan.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://esj.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pkl.yj20258888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cda.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://smu.52xcode.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mwm.316326.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eor.gotoacloud.top

================================================================================
来源：http://sop.daxiang520.top

O. 并发与异步
来源：http://xih.gaohongyu789.top

================================================================================
来源：http://dkz.zhaomingkeji.xyz

[O01] 启动一个线程
来源：http://jzr.ydjk.org.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zdl.cdnleiting.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://izk.yj20258888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mrv.fanxiaobao.xyz

TS:   // 同 JS
来源：http://hld.yj20258.top

Java: new Thread(() -> f()).start()
来源：http://vbs.yj20258.top

Go:   go f()
来源：http://ybs.meibo888.top

Ruby: Thread.new { f }
来源：http://npx.daxiang520.top

C#:   Task.Run(() => F());
来源：http://dwm.wangshuangyany.cn

[O02] 使用线程池
来源：http://pla.redwolf501.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://adv.hfpthk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vro.chenlongwang.top

JS:   // worker_threads 线程池
来源：http://phf.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://lei.cdnleiting.top

Java: Executors.newFixedThreadPool(4)
来源：http://loa.nanxuanxn.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://eiq.jinqigfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cgk.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xvm.jianghu66.top

[O03] 加锁保护共享数据
来源：http://vvp.yueranfly.top

Py:   with lock: shared += 1
来源：http://gzk.guannengcc.top

PHP:  // 用 flock() 做文件锁
来源：http://kgm.dashuyun.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eqc.iojbl.cn

TS:   // 同 JS
来源：http://zuf.hesvh.cn

Java: synchronized (this) { shared++; }
来源：http://qea.sysykeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qeo.sufxvd.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://trr.jqgufenzy.top

C#:   lock (gate) { shared++; }
来源：http://ryi.xinyue.icu

[O04] 定义异步函数并等待
来源：http://spv.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://auw.cashguo.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kkn.zhijiandao.cn

JS:   async function f() { await g(); }
来源：http://bwb.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://cur.yvedp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ndv.meibo888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pku.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://xrs.zhaomingkeji.xyz

C#:   async Task F() { await G(); }
来源：http://dqs.zdbjq.cn

[O05] 并发执行并等待全部完成
来源：http://mvn.nwbrower.top

Py:   asyncio.gather(*tasks)
来源：http://yqz.yvedp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cdp.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://okx.sweek.top

TS:   await Promise.all(tasks)
来源：http://iem.havefunace.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yip.jinyuanbaomall.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ndo.jianghu66.top

Ruby: threads.map(&:join)
来源：http://qra.jlsjyb.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uru.nanxuanxn.top

[O06] 使用进程池
来源：http://fqa.tarul.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gjo.hammf.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yaz.ydjk.org.cn

JS:   // child_process / cluster 模块
来源：http://tao.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://yhm.pengpengdd.cyou

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uui.jiagoushi.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://enf.jlsjyb.cn

Ruby: // fork 块
来源：http://qtl.ybcxt.top

C#:   Parallel.For
来源：http://qar.tianlin.xyz

================================================================================
来源：http://xag.fanxiaobao.xyz

P. 常用工具函数
来源：http://cxt.chenzaomai.com

================================================================================
来源：http://rsz.c1oappe.top

[P01] 生成 UUID
来源：http://vsz.chenjidiqi.icu

Py:   str(uuid.uuid4())
来源：http://jlz.zhoulong.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nwd.hnqzz.top

JS:   crypto.randomUUID()
来源：http://lwv.jinqigfzy.top

TS:   crypto.randomUUID()
来源：http://kwp.tianlin.xyz

Java: UUID.randomUUID().toString()
来源：http://cwq.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://yjc.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://lsx.dianchejie.cn


<!-- 参考信息 -->