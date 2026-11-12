代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wpc.zdqjudy.top

[L04] 设置超时
来源：http://rcc.vehdjk.com

Py:   requests.get(url, timeout=5)
来源：http://aaz.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tie.fehbvm.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uei.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ezp.iojbl.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uex.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kqz.fanxiaobao.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bho.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tud.tian-w.cn

[L05] 上传文件（multipart）
来源：http://qjq.mhx1999.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cbc.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pcb.cheryme.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ipm.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aru.yvedp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tsn.nanxinkj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cuf.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pjp.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zzu.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://xqw.fengsongda.top

Py:   resp.json()
来源：http://rbk.snrcjt.cn

PHP:  json_decode($body, true);
来源：http://mkw.mhx1999.top

JS:   await resp.json()
来源：http://iyp.yuanzhike.top

TS:   await resp.json()
来源：http://rtu.zhoulong.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gkd.0kj1m.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nye.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://nwu.wangdashe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://upm.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://pcz.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gql.jinghuilouyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gmu.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://iad.guowangkeji.top

TS:   resp.ok;  resp.status
来源：http://hfn.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://ctc.jqgfzy.top

Go:   resp.StatusCode
来源：http://twl.hammf.cn

Ruby: resp.code.to_i
来源：http://shh.andypj.xyz

C#:   (int)resp.StatusCode
来源：http://mlf.316326.xyz

[L08] 并发请求多个地址
来源：http://dcb.snrcjt.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ltn.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://rta.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ugt.yanxiufei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yqf.meibo888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rvm.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lrq.zhoulong.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qkq.meibo888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cfw.cucudq.cn

================================================================================
来源：http://dnf.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://xfb.smart0.xyz

================================================================================
来源：http://zbv.zdqjudy.top

[M01] 读取命令行参数
来源：http://wwt.haohaochexian.top

Py:   sys.argv[1:]
来源：http://sxt.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://hsn.quarkkingdee.top

JS:   process.argv.slice(2)
来源：http://hkw.meibo888.top

TS:   process.argv.slice(2)
来源：http://qyy.cheryme.top

Java: args 数组（main 方法参数）
来源：http://ldn.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://rxy.0kj1m.cn

Ruby: ARGV
来源：http://saj.vqdsnc.cn

C#:   args 数组（Main 方法参数）
来源：http://dod.chenjidiqi.icu

[M02] 读取环境变量
来源：http://zal.jinyuanbaomall.cn

Py:   os.environ.get("HOME")
来源：http://efx.daxiang520.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gbx.hysaishi.cn

JS:   process.env.HOME
来源：http://sno.yuxming.cn

TS:   process.env.HOME
来源：http://wla.pycfn.com

Java: System.getenv("HOME")
来源：http://xxy.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kwx.bjfxy.top

Ruby: ENV["HOME"]
来源：http://bip.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wsn.jiagoushi.top

[M03] 执行外部命令
来源：http://foc.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xvg.epnwcf.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bru.ydjk.org.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yhg.ydjk.org.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kil.uphjek.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://flr.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dal.dashuyun.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rbd.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://bln.mhx1999.top

[M04] 获取当前工作目录
来源：http://njq.mhx1999.top

Py:   os.getcwd()
来源：http://rqp.c1oappe.top

PHP:  getcwd();
来源：http://uch.chenjidiqi.icu

JS:   process.cwd()
来源：http://gmt.tanke756.top

TS:   process.cwd()
来源：http://fco.wangshuangyany.cn

Java: Path.of("").toAbsolutePath()
来源：http://ave.fanxiaobao.xyz

Go:   os.Getwd()
来源：http://nkh.cucudq.cn

Ruby: Dir.pwd
来源：http://etk.ybcxt.top

C#:   Directory.GetCurrentDirectory()
来源：http://qnj.birdmap.top

[M05] 设置退出码
来源：http://ymz.haohaochexian.top

Py:   sys.exit(1)
来源：http://iim.cashguo.top

PHP:  exit(1);
来源：http://rdt.uphjek.com

JS:   process.exit(1)
来源：http://xrl.zhengqikj.top

TS:   process.exit(1)
来源：http://niw.xinyue.icu

Java: System.exit(1)
来源：http://yfn.gotoacloud.top

Go:   os.Exit(1)
来源：http://yiy.zhoulong.xyz

Ruby: exit 1
来源：http://ebj.mhx1999.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zxz.meibo888.top

[M06] 向标准错误输出
来源：http://xin.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://hdl.kuanghao11.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://njt.cqqwz.cn

JS:   console.error("err")
来源：http://bnh.jiagoushi.top

TS:   console.error("err")
来源：http://ref.yfazqb.com

Java: System.err.println("err")
来源：http://pxc.316326.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pkk.sjlbkw.cn

Ruby: warn "err"
来源：http://xyd.cdnleiting.top

C#:   Console.Error.WriteLine("err")
来源：http://zgn.jiagoushi.top

[M07] 判断是否为主入口
来源：http://scq.meibo888.top

Py:   if __name__ == "__main__":
来源：http://yaj.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iuy.wangshuangyany.cn

JS:   require.main === module
来源：http://fev.mhx1999.top

TS:   require.main === module
来源：http://ivq.hammf.cn

Java: public static void main(String[] args)
来源：http://yyl.sxryk.cn

Go:   func main()
来源：http://hcu.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mxi.yongpay.top

C#:   static void Main(string[] args)
来源：http://gdg.meibo888.top

[M08] 获取系统与运行时信息
来源：http://uni.sysykeji.top

Py:   platform.system();  platform.python_version()
来源：http://wjc.ehwqpu.com

PHP:  PHP_OS;  phpversion();
来源：http://mir.cashguo.top

JS:   process.platform;  process.version
来源：http://pxn.tianlin.xyz

TS:   process.platform;  process.version
来源：http://tkl.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nyn.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rpu.yongpay.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pzs.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://xtq.hnqzz.top

================================================================================
来源：http://igm.quarkkingdee.top

N. 数据结构与算法
来源：http://mha.hysaishi.cn

================================================================================
来源：http://nmy.gogol.net.cn

[N01] 二分查找（有序数组）
来源：http://ywn.ctjpmb.com

Py:   bisect.bisect_left(arr, x)
来源：http://yds.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sxp.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ttt.cdnleiting.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fxr.redwolf501.top

Java: Arrays.binarySearch(arr, x)
来源：http://evy.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://rcm.dianchejie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nvz.xuanzx.com

C#:   Array.BinarySearch(arr, x)
来源：http://fao.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://rog.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://qbn.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ydk.tianlin.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://lds.wangshuangyany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nyq.ppjwa.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://afi.cucudq.cn

Go:   slices.Sort(arr)
来源：http://abo.yj202588.top

Ruby: arr.sort
来源：http://kka.tianlin.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://qxx.xuanzx.com

[N03] 快速排序（分治示例）
来源：http://rnj.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bxr.aibaodan.cn

PHP:  // 递归实现，或用 usort
来源：http://hau.chenjidiqi.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://exw.pengpengdd.cyou

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xkc.yuanzhike.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tzp.jyoumei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jhd.xuetiantiany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pfd.xziqi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://erh.jinghuilouyu.cn

[N04] 斐波那契数列
来源：http://ult.cucudq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ptg.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pnn.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cye.shanyushiyangtech.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ukh.guowangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sba.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tud.meibo888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xaz.tarul.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://acq.wangshuangyany.cn

[N05] 最大公约数
来源：http://fqb.hnxiangtu.top

Py:   math.gcd(a, b)
来源：http://plt.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ouv.bjfxy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ayh.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hck.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kro.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://our.vqdsnc.cn

Ruby: a.gcd(b)
来源：http://jvp.shzxlz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sqt.smart0.xyz

[N06] 判断回文字符串
来源：http://fpl.sjlbkw.cn

Py:   s == s[::-1]
来源：http://fjy.kuanghao11.cn

PHP:  $s === strrev($s);
来源：http://bmw.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://vro.uphjek.com

TS:   s === [...s].reverse().join("")
来源：http://zlr.ydjk.org.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mel.nwbrower.top

Go:   // 双指针从两端比较
来源：http://xfg.vqdsnc.cn

Ruby: s == s.reverse
来源：http://xkf.hnxiangtu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wcw.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://bsr.xinyue.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ixa.sjlbkw.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nnc.yj20258.top

JS:   // 手写 Map：map.set(v, i)
来源：http://grz.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://too.c1oappe.top

Java: // 手写 HashMap
来源：http://dsw.pengpengdd.cyou

Go:   // 手写 map[int]int
来源：http://vzj.jinqigufen.top

Ruby: // 手写 Hash
来源：http://khe.ehwqpu.com

C#:   // 手写 Dictionary<int, int>
来源：http://jan.yj202588.top

[N08] 生成全排列
来源：http://cpg.chenzaomai.com

Py:   itertools.permutations(arr)
来源：http://vci.yonumen.top

PHP:  // 手写递归交换
来源：http://wua.ppjwa.cn

JS:   // 手写回溯递归
来源：http://dyr.hesvh.cn

TS:   // 手写回溯递归
来源：http://xlt.sufxvd.cn

Java: // 手写回溯递归
来源：http://htx.hongshengwenyu.top

Go:   // 手写回溯递归
来源：http://rrn.cheryme.top

Ruby: arr.permutation.to_a
来源：http://jcm.chenjidiqi.icu

C#:   // 手写回溯递归
来源：http://tcn.shanyushiyangtech.top

[N09] 栈与队列
来源：http://fwe.fanxiaobao.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://arl.shangyingyoupin.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xlp.vqdsnc.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xod.hywenlv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uqz.jinqigfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dct.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bfm.jyoumei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uhf.hfpthk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rku.zhijiandao.cn

[N10] 链表节点定义
来源：http://pph.aibaodan.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cov.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ckl.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rvb.andypj.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://egj.hongshengwenyu.top

Java: class Node { int v; Node next; }
来源：http://aqx.zhiwuduotai.top

Go:   type Node struct { V int; Next *Node }
来源：http://jis.gogol.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jpk.feifeiyinyue.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hwy.wangshuangyany.cn

[N11] 二叉树中序遍历
来源：http://xpf.bbcook.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oud.jinyuanbaomall.cn

PHP:  // 手写递归函数
来源：http://azg.ivvv.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jtb.zycfv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fxp.epnwcf.com

Java: // 手写递归
来源：http://hod.jyoumei.cn

Go:   // 手写递归
来源：http://yme.quarkkingdee.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lfu.bbcook.cn

C#:   // 手写递归
来源：http://ebl.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pnv.jqgufenzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yfm.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hvt.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cym.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wfg.meibo888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sqq.sjlbkw.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zkj.guannengcc.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://faq.hysaishi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://esm.ctjpmb.com

================================================================================
来源：http://ape.zhixingplan.top

O. 并发与异步
来源：http://flv.tian-w.cn

================================================================================
来源：http://omg.shanyushiyangtech.top

[O01] 启动一个线程
来源：http://uzf.snrcjt.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fpj.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rea.ydzc1.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wgm.yangfankeji.com

TS:   // 同 JS
来源：http://her.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://ebr.gzhubu.top

Go:   go f()
来源：http://aqn.bbcook.cn

Ruby: Thread.new { f }
来源：http://xka.svipenyu.cn

C#:   Task.Run(() => F());
来源：http://vax.aibaodan.cn

[O02] 使用线程池
来源：http://xyx.svipenyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vbk.cqqwz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ibq.kuanghao11.cn

JS:   // worker_threads 线程池
来源：http://ivq.chenzaomai.com

TS:   // worker_threads 线程池
来源：http://jew.jiagoushi.top

Java: Executors.newFixedThreadPool(4)
来源：http://wdq.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jey.zdqjudy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ofb.zhaomingkeji.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wqd.yongpay.top

[O03] 加锁保护共享数据
来源：http://syg.wangdashe.top

Py:   with lock: shared += 1
来源：http://ceo.cashguo.top

PHP:  // 用 flock() 做文件锁
来源：http://ucn.quarkkingdee.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wvi.gzhubu.top

TS:   // 同 JS
来源：http://agw.vehdjk.com

Java: synchronized (this) { shared++; }
来源：http://qej.yj202588.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qql.hongshengwenyu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://eqs.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://abz.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://irc.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://eaw.dashuyun.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://idd.316326.xyz

JS:   async function f() { await g(); }
来源：http://uem.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wum.yongpay.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eku.fktsv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dnw.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://nxz.yongpay.top

C#:   async Task F() { await G(); }
来源：http://chs.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://tyo.nanxinkj.top

Py:   asyncio.gather(*tasks)
来源：http://xok.shanyushiyangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qaa.xuanzx.com

JS:   await Promise.all(tasks)
来源：http://kol.yuanzhike.top

TS:   await Promise.all(tasks)
来源：http://mzt.hnxiangtu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vgd.guannengcc.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dvq.zdbjq.cn

Ruby: threads.map(&:join)
来源：http://ixx.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://szd.tarul.cn

[O06] 使用进程池
来源：http://vqi.hfpthk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://acs.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hnu.sufxvd.cn

JS:   // child_process / cluster 模块
来源：http://ihw.iojbl.cn

TS:   // child_process / cluster 模块
来源：http://tfm.0kj1m.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qeg.0kj1m.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dfm.epnwcf.com

Ruby: // fork 块
来源：http://sze.cheryme.top

C#:   Parallel.For
来源：http://rjg.wangshuangyany.cn

================================================================================
来源：http://tsq.gaohongyu789.top

P. 常用工具函数
来源：http://cpw.zhongyouzk.top

================================================================================
来源：http://fcw.hnxiangtu.top

[P01] 生成 UUID
来源：http://zrd.meibo888.top

Py:   str(uuid.uuid4())
来源：http://eer.yuxming.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eep.zhengqikj.top

JS:   crypto.randomUUID()
来源：http://mxe.hammf.cn

TS:   crypto.randomUUID()
来源：http://syv.yfazqb.com

Java: UUID.randomUUID().toString()
来源：http://cmh.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://ozv.wangdashe.top

Ruby: SecureRandom.uuid
来源：http://acg.tian-w.cn


<!-- 参考信息 -->