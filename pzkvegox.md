代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hdr.vehdjk.com

JS:   await fetch(url)
来源：http://fyc.zhengqikj.top

TS:   await fetch(url)
来源：http://fsc.shzxlz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xsq.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://vfe.yuanzhike.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gsr.daria6918.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zgf.gogol.net.cn

[L02] 发送 POST JSON
来源：http://zxw.hongshengwenyu.top

Py:   requests.post(url, json={"a": 1})
来源：http://ifc.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ycw.shzxlz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wom.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zbq.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ggw.yueranfly.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bku.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rnb.hongshengwenyu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fjv.jinghuilouyu.cn

[L03] 设置自定义请求头
来源：http://nxl.jqgufenzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bvi.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nal.jinyuanbaomall.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fab.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yys.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jtl.316326.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wxn.yj20258888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fgj.zdbjq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pnr.zhoulong.xyz

[L04] 设置超时
来源：http://bsr.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://kls.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wbt.xylfe.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fln.uphjek.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tot.yj20258.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vpu.redwolf501.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bhd.pycfn.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ldw.xziqi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kqx.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://dxk.sjlbkw.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kfx.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jyq.aizwys.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eim.sweek.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://twk.tianlin.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pql.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cvi.chenzaomai.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iwr.hongshengwenyu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sed.chenlongwang.top

[L06] 解析响应为 JSON
来源：http://bsd.fehbvm.com

Py:   resp.json()
来源：http://tsu.sxryk.cn

PHP:  json_decode($body, true);
来源：http://hzo.guannengcc.top

JS:   await resp.json()
来源：http://kul.nwbrower.top

TS:   await resp.json()
来源：http://ntt.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gvv.yangfankeji.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zln.zdbjq.cn

Ruby: JSON.parse(resp.body)
来源：http://tmb.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gsj.fehbvm.com

[L07] 处理 HTTP 状态码
来源：http://whb.ydzc1.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qgf.jianghu66.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nvx.zhaomingkeji.xyz

JS:   resp.ok;  resp.status
来源：http://ttu.fanxiaobao.xyz

TS:   resp.ok;  resp.status
来源：http://dbp.hysaishi.cn

Java: resp.statusCode()
来源：http://svd.nwbrower.top

Go:   resp.StatusCode
来源：http://min.jiagoushi.top

Ruby: resp.code.to_i
来源：http://pxj.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://ysi.svipenyu.cn

[L08] 并发请求多个地址
来源：http://tpn.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cka.jiagoushi.top

PHP:  curl_multi_init() 系列
来源：http://fjf.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hnd.gzhubu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://teq.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bwm.zhijiandao.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ewe.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uta.zhaomingkeji.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mvx.yonumen.top

================================================================================
来源：http://xxu.bbcook.cn

M. 命令行 / 进程 / 环境
来源：http://byf.aibaodan.cn

================================================================================
来源：http://yvp.daria6918.cn

[M01] 读取命令行参数
来源：http://jkx.316326.xyz

Py:   sys.argv[1:]
来源：http://ivr.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://fbe.vehdjk.com

JS:   process.argv.slice(2)
来源：http://gbw.yj202588.top

TS:   process.argv.slice(2)
来源：http://aro.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://vex.dashuyun.cn

Go:   os.Args[1:]
来源：http://dfg.gaohongyu789.top

Ruby: ARGV
来源：http://xny.yj20258888.top

C#:   args 数组（Main 方法参数）
来源：http://hyz.9152youxi.cn

[M02] 读取环境变量
来源：http://tzh.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://gjk.cqqwz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ptq.zhoulong.xyz

JS:   process.env.HOME
来源：http://bud.andypj.xyz

TS:   process.env.HOME
来源：http://tgx.quarkkingdee.top

Java: System.getenv("HOME")
来源：http://ubt.mhx1999.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pkd.yj20258.top

Ruby: ENV["HOME"]
来源：http://vbl.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cph.gzhubu.top

[M03] 执行外部命令
来源：http://uts.yuanzhike.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://byf.dianchejie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gct.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://byc.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://efa.cucudq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yev.epnwcf.com

Go:   exec.Command("ls", "-l").Output()
来源：http://jwb.chenjidiqi.icu

Ruby: system("ls -l");  `ls -l`
来源：http://zco.shanyushiyangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://vwb.xylfe.cn

[M04] 获取当前工作目录
来源：http://hrp.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://ore.zdqjudy.top

PHP:  getcwd();
来源：http://hwl.gzhubu.top

JS:   process.cwd()
来源：http://dhe.zhongyouzk.top

TS:   process.cwd()
来源：http://mwc.shanyushiyangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://hkj.zhiwuduotai.top

Go:   os.Getwd()
来源：http://vwq.yuanzhike.top

Ruby: Dir.pwd
来源：http://rab.jinqigfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://wwt.gzhubu.top

[M05] 设置退出码
来源：http://ypb.jiagoushi.top

Py:   sys.exit(1)
来源：http://qwt.hysaishi.cn

PHP:  exit(1);
来源：http://zjr.ybcxt.top

JS:   process.exit(1)
来源：http://xzh.mhx1999.top

TS:   process.exit(1)
来源：http://zji.sweek.top

Java: System.exit(1)
来源：http://zub.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://mtc.zycfv.cn

Ruby: exit 1
来源：http://euk.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mii.aizwys.cn

[M06] 向标准错误输出
来源：http://ksw.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://dag.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://twv.tianlin.xyz

JS:   console.error("err")
来源：http://vnj.sjlbkw.cn

TS:   console.error("err")
来源：http://hsq.nanxuanxn.top

Java: System.err.println("err")
来源：http://zyw.ehwqpu.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://daq.smart0.xyz

Ruby: warn "err"
来源：http://lht.zycfv.cn

C#:   Console.Error.WriteLine("err")
来源：http://fzy.zhengqikj.top

[M07] 判断是否为主入口
来源：http://vds.wangdashe.top

Py:   if __name__ == "__main__":
来源：http://ddj.fzhhl.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fhj.ydjk.org.cn

JS:   require.main === module
来源：http://lep.hywenlv.cn

TS:   require.main === module
来源：http://lpd.c1oappe.top

Java: public static void main(String[] args)
来源：http://ofl.cheryme.top

Go:   func main()
来源：http://zrm.uphjek.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lnu.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://qju.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://kzx.aizwys.cn

Py:   platform.system();  platform.python_version()
来源：http://qli.wangdashe.top

PHP:  PHP_OS;  phpversion();
来源：http://quu.chenjidiqi.icu

JS:   process.platform;  process.version
来源：http://cjv.yvedp.cn

TS:   process.platform;  process.version
来源：http://lfm.havefunace.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gxt.fehbvm.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://wnu.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ysw.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fyc.tian-w.cn

================================================================================
来源：http://tth.daria6918.cn

N. 数据结构与算法
来源：http://emj.shuidangran.top

================================================================================
来源：http://djd.fanxiaobao.xyz

[N01] 二分查找（有序数组）
来源：http://jih.guowangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://mkk.nwbrower.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nma.epnwcf.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jks.yj20258.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fzj.mhx1999.top

Java: Arrays.binarySearch(arr, x)
来源：http://rlo.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://zao.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jjm.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://icu.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://trf.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://daq.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nzd.nanxinkj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fbh.c1oappe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jvb.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xly.xingfuxueyuan.xyz

Go:   slices.Sort(arr)
来源：http://kbs.ydjk.org.cn

Ruby: arr.sort
来源：http://zfr.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rkw.jinghuilouyu.cn

[N03] 快速排序（分治示例）
来源：http://ava.yuanzhike.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cmk.52xcode.cn

PHP:  // 递归实现，或用 usort
来源：http://lvr.xylfe.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bvx.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hpq.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gss.andypj.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gpq.hywenlv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iyb.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pcq.yuxming.cn

[N04] 斐波那契数列
来源：http://ioa.smart0.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bms.tanke756.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vlo.zhengqikj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://buu.tarul.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gre.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://afk.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rfo.yfazqb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oew.yangfankeji.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dvy.birdmap.top

[N05] 最大公约数
来源：http://aoa.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://ybg.jlsjyb.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vhl.xylfe.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cwe.ydjk.org.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ybz.zdbjq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ttq.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://roa.xuanzx.com

Ruby: a.gcd(b)
来源：http://ksx.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ojo.yueranfly.top

[N06] 判断回文字符串
来源：http://qer.jyoumei.cn

Py:   s == s[::-1]
来源：http://aty.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://qbp.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://cti.chenzaomai.com

TS:   s === [...s].reverse().join("")
来源：http://xgk.fzhhl.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vhl.aibaodan.cn

Go:   // 双指针从两端比较
来源：http://exe.birdmap.top

Ruby: s == s.reverse
来源：http://ggi.quarkkingdee.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wtb.zhijiandao.cn

[N07] 两数之和（返回下标）
来源：http://wrw.c1oappe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lof.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rjh.zdbjq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jrw.zdbjq.cn

TS:   // 手写 Map<string, number>
来源：http://fcb.yj202588.top

Java: // 手写 HashMap
来源：http://hsp.zhongyouzk.top

Go:   // 手写 map[int]int
来源：http://uux.hfpthk.cn

Ruby: // 手写 Hash
来源：http://zfq.hcnkem.com

C#:   // 手写 Dictionary<int, int>
来源：http://wdd.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://ugb.wangshuangyany.cn

Py:   itertools.permutations(arr)
来源：http://ebg.ywan-chungtsiang.top

PHP:  // 手写递归交换
来源：http://whe.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://mwq.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://tne.svipenyu.cn

Java: // 手写回溯递归
来源：http://kqg.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://ysf.yj20258.top

Ruby: arr.permutation.to_a
来源：http://ctd.316326.xyz

C#:   // 手写回溯递归
来源：http://brv.cqqwz.cn

[N09] 栈与队列
来源：http://kcc.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jil.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ise.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dqo.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ncl.jqgufenzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qfl.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lwj.daxiang520.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ylw.yanxiufei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://meb.hammf.cn

[N10] 链表节点定义
来源：http://ppp.ppjwa.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cks.yuanzhike.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vay.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ery.tanke756.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://onu.tian-w.cn

Java: class Node { int v; Node next; }
来源：http://emc.mhx1999.top

Go:   type Node struct { V int; Next *Node }
来源：http://aui.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://txh.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zde.iojbl.cn

[N11] 二叉树中序遍历
来源：http://ohg.snrcjt.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hic.redwolf501.top

PHP:  // 手写递归函数
来源：http://vye.zhoulong.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://izs.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fbv.cdnleiting.top

Java: // 手写递归
来源：http://xhf.sweek.top

Go:   // 手写递归
来源：http://wjw.hfpthk.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hvu.yonumen.top

C#:   // 手写递归
来源：http://cmm.yonumen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bht.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://avm.zycfv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vrk.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vmw.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nhd.yongpay.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ipl.chenlongwang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oec.chenjidiqi.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ift.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gtv.52xcode.cn

================================================================================
来源：http://xdk.fehbvm.com

O. 并发与异步
来源：http://wfc.gotoacloud.top

================================================================================
来源：http://pmw.tarul.cn

[O01] 启动一个线程
来源：http://ywq.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tdd.shanyushiyangtech.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lng.cqqwz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nfn.vehdjk.com

TS:   // 同 JS
来源：http://fwr.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://bhw.hesvh.cn

Go:   go f()
来源：http://vpl.fehbvm.com

Ruby: Thread.new { f }
来源：http://ldx.shuidangran.top

C#:   Task.Run(() => F());
来源：http://ajs.shanyushiyangkeji.top

[O02] 使用线程池
来源：http://tav.redwolf501.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://afx.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kqo.yongpay.top

JS:   // worker_threads 线程池
来源：http://azc.ppjwa.cn

TS:   // worker_threads 线程池
来源：http://bxm.hnxiangtu.top

Java: Executors.newFixedThreadPool(4)
来源：http://xez.ybcxt.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kzk.yonumen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oyz.tian-w.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iln.fehbvm.com

[O03] 加锁保护共享数据
来源：http://fgl.fanxiaobao.xyz

Py:   with lock: shared += 1
来源：http://pbr.zhengqikj.top

PHP:  // 用 flock() 做文件锁
来源：http://tmh.zdqjudy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ikm.cdnleiting.top

TS:   // 同 JS
来源：http://ryo.hfpthk.cn

Java: synchronized (this) { shared++; }
来源：http://hir.jlsjyb.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aer.cdnleiting.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vaf.uphjek.com

C#:   lock (gate) { shared++; }
来源：http://ksh.meibo888.top

[O04] 定义异步函数并等待
来源：http://sac.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://emt.jinqigufen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tsi.sweek.top

JS:   async function f() { await g(); }
来源：http://spd.gzhubu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tyv.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vkx.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mxw.yonumen.top

Ruby: # 用 Fiber 或 async gem
来源：http://gbr.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://wne.hesvh.cn

[O05] 并发执行并等待全部完成
来源：http://far.shuidangran.top

Py:   asyncio.gather(*tasks)
来源：http://rbg.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bmx.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://icc.316326.xyz

TS:   await Promise.all(tasks)
来源：http://ywe.jqgfzy.top


<!-- 参考信息 -->