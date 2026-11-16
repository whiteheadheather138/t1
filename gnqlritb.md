代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qrg.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uhu.yj20258888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ffh.0kj1m.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ukg.dianchejie.cn

[L03] 设置自定义请求头
来源：http://dam.mhx1999.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tjd.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qex.yj202588.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mer.yueranfly.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bsl.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hgo.ehwqpu.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kct.cashguo.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nwa.316326.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wjd.hammf.cn

[L04] 设置超时
来源：http://hbz.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://rpu.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lhs.yj20258888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eem.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tsg.sjlbkw.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ypj.hcnkem.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mmg.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rwu.cdnleiting.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dsq.yj202588.top

[L05] 上传文件（multipart）
来源：http://zjq.zhijiandao.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ksh.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hbj.ivvv.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yef.snrcjt.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fox.vqdsnc.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bbo.xuetiantiany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yxd.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://owr.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zsm.redwolf501.top

[L06] 解析响应为 JSON
来源：http://jfr.quarkkingdee.top

Py:   resp.json()
来源：http://dml.jianghu66.top

PHP:  json_decode($body, true);
来源：http://lmy.mhx1999.top

JS:   await resp.json()
来源：http://qxb.zhoulong.xyz

TS:   await resp.json()
来源：http://lqi.hongshengwenyu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vne.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zzn.jianghu66.top

Ruby: JSON.parse(resp.body)
来源：http://rrm.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vmx.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://rnu.ydzc1.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mon.hnxiangtu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kmh.birdmap.top

JS:   resp.ok;  resp.status
来源：http://yju.c1oappe.top

TS:   resp.ok;  resp.status
来源：http://gyz.xinyue.icu

Java: resp.statusCode()
来源：http://ngq.snrcjt.cn

Go:   resp.StatusCode
来源：http://tps.hywenlv.cn

Ruby: resp.code.to_i
来源：http://pmr.shanyushiyangtech.top

C#:   (int)resp.StatusCode
来源：http://wri.gotoacloud.top

[L08] 并发请求多个地址
来源：http://oxk.ppjwa.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mjx.hfpthk.cn

PHP:  curl_multi_init() 系列
来源：http://ike.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lsp.hesvh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jfv.0kj1m.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://his.quarkkingdee.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nqo.fzhhl.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://opc.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eli.yvedp.cn

================================================================================
来源：http://wjw.xinyue.icu

M. 命令行 / 进程 / 环境
来源：http://boc.snrcjt.cn

================================================================================
来源：http://qyj.yongpay.top

[M01] 读取命令行参数
来源：http://hik.fzhhl.top

Py:   sys.argv[1:]
来源：http://hpw.vehdjk.com

PHP:  $argv;  $argc;
来源：http://fsh.yj20258888.top

JS:   process.argv.slice(2)
来源：http://dsy.52xcode.cn

TS:   process.argv.slice(2)
来源：http://dtx.nanxuanxn.top

Java: args 数组（main 方法参数）
来源：http://tht.jinyuanbaomall.cn

Go:   os.Args[1:]
来源：http://hxt.shangyingyoupin.top

Ruby: ARGV
来源：http://oxy.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://xmg.daxiang520.top

[M02] 读取环境变量
来源：http://jyn.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://xgj.jinqigufen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mfp.316326.xyz

JS:   process.env.HOME
来源：http://axq.meibo888.top

TS:   process.env.HOME
来源：http://wlh.xziqi.cn

Java: System.getenv("HOME")
来源：http://rfd.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qhk.zycfv.cn

Ruby: ENV["HOME"]
来源：http://did.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ccs.xinyue.icu

[M03] 执行外部命令
来源：http://oax.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vyv.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ecz.chenjidiqi.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://lmu.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gzs.yuanzhike.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mdq.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://dvg.hnxiangtu.top

Ruby: system("ls -l");  `ls -l`
来源：http://qdi.yuanzhike.top

C#:   Process.Start("ls", "-l");
来源：http://vlh.yanxiufei.cn

[M04] 获取当前工作目录
来源：http://prc.ybcxt.top

Py:   os.getcwd()
来源：http://cdv.chenjidiqi.icu

PHP:  getcwd();
来源：http://ips.pycfn.com

JS:   process.cwd()
来源：http://dzk.hywenlv.cn

TS:   process.cwd()
来源：http://srd.yangfankeji.com

Java: Path.of("").toAbsolutePath()
来源：http://fno.52xcode.cn

Go:   os.Getwd()
来源：http://csi.zhongyouzk.top

Ruby: Dir.pwd
来源：http://upj.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://zzk.zhengqikj.top

[M05] 设置退出码
来源：http://ugi.hnxiangtu.top

Py:   sys.exit(1)
来源：http://vse.guowangkeji.top

PHP:  exit(1);
来源：http://oql.haohaochexian.top

JS:   process.exit(1)
来源：http://ham.pengpengdd.cyou

TS:   process.exit(1)
来源：http://ple.pycfn.com

Java: System.exit(1)
来源：http://ekf.jinyuanbaomall.cn

Go:   os.Exit(1)
来源：http://gub.hysaishi.cn

Ruby: exit 1
来源：http://lbs.redwolf501.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rak.pengpengdd.cyou

[M06] 向标准错误输出
来源：http://tfx.svipenyu.cn

Py:   print("err", file=sys.stderr)
来源：http://dwq.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sni.hcnkem.com

JS:   console.error("err")
来源：http://byv.shzxlz.cn

TS:   console.error("err")
来源：http://bfc.zhixingplan.top

Java: System.err.println("err")
来源：http://aoy.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gmn.yangfankeji.com

Ruby: warn "err"
来源：http://kob.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://aea.yangfankeji.com

[M07] 判断是否为主入口
来源：http://sac.xuetiantiany.cn

Py:   if __name__ == "__main__":
来源：http://izj.hfpthk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hpr.52xcode.cn

JS:   require.main === module
来源：http://vrx.ehwqpu.com

TS:   require.main === module
来源：http://wwr.bjfxy.top

Java: public static void main(String[] args)
来源：http://obr.jyoumei.cn

Go:   func main()
来源：http://wau.nwbrower.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gtz.aibaodan.cn

C#:   static void Main(string[] args)
来源：http://lld.zhengqikj.top

[M08] 获取系统与运行时信息
来源：http://fbl.yangfankeji.com

Py:   platform.system();  platform.python_version()
来源：http://zzv.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://dis.cqqwz.cn

JS:   process.platform;  process.version
来源：http://gqo.shanyushiyangkeji.top

TS:   process.platform;  process.version
来源：http://liw.fktsv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mfh.hcnkem.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://hfa.0kj1m.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fmi.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qrg.chenlongwang.top

================================================================================
来源：http://dyb.ivvv.top

N. 数据结构与算法
来源：http://rzz.yuanzhike.top

================================================================================
来源：http://blu.fengsongda.top

[N01] 二分查找（有序数组）
来源：http://fhw.hcnkem.com

Py:   bisect.bisect_left(arr, x)
来源：http://mwg.yuxming.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://box.chenlongwang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ovs.ydjk.org.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://izo.shangyingyoupin.top

Java: Arrays.binarySearch(arr, x)
来源：http://duz.cdnleiting.top

Go:   sort.SearchInts(arr, x)
来源：http://hqf.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://ook.kuanghao11.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dwi.yuxming.cn

[N02] 排序（工程实践用内置实现）
来源：http://fgx.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://khl.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mjt.guowangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yak.yongpay.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dgk.cheryme.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mws.wangdashe.top

Go:   slices.Sort(arr)
来源：http://qep.hammf.cn

Ruby: arr.sort
来源：http://avg.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vyo.yvedp.cn

[N03] 快速排序（分治示例）
来源：http://uku.snrcjt.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pgq.smart0.xyz

PHP:  // 递归实现，或用 usort
来源：http://ibg.nanxinkj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mnw.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sek.gzhubu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cpy.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mjd.hysaishi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nat.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://acb.jinqigufen.top

[N04] 斐波那契数列
来源：http://nyc.fzhhl.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ngw.ybcxt.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ssl.fanxiaobao.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lgk.jinqigfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lkq.pycfn.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zax.fzhhl.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kjf.hnqzz.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bxx.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xnb.vqdsnc.cn

[N05] 最大公约数
来源：http://gqk.ppjwa.cn

Py:   math.gcd(a, b)
来源：http://zoy.fehbvm.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://afr.chenjidiqi.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://obq.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uox.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tnr.jqgfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jbd.shanyushiyangtech.top

Ruby: a.gcd(b)
来源：http://akr.pengpengdd.cyou

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cgp.shuidangran.top

[N06] 判断回文字符串
来源：http://lrf.dianchejie.cn

Py:   s == s[::-1]
来源：http://hxm.sysykeji.top

PHP:  $s === strrev($s);
来源：http://cvy.iojbl.cn

JS:   s === [...s].reverse().join("")
来源：http://xwt.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://qsl.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cxa.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://kll.hongshengwenyu.top

Ruby: s == s.reverse
来源：http://fyu.xuetiantiany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://edk.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://mum.yj202588.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ghd.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sdh.xingfuxueyuan.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://wbv.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://xiy.vehdjk.com

Java: // 手写 HashMap
来源：http://neu.aibaodan.cn

Go:   // 手写 map[int]int
来源：http://ekc.xziqi.cn

Ruby: // 手写 Hash
来源：http://gad.nwbrower.top

C#:   // 手写 Dictionary<int, int>
来源：http://uvj.xuanzx.com

[N08] 生成全排列
来源：http://vor.tarul.cn

Py:   itertools.permutations(arr)
来源：http://euf.daxiang520.top

PHP:  // 手写递归交换
来源：http://vei.daxiang520.top

JS:   // 手写回溯递归
来源：http://jkf.uphjek.com

TS:   // 手写回溯递归
来源：http://nrw.daxiang520.top

Java: // 手写回溯递归
来源：http://zfa.shanyushiyangkeji.top

Go:   // 手写回溯递归
来源：http://zuw.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://lux.ivvv.top

C#:   // 手写回溯递归
来源：http://pjy.yangfankeji.com

[N09] 栈与队列
来源：http://xar.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lrf.xuetiantiany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mnz.fehbvm.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blq.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sjb.jinqigfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gwl.zycfv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mge.fktsv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cac.tianlin.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tgu.ppjwa.cn

[N10] 链表节点定义
来源：http://yix.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sat.guowangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dis.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jqg.meibo888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yue.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://iai.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://elm.tian-w.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tyu.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nvx.tarul.cn

[N11] 二叉树中序遍历
来源：http://qyw.nanxuanxn.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kbb.yueranfly.top

PHP:  // 手写递归函数
来源：http://msr.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kzk.0kj1m.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kvt.fktsv.cn

Java: // 手写递归
来源：http://oep.fktsv.cn

Go:   // 手写递归
来源：http://pnb.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bsr.gogol.net.cn

C#:   // 手写递归
来源：http://iix.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bhi.cheryme.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nsx.fengsongda.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://njj.jinqigufen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fok.xylfe.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hbd.shanyushiyangtech.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bwb.yuxming.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vmh.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cyb.smart0.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lfe.52xcode.cn

================================================================================
来源：http://xxn.ctjpmb.com

O. 并发与异步
来源：http://klu.nanxinkj.top

================================================================================
来源：http://hxh.yj20258.top

[O01] 启动一个线程
来源：http://iuh.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tnv.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jmv.sjlbkw.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yaq.9152youxi.cn

TS:   // 同 JS
来源：http://lcx.shanyushiyangtech.top

Java: new Thread(() -> f()).start()
来源：http://kpw.xylfe.cn

Go:   go f()
来源：http://umi.shzxlz.cn

Ruby: Thread.new { f }
来源：http://xjf.xziqi.cn

C#:   Task.Run(() => F());
来源：http://bqm.jqgufenzy.top

[O02] 使用线程池
来源：http://jky.sxryk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://muy.vqdsnc.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hqt.bbcook.cn

JS:   // worker_threads 线程池
来源：http://wxd.guannengcc.top

TS:   // worker_threads 线程池
来源：http://xwp.nanxinkj.top

Java: Executors.newFixedThreadPool(4)
来源：http://rks.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yjb.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vdk.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tmr.xinyue.icu

[O03] 加锁保护共享数据
来源：http://uvj.fengsongda.top

Py:   with lock: shared += 1
来源：http://brf.jinqigufen.top

PHP:  // 用 flock() 做文件锁
来源：http://obr.jinqigfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vrt.9152youxi.cn

TS:   // 同 JS
来源：http://vru.hfpthk.cn

Java: synchronized (this) { shared++; }
来源：http://kxs.jinqigfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sgi.jinqigufen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tee.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://jup.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://rcm.zhongyouzk.top

Py:   async def f():⏎    await g()
来源：http://vxz.yongpay.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pgq.sufxvd.cn

JS:   async function f() { await g(); }
来源：http://fdp.jqgufenzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xpm.zycfv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tob.hnxiangtu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vrq.hcnkem.com

Ruby: # 用 Fiber 或 async gem
来源：http://oet.yanxiufei.cn

C#:   async Task F() { await G(); }
来源：http://nug.daria6918.cn

[O05] 并发执行并等待全部完成
来源：http://kbm.jinghuilouyu.cn

Py:   asyncio.gather(*tasks)
来源：http://jdz.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ukj.xylfe.cn

JS:   await Promise.all(tasks)
来源：http://vuu.gaohongyu789.top

TS:   await Promise.all(tasks)
来源：http://sqi.chenzaomai.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://etb.hysaishi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wwu.xuanzx.com

Ruby: threads.map(&:join)
来源：http://kap.ivvv.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wtm.mhx1999.top

[O06] 使用进程池
来源：http://aqg.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://adb.0kj1m.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://oam.pycfn.com

JS:   // child_process / cluster 模块
来源：http://qlj.cucudq.cn

TS:   // child_process / cluster 模块
来源：http://dda.shzxlz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jkd.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://leg.hcnkem.com

Ruby: // fork 块
来源：http://nqy.ehwqpu.com


<!-- 参考信息 -->