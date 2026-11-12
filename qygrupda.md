代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://oap.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rod.chenzaomai.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iqw.pengpengdd.cyou

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://joy.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://twl.yanxiufei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ssl.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rrf.jianghu66.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jla.jiagoushi.top

[L03] 设置自定义请求头
来源：http://ykz.andypj.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rra.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fph.jinyuanbaomall.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jgs.zhengqikj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://klz.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mqf.shanyushiyangtech.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tvf.zdqjudy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://neg.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://okw.xuanzx.com

[L04] 设置超时
来源：http://xzo.jqgfzy.top

Py:   requests.get(url, timeout=5)
来源：http://jrr.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zdf.wangdashe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pkz.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xnz.xinyue.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vzt.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vzu.sufxvd.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://guv.epnwcf.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ifi.yanxiufei.cn

[L05] 上传文件（multipart）
来源：http://qyn.iojbl.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jgk.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ske.hongshengwenyu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://beb.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eht.hammf.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xco.jyoumei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iqe.fehbvm.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://epb.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://khj.zdbjq.cn

[L06] 解析响应为 JSON
来源：http://efy.hywenlv.cn

Py:   resp.json()
来源：http://yof.sxryk.cn

PHP:  json_decode($body, true);
来源：http://hwk.yongpay.top

JS:   await resp.json()
来源：http://btk.jiagoushi.top

TS:   await resp.json()
来源：http://vwj.zhixingplan.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jsp.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rlz.gogol.net.cn

Ruby: JSON.parse(resp.body)
来源：http://flu.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fcl.nwbrower.top

[L07] 处理 HTTP 状态码
来源：http://eyw.shanyushiyangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dkx.nwbrower.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://abo.cdnleiting.top

JS:   resp.ok;  resp.status
来源：http://wjp.shangyingyoupin.top

TS:   resp.ok;  resp.status
来源：http://lgo.pengpengdd.cyou

Java: resp.statusCode()
来源：http://bsq.sufxvd.cn

Go:   resp.StatusCode
来源：http://fkm.316326.xyz

Ruby: resp.code.to_i
来源：http://vkk.316326.xyz

C#:   (int)resp.StatusCode
来源：http://svn.hnqzz.top

[L08] 并发请求多个地址
来源：http://yhv.iojbl.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ycl.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://bcl.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xel.feifeiyinyue.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pxx.dianchejie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gbf.guannengcc.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sni.shanyushiyangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zvi.daxiang520.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zvg.jqgfzy.top

================================================================================
来源：http://hyp.xuetiantiany.cn

M. 命令行 / 进程 / 环境
来源：http://olz.jinqigufen.top

================================================================================
来源：http://rpt.jinqigufen.top

[M01] 读取命令行参数
来源：http://nqb.316326.xyz

Py:   sys.argv[1:]
来源：http://vgv.yj202588.top

PHP:  $argv;  $argc;
来源：http://cwv.shanyushiyangkeji.top

JS:   process.argv.slice(2)
来源：http://tcl.wangdashe.top

TS:   process.argv.slice(2)
来源：http://vjh.sufxvd.cn

Java: args 数组（main 方法参数）
来源：http://vbc.sysykeji.top

Go:   os.Args[1:]
来源：http://zwp.svipenyu.cn

Ruby: ARGV
来源：http://npm.yongpay.top

C#:   args 数组（Main 方法参数）
来源：http://npf.xylfe.cn

[M02] 读取环境变量
来源：http://cel.yanxiufei.cn

Py:   os.environ.get("HOME")
来源：http://zti.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wtq.zycfv.cn

JS:   process.env.HOME
来源：http://qnl.jinqigufen.top

TS:   process.env.HOME
来源：http://gzf.yonumen.top

Java: System.getenv("HOME")
来源：http://dif.hammf.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nin.jinghuilouyu.cn

Ruby: ENV["HOME"]
来源：http://jvk.ydzc1.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://awg.yongpay.top

[M03] 执行外部命令
来源：http://oxa.jinqigufen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fis.yongpay.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rng.tanke756.top

JS:   child_process.execSync("ls -l").toString()
来源：http://grd.cqqwz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kka.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://szn.vqdsnc.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://omt.zdqjudy.top

Ruby: system("ls -l");  `ls -l`
来源：http://apr.zhijiandao.cn

C#:   Process.Start("ls", "-l");
来源：http://dkn.guannengcc.top

[M04] 获取当前工作目录
来源：http://xxj.52xcode.cn

Py:   os.getcwd()
来源：http://usf.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://lad.hongshengwenyu.top

JS:   process.cwd()
来源：http://phk.yanxiufei.cn

TS:   process.cwd()
来源：http://aet.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://iig.zhiwuduotai.top

Go:   os.Getwd()
来源：http://ypt.xinyue.icu

Ruby: Dir.pwd
来源：http://imz.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tpo.jqgfzy.top

[M05] 设置退出码
来源：http://vnm.aibaodan.cn

Py:   sys.exit(1)
来源：http://qwc.dashuyun.cn

PHP:  exit(1);
来源：http://ipl.fanxiaobao.xyz

JS:   process.exit(1)
来源：http://hbc.pycfn.com

TS:   process.exit(1)
来源：http://haa.nanxuanxn.top

Java: System.exit(1)
来源：http://vbz.zhengqikj.top

Go:   os.Exit(1)
来源：http://lus.pycfn.com

Ruby: exit 1
来源：http://das.bbcook.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wmb.yj202588.top

[M06] 向标准错误输出
来源：http://hkz.sweek.top

Py:   print("err", file=sys.stderr)
来源：http://yhy.yfazqb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://hxv.redwolf501.top

JS:   console.error("err")
来源：http://uux.andypj.xyz

TS:   console.error("err")
来源：http://yhp.chenjidiqi.icu

Java: System.err.println("err")
来源：http://cvd.aibaodan.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ocf.xuanzx.com

Ruby: warn "err"
来源：http://djk.jinqigfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://tgl.jiagoushi.top

[M07] 判断是否为主入口
来源：http://bid.jinqigufen.top

Py:   if __name__ == "__main__":
来源：http://ifl.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lud.xinyue.icu

JS:   require.main === module
来源：http://zzj.yuanzhike.top

TS:   require.main === module
来源：http://odl.fzhhl.top

Java: public static void main(String[] args)
来源：http://ake.birdmap.top

Go:   func main()
来源：http://qza.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wgp.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://gfo.cheryme.top

[M08] 获取系统与运行时信息
来源：http://nwn.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://xed.shzxlz.cn

PHP:  PHP_OS;  phpversion();
来源：http://del.bjfxy.top

JS:   process.platform;  process.version
来源：http://vfm.ydzc1.top

TS:   process.platform;  process.version
来源：http://fev.tanke756.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wpn.9152youxi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yhw.jinqigfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wdu.bjfxy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qzu.nanxuanxn.top

================================================================================
来源：http://lch.ydzc1.top

N. 数据结构与算法
来源：http://nen.sxryk.cn

================================================================================
来源：http://ovv.gogol.net.cn

[N01] 二分查找（有序数组）
来源：http://lnh.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://gtr.zhiwuduotai.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wie.zhongyouzk.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pnm.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zou.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://cqe.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://yug.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hsk.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://stj.sufxvd.cn

[N02] 排序（工程实践用内置实现）
来源：http://rdi.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://jee.hammf.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xdl.yuxming.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jyz.xziqi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://amh.zycfv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://phr.xziqi.cn

Go:   slices.Sort(arr)
来源：http://nhe.chenzaomai.com

Ruby: arr.sort
来源：http://dbe.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bxv.yj20258888.top

[N03] 快速排序（分治示例）
来源：http://lnd.jqgfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vzj.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://psi.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ati.xylfe.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aag.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oio.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uaq.yuxming.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zdn.zycfv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://clu.chenzaomai.com

[N04] 斐波那契数列
来源：http://dak.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gqq.cdnleiting.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://veq.cdnleiting.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://quc.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jnt.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sdn.zdqjudy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zkt.cdnleiting.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ddt.pengpengdd.cyou

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hii.vqdsnc.cn

[N05] 最大公约数
来源：http://ypg.nanxuanxn.top

Py:   math.gcd(a, b)
来源：http://kvh.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jlc.shzxlz.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ocj.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://add.jinyuanbaomall.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qqo.smart0.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bvv.sysykeji.top

Ruby: a.gcd(b)
来源：http://yvv.havefunace.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lse.sweek.top

[N06] 判断回文字符串
来源：http://mkg.quarkkingdee.top

Py:   s == s[::-1]
来源：http://chg.52xcode.cn

PHP:  $s === strrev($s);
来源：http://uby.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://vto.smart0.xyz

TS:   s === [...s].reverse().join("")
来源：http://ilw.svipenyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://urd.jinqigufen.top

Go:   // 双指针从两端比较
来源：http://jct.xylfe.cn

Ruby: s == s.reverse
来源：http://ywl.fzhhl.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nic.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://kmd.mhx1999.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xzt.tian-w.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rtk.xuanzx.com

JS:   // 手写 Map：map.set(v, i)
来源：http://nca.zhoulong.xyz

TS:   // 手写 Map<string, number>
来源：http://btv.guannengcc.top

Java: // 手写 HashMap
来源：http://mhx.andypj.xyz

Go:   // 手写 map[int]int
来源：http://nkb.nanxinkj.top

Ruby: // 手写 Hash
来源：http://fpq.ehwqpu.com

C#:   // 手写 Dictionary<int, int>
来源：http://ppy.yuxming.cn

[N08] 生成全排列
来源：http://giq.sysykeji.top

Py:   itertools.permutations(arr)
来源：http://irs.fzhhl.top

PHP:  // 手写递归交换
来源：http://oof.epnwcf.com

JS:   // 手写回溯递归
来源：http://ugp.hcnkem.com

TS:   // 手写回溯递归
来源：http://uez.ehwqpu.com

Java: // 手写回溯递归
来源：http://ivk.hnxiangtu.top

Go:   // 手写回溯递归
来源：http://pxh.daria6918.cn

Ruby: arr.permutation.to_a
来源：http://lph.vehdjk.com

C#:   // 手写回溯递归
来源：http://ocj.daxiang520.top

[N09] 栈与队列
来源：http://pon.snrcjt.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://njj.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tia.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://exl.xziqi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pyw.ppjwa.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wjh.dashuyun.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rwf.kuanghao11.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rzk.ivvv.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ckr.guowangkeji.top

[N10] 链表节点定义
来源：http://akp.iojbl.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ilb.sysykeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kqq.sufxvd.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zot.chenzaomai.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://arh.yuanzhike.top

Java: class Node { int v; Node next; }
来源：http://aia.bjfxy.top

Go:   type Node struct { V int; Next *Node }
来源：http://wml.tian-w.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vyt.daxiang520.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zth.ydzc1.top

[N11] 二叉树中序遍历
来源：http://wjc.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ran.fanxiaobao.xyz

PHP:  // 手写递归函数
来源：http://xjq.guowangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vsf.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nby.hammf.cn

Java: // 手写递归
来源：http://rqs.guowangkeji.top

Go:   // 手写递归
来源：http://qjb.shanyushiyangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zyh.nanxinkj.top

C#:   // 手写递归
来源：http://bbr.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lpv.jqgufenzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uaa.yuanzhike.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uva.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xxc.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rvi.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nof.aibaodan.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iwz.fanxiaobao.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://prg.chenzaomai.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://swz.jinghuilouyu.cn

================================================================================
来源：http://swz.fzhhl.top

O. 并发与异步
来源：http://swi.sjlbkw.cn

================================================================================
来源：http://gan.pycfn.com

[O01] 启动一个线程
来源：http://wqy.aizwys.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ker.xziqi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kqh.xingfuxueyuan.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rnr.dashuyun.cn

TS:   // 同 JS
来源：http://cpa.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://brm.pycfn.com

Go:   go f()
来源：http://azu.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://ntz.shzxlz.cn

C#:   Task.Run(() => F());
来源：http://khp.quarkkingdee.top

[O02] 使用线程池
来源：http://tqh.cqqwz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baa.nwbrower.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zzc.zhiwuduotai.top

JS:   // worker_threads 线程池
来源：http://ytl.jqgufenzy.top

TS:   // worker_threads 线程池
来源：http://adx.sxryk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qli.tanke756.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bxq.zhengqikj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lot.wangshuangyany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yim.iojbl.cn

[O03] 加锁保护共享数据
来源：http://pfs.jyoumei.cn

Py:   with lock: shared += 1
来源：http://dsn.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ycy.yanxiufei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gnh.birdmap.top

TS:   // 同 JS
来源：http://xba.xingfuxueyuan.xyz

Java: synchronized (this) { shared++; }
来源：http://hhg.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rwi.epnwcf.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://vbb.cheryme.top

C#:   lock (gate) { shared++; }
来源：http://mdv.havefunace.top

[O04] 定义异步函数并等待
来源：http://xwe.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://tbh.jinghuilouyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cxw.yongpay.top

JS:   async function f() { await g(); }
来源：http://kox.zhongyouzk.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://uwm.hammf.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nri.jiagoushi.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://num.0kj1m.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pll.jinqigufen.top

C#:   async Task F() { await G(); }
来源：http://ddm.fehbvm.com

[O05] 并发执行并等待全部完成
来源：http://uyi.meibo888.top

Py:   asyncio.gather(*tasks)
来源：http://grn.aizwys.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://beo.meibo888.top

JS:   await Promise.all(tasks)
来源：http://iqm.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://shu.yj20258888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lmn.sjlbkw.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://paz.shangyingyoupin.top

Ruby: threads.map(&:join)
来源：http://tpv.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qkc.redwolf501.top

[O06] 使用进程池
来源：http://ktp.tian-w.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ejp.jianghu66.top

PHP:  // pcntl_fork 或多进程队列
来源：http://snv.shuidangran.top

JS:   // child_process / cluster 模块
来源：http://tdb.jinghuilouyu.cn


<!-- 参考信息 -->