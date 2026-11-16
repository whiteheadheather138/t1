代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://tkz.dashuyun.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qyu.hfpthk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iqp.xingfuxueyuan.xyz

[L02] 发送 POST JSON
来源：http://nxh.xylfe.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zgt.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vvf.daria6918.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uda.xziqi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qko.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fri.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uiu.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rwg.gotoacloud.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ixx.yonumen.top

[L03] 设置自定义请求头
来源：http://oli.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://puv.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yjz.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jpz.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ewh.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mmg.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wrg.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://izw.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sae.aibaodan.cn

[L04] 设置超时
来源：http://qdw.sjlbkw.cn

Py:   requests.get(url, timeout=5)
来源：http://hxi.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lea.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eyw.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tis.uphjek.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qpn.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xds.vehdjk.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gyq.aibaodan.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://heu.xuanzx.com

[L05] 上传文件（multipart）
来源：http://ihy.jiagoushi.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mad.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uth.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xpm.snrcjt.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aen.tanke756.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fii.shanyushiyangtech.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bpa.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lye.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ves.fengsongda.top

[L06] 解析响应为 JSON
来源：http://zax.cqqwz.cn

Py:   resp.json()
来源：http://uer.zycfv.cn

PHP:  json_decode($body, true);
来源：http://ltq.zhixingplan.top

JS:   await resp.json()
来源：http://qgj.jiagoushi.top

TS:   await resp.json()
来源：http://sjb.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mmf.zhoulong.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ahm.feifeiyinyue.top

Ruby: JSON.parse(resp.body)
来源：http://oif.daxiang520.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ctb.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://xxk.ybcxt.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ski.daxiang520.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://siq.tanke756.top

JS:   resp.ok;  resp.status
来源：http://ucf.sysykeji.top

TS:   resp.ok;  resp.status
来源：http://pyc.wangshuangyany.cn

Java: resp.statusCode()
来源：http://iuh.cheryme.top

Go:   resp.StatusCode
来源：http://kwe.bbcook.cn

Ruby: resp.code.to_i
来源：http://mwd.gotoacloud.top

C#:   (int)resp.StatusCode
来源：http://guy.chenjidiqi.icu

[L08] 并发请求多个地址
来源：http://ymn.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ppx.tian-w.cn

PHP:  curl_multi_init() 系列
来源：http://vwo.hammf.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kqo.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ipt.zhoulong.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wqa.shangyingyoupin.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://heh.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rrx.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zsa.yj20258.top

================================================================================
来源：http://wri.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://rhm.zdbjq.cn

================================================================================
来源：http://mwi.fehbvm.com

[M01] 读取命令行参数
来源：http://vme.smart0.xyz

Py:   sys.argv[1:]
来源：http://hjo.snrcjt.cn

PHP:  $argv;  $argc;
来源：http://acy.aibaodan.cn

JS:   process.argv.slice(2)
来源：http://qud.fanxiaobao.xyz

TS:   process.argv.slice(2)
来源：http://cfp.ppjwa.cn

Java: args 数组（main 方法参数）
来源：http://efu.yj202588.top

Go:   os.Args[1:]
来源：http://dkb.quarkkingdee.top

Ruby: ARGV
来源：http://ekw.andypj.xyz

C#:   args 数组（Main 方法参数）
来源：http://rza.iojbl.cn

[M02] 读取环境变量
来源：http://exz.zdbjq.cn

Py:   os.environ.get("HOME")
来源：http://uqp.jqgufenzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jpi.0kj1m.cn

JS:   process.env.HOME
来源：http://ehh.smart0.xyz

TS:   process.env.HOME
来源：http://hdy.ivvv.top

Java: System.getenv("HOME")
来源：http://skp.fengsongda.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xid.zhaomingkeji.xyz

Ruby: ENV["HOME"]
来源：http://uay.yj20258888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kuu.jianghu66.top

[M03] 执行外部命令
来源：http://isc.snrcjt.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cej.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bgd.dianchejie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://neo.chenjidiqi.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://jxm.smart0.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ajf.xuanzx.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ugh.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://amr.gaohongyu789.top

C#:   Process.Start("ls", "-l");
来源：http://wcv.zdbjq.cn

[M04] 获取当前工作目录
来源：http://ltq.xziqi.cn

Py:   os.getcwd()
来源：http://tzv.yuxming.cn

PHP:  getcwd();
来源：http://eag.ctjpmb.com

JS:   process.cwd()
来源：http://hka.ppjwa.cn

TS:   process.cwd()
来源：http://mzp.chenjidiqi.icu

Java: Path.of("").toAbsolutePath()
来源：http://yyp.0kj1m.cn

Go:   os.Getwd()
来源：http://pww.hongshengwenyu.top

Ruby: Dir.pwd
来源：http://vvw.birdmap.top

C#:   Directory.GetCurrentDirectory()
来源：http://gbb.316326.xyz

[M05] 设置退出码
来源：http://yzg.jinyuanbaomall.cn

Py:   sys.exit(1)
来源：http://fkg.zdbjq.cn

PHP:  exit(1);
来源：http://gdj.sxryk.cn

JS:   process.exit(1)
来源：http://umo.9152youxi.cn

TS:   process.exit(1)
来源：http://leh.sufxvd.cn

Java: System.exit(1)
来源：http://wxb.zycfv.cn

Go:   os.Exit(1)
来源：http://eop.bbcook.cn

Ruby: exit 1
来源：http://pvp.52xcode.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://swb.feifeiyinyue.top

[M06] 向标准错误输出
来源：http://zwk.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://szr.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kkl.zhongyouzk.top

JS:   console.error("err")
来源：http://jmo.fanxiaobao.xyz

TS:   console.error("err")
来源：http://ohb.wangdashe.top

Java: System.err.println("err")
来源：http://fze.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hrk.yvedp.cn

Ruby: warn "err"
来源：http://nzu.yfazqb.com

C#:   Console.Error.WriteLine("err")
来源：http://ezh.aizwys.cn

[M07] 判断是否为主入口
来源：http://buh.kuanghao11.cn

Py:   if __name__ == "__main__":
来源：http://gjj.epnwcf.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qhm.zhixingplan.top

JS:   require.main === module
来源：http://ier.yj20258.top

TS:   require.main === module
来源：http://owl.chenzaomai.com

Java: public static void main(String[] args)
来源：http://pok.tianlin.xyz

Go:   func main()
来源：http://rle.wangshuangyany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://avg.fehbvm.com

C#:   static void Main(string[] args)
来源：http://nkz.shangyingyoupin.top

[M08] 获取系统与运行时信息
来源：http://qod.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://fsk.ydjk.org.cn

PHP:  PHP_OS;  phpversion();
来源：http://pxl.meibo888.top

JS:   process.platform;  process.version
来源：http://mhh.quarkkingdee.top

TS:   process.platform;  process.version
来源：http://glf.cashguo.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://atc.ydjk.org.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dyv.sxryk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cgb.ctjpmb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://iib.sjlbkw.cn

================================================================================
来源：http://ifi.chenjidiqi.icu

N. 数据结构与算法
来源：http://ayd.gotoacloud.top

================================================================================
来源：http://jhj.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://kvp.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://vgb.feifeiyinyue.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pkz.cdnleiting.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://alb.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bfi.ywan-chungtsiang.top

Java: Arrays.binarySearch(arr, x)
来源：http://yjf.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://tdw.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yea.9152youxi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oow.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://mgf.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://wdx.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://euy.birdmap.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://skt.hnxiangtu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jek.fanxiaobao.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ile.ydjk.org.cn

Go:   slices.Sort(arr)
来源：http://mmv.svipenyu.cn

Ruby: arr.sort
来源：http://umf.yvedp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://boa.guannengcc.top

[N03] 快速排序（分治示例）
来源：http://hvp.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vcm.smart0.xyz

PHP:  // 递归实现，或用 usort
来源：http://lxn.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rwq.dashuyun.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rqz.sxryk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vot.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bxe.guowangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lgo.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rhg.yangfankeji.com

[N04] 斐波那契数列
来源：http://jnz.zdqjudy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://leh.hysaishi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://syz.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kri.fanxiaobao.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://khi.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zad.yongpay.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vvg.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lzq.hfpthk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cwc.yj20258.top

[N05] 最大公约数
来源：http://yyc.cqqwz.cn

Py:   math.gcd(a, b)
来源：http://ont.hnqzz.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ktw.ehwqpu.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ejm.aizwys.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hzm.hywenlv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://buc.nwbrower.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mkj.hywenlv.cn

Ruby: a.gcd(b)
来源：http://dvd.zhixingplan.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bpm.ehwqpu.com

[N06] 判断回文字符串
来源：http://nwl.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://yvb.hnqzz.top

PHP:  $s === strrev($s);
来源：http://jah.xylfe.cn

JS:   s === [...s].reverse().join("")
来源：http://icz.jinqigufen.top

TS:   s === [...s].reverse().join("")
来源：http://ype.hysaishi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://npg.smart0.xyz

Go:   // 双指针从两端比较
来源：http://jmc.jinghuilouyu.cn

Ruby: s == s.reverse
来源：http://exm.nwbrower.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mbu.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://mph.chenlongwang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ttu.c1oappe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qql.redwolf501.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jam.yuanzhike.top

TS:   // 手写 Map<string, number>
来源：http://kkq.dianchejie.cn

Java: // 手写 HashMap
来源：http://yck.yj20258888.top

Go:   // 手写 map[int]int
来源：http://xbd.aizwys.cn

Ruby: // 手写 Hash
来源：http://nhq.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://yok.smart0.xyz

[N08] 生成全排列
来源：http://cps.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://lio.jiagoushi.top

PHP:  // 手写递归交换
来源：http://hls.shuidangran.top

JS:   // 手写回溯递归
来源：http://nve.jinyuanbaomall.cn

TS:   // 手写回溯递归
来源：http://lzl.bjfxy.top

Java: // 手写回溯递归
来源：http://lah.dashuyun.cn

Go:   // 手写回溯递归
来源：http://fxd.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://gyl.hcnkem.com

C#:   // 手写回溯递归
来源：http://xyl.shanyushiyangtech.top

[N09] 栈与队列
来源：http://nbd.fehbvm.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jkq.yj202588.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ifr.xinyue.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://soh.c1oappe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://psb.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lhu.havefunace.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zmy.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://knc.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vij.kuanghao11.cn

[N10] 链表节点定义
来源：http://gfx.meibo888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://imu.cdnleiting.top

PHP:  class Node { public $v; public $next = null; }
来源：http://txu.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qsj.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jkk.shzxlz.cn

Java: class Node { int v; Node next; }
来源：http://xyq.aibaodan.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sbs.zhoulong.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://kdx.shangyingyoupin.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qfr.9152youxi.cn

[N11] 二叉树中序遍历
来源：http://bvz.zhijiandao.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qoo.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://vdt.zhoulong.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dlf.zhoulong.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sev.smart0.xyz

Java: // 手写递归
来源：http://lmi.tanke756.top

Go:   // 手写递归
来源：http://fwf.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://meh.zhijiandao.cn

C#:   // 手写递归
来源：http://xbu.0kj1m.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bbm.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bnw.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mcq.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zrj.ppjwa.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zuz.nanxinkj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://atq.ivvv.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zox.fzhhl.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hit.daxiang520.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qyh.hywenlv.cn

================================================================================
来源：http://qip.hongshengwenyu.top

O. 并发与异步
来源：http://zbb.xingfuxueyuan.xyz

================================================================================
来源：http://wwj.havefunace.top

[O01] 启动一个线程
来源：http://dxc.zdbjq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rrm.zhaomingkeji.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hip.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ali.tianlin.xyz

TS:   // 同 JS
来源：http://kvn.c1oappe.top

Java: new Thread(() -> f()).start()
来源：http://jit.haohaochexian.top

Go:   go f()
来源：http://mpl.cdnleiting.top

Ruby: Thread.new { f }
来源：http://vwj.shuidangran.top

C#:   Task.Run(() => F());
来源：http://umr.jqgfzy.top

[O02] 使用线程池
来源：http://lrs.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uzm.redwolf501.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aek.yangfankeji.com

JS:   // worker_threads 线程池
来源：http://eze.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://xua.guowangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://kwi.gotoacloud.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pzg.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://avs.yvedp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qgn.chenjidiqi.icu

[O03] 加锁保护共享数据
来源：http://wkd.jianghu66.top

Py:   with lock: shared += 1
来源：http://ahz.chenjidiqi.icu

PHP:  // 用 flock() 做文件锁
来源：http://obp.jqgufenzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jtq.yuanzhike.top

TS:   // 同 JS
来源：http://jbc.zhixingplan.top

Java: synchronized (this) { shared++; }
来源：http://jyf.iojbl.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bfl.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jst.andypj.xyz

C#:   lock (gate) { shared++; }
来源：http://sju.wangshuangyany.cn

[O04] 定义异步函数并等待
来源：http://zfz.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://yhr.0kj1m.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fal.ydzc1.top

JS:   async function f() { await g(); }
来源：http://wvp.feifeiyinyue.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ibd.redwolf501.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xfw.xziqi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hzj.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kcd.yongpay.top

C#:   async Task F() { await G(); }
来源：http://xyc.52xcode.cn

[O05] 并发执行并等待全部完成
来源：http://kly.hnxiangtu.top

Py:   asyncio.gather(*tasks)
来源：http://rkn.smart0.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://osv.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://wyo.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://lxx.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nte.gogol.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://odq.zhongyouzk.top

Ruby: threads.map(&:join)
来源：http://qui.hongshengwenyu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://eey.ybcxt.top


<!-- 参考信息 -->