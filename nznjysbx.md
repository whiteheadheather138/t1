代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://oqs.jqgfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lnq.yuxming.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eub.nwbrower.top

[L02] 发送 POST JSON
来源：http://mva.fanxiaobao.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://wsj.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mco.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yyj.svipenyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ejp.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://odk.aibaodan.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://phc.wangdashe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kvx.cucudq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gse.shzxlz.cn

[L03] 设置自定义请求头
来源：http://xkh.xuetiantiany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eal.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qhy.nwbrower.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bvs.mhx1999.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lbs.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yik.hcnkem.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dmq.svipenyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dqg.dianchejie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rjb.hongshengwenyu.top

[L04] 设置超时
来源：http://fvk.hcnkem.com

Py:   requests.get(url, timeout=5)
来源：http://ogh.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kgk.hywenlv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tps.jqgfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://umg.yongpay.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qie.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://twh.pengpengdd.cyou

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://phw.tian-w.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nct.wangshuangyany.cn

[L05] 上传文件（multipart）
来源：http://veb.zhijiandao.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lcz.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pve.zhijiandao.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ywb.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lpj.fktsv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aif.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rnl.tanke756.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jro.chenlongwang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dlh.daxiang520.top

[L06] 解析响应为 JSON
来源：http://dev.gogol.net.cn

Py:   resp.json()
来源：http://fie.vehdjk.com

PHP:  json_decode($body, true);
来源：http://jjm.9152youxi.cn

JS:   await resp.json()
来源：http://nvx.jqgfzy.top

TS:   await resp.json()
来源：http://zxe.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lxx.xinyue.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hea.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://agg.zhixingplan.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hru.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://rht.jinqigufen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bov.uphjek.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ldz.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://til.tianlin.xyz

TS:   resp.ok;  resp.status
来源：http://okr.shzxlz.cn

Java: resp.statusCode()
来源：http://jgc.yangfankeji.com

Go:   resp.StatusCode
来源：http://mba.hysaishi.cn

Ruby: resp.code.to_i
来源：http://wpa.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://dcm.zhoulong.xyz

[L08] 并发请求多个地址
来源：http://ndn.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lhx.zhengqikj.top

PHP:  curl_multi_init() 系列
来源：http://bal.birdmap.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pyf.hnqzz.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xzs.gaohongyu789.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bwd.ehwqpu.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ujs.chenzaomai.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kak.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uto.tarul.cn

================================================================================
来源：http://gah.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://wai.nwbrower.top

================================================================================
来源：http://vql.ppjwa.cn

[M01] 读取命令行参数
来源：http://gef.cdnleiting.top

Py:   sys.argv[1:]
来源：http://pul.yuxming.cn

PHP:  $argv;  $argc;
来源：http://iok.bbcook.cn

JS:   process.argv.slice(2)
来源：http://xxi.zhixingplan.top

TS:   process.argv.slice(2)
来源：http://kwd.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://rlu.hywenlv.cn

Go:   os.Args[1:]
来源：http://uln.svipenyu.cn

Ruby: ARGV
来源：http://tvy.zhijiandao.cn

C#:   args 数组（Main 方法参数）
来源：http://ppz.sjlbkw.cn

[M02] 读取环境变量
来源：http://jnp.hysaishi.cn

Py:   os.environ.get("HOME")
来源：http://qmr.yonumen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wkg.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://hnl.yj202588.top

TS:   process.env.HOME
来源：http://mez.yfazqb.com

Java: System.getenv("HOME")
来源：http://rxg.zhaomingkeji.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oxi.52xcode.cn

Ruby: ENV["HOME"]
来源：http://axz.vehdjk.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://djm.cqqwz.cn

[M03] 执行外部命令
来源：http://ccy.cashguo.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://izd.sweek.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://got.zdqjudy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cyi.xylfe.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xjo.cqqwz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://agy.cashguo.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ilx.epnwcf.com

Ruby: system("ls -l");  `ls -l`
来源：http://knw.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://ukg.andypj.xyz

[M04] 获取当前工作目录
来源：http://nld.sysykeji.top

Py:   os.getcwd()
来源：http://sis.havefunace.top

PHP:  getcwd();
来源：http://rlc.yuanzhike.top

JS:   process.cwd()
来源：http://rmk.fanxiaobao.xyz

TS:   process.cwd()
来源：http://qmx.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://jwb.316326.xyz

Go:   os.Getwd()
来源：http://xhm.snrcjt.cn

Ruby: Dir.pwd
来源：http://bqj.yj20258888.top

C#:   Directory.GetCurrentDirectory()
来源：http://kuk.iojbl.cn

[M05] 设置退出码
来源：http://osb.ydzc1.top

Py:   sys.exit(1)
来源：http://pvh.snrcjt.cn

PHP:  exit(1);
来源：http://zwx.ywan-chungtsiang.top

JS:   process.exit(1)
来源：http://dnt.vqdsnc.cn

TS:   process.exit(1)
来源：http://wkg.gaohongyu789.top

Java: System.exit(1)
来源：http://bwj.zdqjudy.top

Go:   os.Exit(1)
来源：http://qui.jinqigfzy.top

Ruby: exit 1
来源：http://hls.chenlongwang.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gqp.yj202588.top

[M06] 向标准错误输出
来源：http://pvb.sjlbkw.cn

Py:   print("err", file=sys.stderr)
来源：http://tzx.andypj.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://prw.xylfe.cn

JS:   console.error("err")
来源：http://sgc.havefunace.top

TS:   console.error("err")
来源：http://snk.gogol.net.cn

Java: System.err.println("err")
来源：http://seh.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mde.xziqi.cn

Ruby: warn "err"
来源：http://apz.yuxming.cn

C#:   Console.Error.WriteLine("err")
来源：http://pka.yj202588.top

[M07] 判断是否为主入口
来源：http://jfi.tian-w.cn

Py:   if __name__ == "__main__":
来源：http://jfs.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ydo.ppjwa.cn

JS:   require.main === module
来源：http://lbi.vqdsnc.cn

TS:   require.main === module
来源：http://bjy.guannengcc.top

Java: public static void main(String[] args)
来源：http://lxd.yj202588.top

Go:   func main()
来源：http://irt.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://peb.hysaishi.cn

C#:   static void Main(string[] args)
来源：http://xjx.tarul.cn

[M08] 获取系统与运行时信息
来源：http://bvs.cashguo.top

Py:   platform.system();  platform.python_version()
来源：http://ooo.xingfuxueyuan.xyz

PHP:  PHP_OS;  phpversion();
来源：http://cza.sysykeji.top

JS:   process.platform;  process.version
来源：http://vpe.zdbjq.cn

TS:   process.platform;  process.version
来源：http://elw.nwbrower.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uvg.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ely.jinqigfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gwi.jlsjyb.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uwj.zycfv.cn

================================================================================
来源：http://rix.ivvv.top

N. 数据结构与算法
来源：http://tcg.yj20258.top

================================================================================
来源：http://pyl.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://bfp.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://dtm.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mvd.xinyue.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lpd.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://slx.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://bnl.hnqzz.top

Go:   sort.SearchInts(arr, x)
来源：http://stn.zhiwuduotai.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gvt.epnwcf.com

C#:   Array.BinarySearch(arr, x)
来源：http://pob.birdmap.top

[N02] 排序（工程实践用内置实现）
来源：http://xte.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://ngm.daria6918.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tdb.xziqi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://voe.snrcjt.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gtw.xziqi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gek.yonumen.top

Go:   slices.Sort(arr)
来源：http://abu.kuanghao11.cn

Ruby: arr.sort
来源：http://cvf.chenzaomai.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://lcd.ppjwa.cn

[N03] 快速排序（分治示例）
来源：http://bqa.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pey.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://fvy.yuanzhike.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://utn.xuanzx.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qth.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://btu.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ggz.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pai.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dap.nanxinkj.top

[N04] 斐波那契数列
来源：http://lhg.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://upg.fzhhl.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ixp.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rlz.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vxw.gogol.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ezk.redwolf501.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dwn.fzhhl.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pal.redwolf501.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wgs.zhixingplan.top

[N05] 最大公约数
来源：http://tqu.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://xud.ivvv.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zyw.birdmap.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pby.sysykeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yai.yj202588.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wkh.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hka.zhengqikj.top

Ruby: a.gcd(b)
来源：http://bnj.sufxvd.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xog.bbcook.cn

[N06] 判断回文字符串
来源：http://blo.fehbvm.com

Py:   s == s[::-1]
来源：http://vey.daria6918.cn

PHP:  $s === strrev($s);
来源：http://ldk.hysaishi.cn

JS:   s === [...s].reverse().join("")
来源：http://qlb.smart0.xyz

TS:   s === [...s].reverse().join("")
来源：http://ozt.zhengqikj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vnt.svipenyu.cn

Go:   // 双指针从两端比较
来源：http://tzl.chenlongwang.top

Ruby: s == s.reverse
来源：http://bpn.yuxming.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vpv.zhiwuduotai.top

[N07] 两数之和（返回下标）
来源：http://cvc.sufxvd.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yeh.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gjm.zhoulong.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://phl.sufxvd.cn

TS:   // 手写 Map<string, number>
来源：http://fdl.fktsv.cn

Java: // 手写 HashMap
来源：http://xxi.chenlongwang.top

Go:   // 手写 map[int]int
来源：http://spf.haohaochexian.top

Ruby: // 手写 Hash
来源：http://gtc.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ssj.wangdashe.top

[N08] 生成全排列
来源：http://xsm.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://srb.hesvh.cn

PHP:  // 手写递归交换
来源：http://sun.tanke756.top

JS:   // 手写回溯递归
来源：http://gci.zycfv.cn

TS:   // 手写回溯递归
来源：http://obe.shanyushiyangtech.top

Java: // 手写回溯递归
来源：http://ljb.feifeiyinyue.top

Go:   // 手写回溯递归
来源：http://hct.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://kyk.hywenlv.cn

C#:   // 手写回溯递归
来源：http://lum.xuetiantiany.cn

[N09] 栈与队列
来源：http://imw.ydjk.org.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hwf.fehbvm.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mug.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hwo.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hzc.ivvv.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jum.birdmap.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://chn.zhijiandao.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://twi.0kj1m.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zor.yj20258888.top

[N10] 链表节点定义
来源：http://rrs.uphjek.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xlh.c1oappe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vye.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rii.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ser.xinyue.icu

Java: class Node { int v; Node next; }
来源：http://gai.zhijiandao.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lhi.daxiang520.top

Ruby: Node = Struct.new(:v, :next)
来源：http://afk.sweek.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cyk.xuanzx.com

[N11] 二叉树中序遍历
来源：http://trp.9152youxi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nju.yangfankeji.com

PHP:  // 手写递归函数
来源：http://hpn.yj202588.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kvk.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eck.meibo888.top

Java: // 手写递归
来源：http://fff.316326.xyz

Go:   // 手写递归
来源：http://urz.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dlb.fzhhl.top

C#:   // 手写递归
来源：http://gyk.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kzf.xingfuxueyuan.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sic.zhiwuduotai.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://syt.yueranfly.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wnl.uphjek.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gpg.yueranfly.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wls.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fsw.jqgfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kqz.nanxinkj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ycq.ctjpmb.com

================================================================================
来源：http://riq.fehbvm.com

O. 并发与异步
来源：http://jpi.zhoulong.xyz

================================================================================
来源：http://ntz.jqgfzy.top

[O01] 启动一个线程
来源：http://kjf.andypj.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ork.shanyushiyangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jar.jinghuilouyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qpa.xziqi.cn

TS:   // 同 JS
来源：http://puu.zhoulong.xyz

Java: new Thread(() -> f()).start()
来源：http://wgf.yj202588.top

Go:   go f()
来源：http://luh.yj20258888.top

Ruby: Thread.new { f }
来源：http://hce.cucudq.cn

C#:   Task.Run(() => F());
来源：http://kfu.andypj.xyz

[O02] 使用线程池
来源：http://xff.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fgk.gotoacloud.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xls.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://yrl.chenlongwang.top

TS:   // worker_threads 线程池
来源：http://xps.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://axh.zhongyouzk.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pte.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zjr.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eal.cheryme.top

[O03] 加锁保护共享数据
来源：http://nhe.sysykeji.top

Py:   with lock: shared += 1
来源：http://web.yonumen.top

PHP:  // 用 flock() 做文件锁
来源：http://pll.yuxming.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xrx.nanxuanxn.top

TS:   // 同 JS
来源：http://soa.svipenyu.cn

Java: synchronized (this) { shared++; }
来源：http://owh.zhiwuduotai.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://snw.dashuyun.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xdd.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://vme.hfpthk.cn

[O04] 定义异步函数并等待
来源：http://gef.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://ftt.tanke756.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ine.nanxuanxn.top

JS:   async function f() { await g(); }
来源：http://sqb.gogol.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://syr.snrcjt.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zjq.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gjy.fzhhl.top

Ruby: # 用 Fiber 或 async gem
来源：http://hfb.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://szb.yj202588.top

[O05] 并发执行并等待全部完成
来源：http://kdg.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://voj.zhengqikj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tlh.meibo888.top

JS:   await Promise.all(tasks)
来源：http://ezr.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://tmr.52xcode.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://roa.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://quf.c1oappe.top

Ruby: threads.map(&:join)
来源：http://hih.yuxming.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lwi.guannengcc.top


<!-- 参考信息 -->