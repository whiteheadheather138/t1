代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://jib.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wbi.fehbvm.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jen.yongpay.top

[L02] 发送 POST JSON
来源：http://kmi.sweek.top

Py:   requests.post(url, json={"a": 1})
来源：http://uxp.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://saq.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xdu.jqgfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sdv.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://emm.nanxinkj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mtd.ywan-chungtsiang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rfw.yfazqb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ikt.316326.xyz

[L03] 设置自定义请求头
来源：http://ojz.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dqh.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xrp.zhaomingkeji.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://daz.jlsjyb.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vaa.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vbt.zhoulong.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mpg.xinyue.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wje.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kgl.sysykeji.top

[L04] 设置超时
来源：http://bih.daria6918.cn

Py:   requests.get(url, timeout=5)
来源：http://ytg.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vqq.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dfm.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uzo.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yhl.chenlongwang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tfq.daria6918.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jzt.haohaochexian.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ftt.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://vey.shanyushiyangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jqf.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hgc.zhijiandao.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ffi.xuanzx.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wml.gzhubu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ytg.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ype.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zfp.hnxiangtu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tts.ywan-chungtsiang.top

[L06] 解析响应为 JSON
来源：http://csv.yfazqb.com

Py:   resp.json()
来源：http://pni.zycfv.cn

PHP:  json_decode($body, true);
来源：http://now.vehdjk.com

JS:   await resp.json()
来源：http://oco.redwolf501.top

TS:   await resp.json()
来源：http://myq.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://div.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xpd.yfazqb.com

Ruby: JSON.parse(resp.body)
来源：http://szz.gaohongyu789.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ljh.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://sci.ctjpmb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nah.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bqy.hywenlv.cn

JS:   resp.ok;  resp.status
来源：http://amg.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://izk.uphjek.com

Java: resp.statusCode()
来源：http://qwi.zycfv.cn

Go:   resp.StatusCode
来源：http://jxb.yj20258.top

Ruby: resp.code.to_i
来源：http://ird.dianchejie.cn

C#:   (int)resp.StatusCode
来源：http://ahf.yj20258.top

[L08] 并发请求多个地址
来源：http://aym.sxryk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zsq.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://ppn.zycfv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iqt.dianchejie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rzl.zhongyouzk.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xws.zhoulong.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rfr.guowangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gwm.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pyp.daria6918.cn

================================================================================
来源：http://onc.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://fla.xuetiantiany.cn

================================================================================
来源：http://kbv.sxryk.cn

[M01] 读取命令行参数
来源：http://igw.zhixingplan.top

Py:   sys.argv[1:]
来源：http://sjs.gzhubu.top

PHP:  $argv;  $argc;
来源：http://mpu.mhx1999.top

JS:   process.argv.slice(2)
来源：http://yen.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://xhx.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://ldw.redwolf501.top

Go:   os.Args[1:]
来源：http://cyc.jiagoushi.top

Ruby: ARGV
来源：http://tmw.shuidangran.top

C#:   args 数组（Main 方法参数）
来源：http://eoy.yonumen.top

[M02] 读取环境变量
来源：http://hqg.tianlin.xyz

Py:   os.environ.get("HOME")
来源：http://oxb.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xrz.52xcode.cn

JS:   process.env.HOME
来源：http://hly.dianchejie.cn

TS:   process.env.HOME
来源：http://bgt.cheryme.top

Java: System.getenv("HOME")
来源：http://szo.yonumen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fsb.jqgufenzy.top

Ruby: ENV["HOME"]
来源：http://imq.zhoulong.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pws.gotoacloud.top

[M03] 执行外部命令
来源：http://kwp.chenzaomai.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://haj.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hyh.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kdx.meibo888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://sin.fanxiaobao.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nyr.ydjk.org.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qvu.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hus.ivvv.top

C#:   Process.Start("ls", "-l");
来源：http://gdy.c1oappe.top

[M04] 获取当前工作目录
来源：http://syc.gogol.net.cn

Py:   os.getcwd()
来源：http://yju.zhoulong.xyz

PHP:  getcwd();
来源：http://qoj.xylfe.cn

JS:   process.cwd()
来源：http://bom.cdnleiting.top

TS:   process.cwd()
来源：http://myi.yuanzhike.top

Java: Path.of("").toAbsolutePath()
来源：http://afk.shzxlz.cn

Go:   os.Getwd()
来源：http://onz.cqqwz.cn

Ruby: Dir.pwd
来源：http://ztg.zdqjudy.top

C#:   Directory.GetCurrentDirectory()
来源：http://jln.shangyingyoupin.top

[M05] 设置退出码
来源：http://kxj.fehbvm.com

Py:   sys.exit(1)
来源：http://bep.haohaochexian.top

PHP:  exit(1);
来源：http://yvn.iojbl.cn

JS:   process.exit(1)
来源：http://hxp.birdmap.top

TS:   process.exit(1)
来源：http://xkh.svipenyu.cn

Java: System.exit(1)
来源：http://afe.meibo888.top

Go:   os.Exit(1)
来源：http://nod.xylfe.cn

Ruby: exit 1
来源：http://vff.tarul.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mhj.hnqzz.top

[M06] 向标准错误输出
来源：http://nmf.zdbjq.cn

Py:   print("err", file=sys.stderr)
来源：http://qps.xinyue.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://cbc.yuanzhike.top

JS:   console.error("err")
来源：http://fqv.yfazqb.com

TS:   console.error("err")
来源：http://hnb.cqqwz.cn

Java: System.err.println("err")
来源：http://abr.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dkr.yuxming.cn

Ruby: warn "err"
来源：http://cyb.smart0.xyz

C#:   Console.Error.WriteLine("err")
来源：http://tra.fzhhl.top

[M07] 判断是否为主入口
来源：http://hba.yongpay.top

Py:   if __name__ == "__main__":
来源：http://hda.ppjwa.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eky.316326.xyz

JS:   require.main === module
来源：http://xtw.cashguo.top

TS:   require.main === module
来源：http://jgh.hongshengwenyu.top

Java: public static void main(String[] args)
来源：http://sov.jinqigufen.top

Go:   func main()
来源：http://ear.yanxiufei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vxl.jianghu66.top

C#:   static void Main(string[] args)
来源：http://tjl.chenjidiqi.icu

[M08] 获取系统与运行时信息
来源：http://pdw.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://jpy.dashuyun.cn

PHP:  PHP_OS;  phpversion();
来源：http://gtj.yfazqb.com

JS:   process.platform;  process.version
来源：http://gyx.c1oappe.top

TS:   process.platform;  process.version
来源：http://esg.epnwcf.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rim.hongshengwenyu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hsq.52xcode.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rin.epnwcf.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://vmy.nwbrower.top

================================================================================
来源：http://bdc.jinqigfzy.top

N. 数据结构与算法
来源：http://esc.jqgfzy.top

================================================================================
来源：http://sku.tian-w.cn

[N01] 二分查找（有序数组）
来源：http://fzl.hnxiangtu.top

Py:   bisect.bisect_left(arr, x)
来源：http://chh.yangfankeji.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://raq.havefunace.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://thc.chenjidiqi.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ttb.ivvv.top

Java: Arrays.binarySearch(arr, x)
来源：http://vil.316326.xyz

Go:   sort.SearchInts(arr, x)
来源：http://kqo.nanxinkj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vcp.sxryk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://asf.birdmap.top

[N02] 排序（工程实践用内置实现）
来源：http://wsd.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://oiz.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lsn.xinyue.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://nsl.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ars.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rly.nanxuanxn.top

Go:   slices.Sort(arr)
来源：http://gvr.hywenlv.cn

Ruby: arr.sort
来源：http://mhw.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://owo.jlsjyb.cn

[N03] 快速排序（分治示例）
来源：http://gcc.yangfankeji.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rtd.hywenlv.cn

PHP:  // 递归实现，或用 usort
来源：http://afu.andypj.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://art.aibaodan.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mpa.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://boj.shzxlz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://scr.sufxvd.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://isv.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://nje.feifeiyinyue.top

[N04] 斐波那契数列
来源：http://djt.pycfn.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dsx.0kj1m.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bqy.fzhhl.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kkz.cqqwz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mae.gogol.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pgl.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yru.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lyd.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://env.52xcode.cn

[N05] 最大公约数
来源：http://mvu.wangdashe.top

Py:   math.gcd(a, b)
来源：http://dao.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uvk.svipenyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://byh.vehdjk.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cpl.sufxvd.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lvt.jiagoushi.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wvj.52xcode.cn

Ruby: a.gcd(b)
来源：http://cjw.quarkkingdee.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bpn.zycfv.cn

[N06] 判断回文字符串
来源：http://gdw.aizwys.cn

Py:   s == s[::-1]
来源：http://agi.gotoacloud.top

PHP:  $s === strrev($s);
来源：http://glc.nanxinkj.top

JS:   s === [...s].reverse().join("")
来源：http://vsf.redwolf501.top

TS:   s === [...s].reverse().join("")
来源：http://pkv.xziqi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://frk.uphjek.com

Go:   // 双指针从两端比较
来源：http://pbz.gogol.net.cn

Ruby: s == s.reverse
来源：http://cfs.bjfxy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mfs.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://enr.redwolf501.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qkp.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yhv.chenjidiqi.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://mhf.aibaodan.cn

TS:   // 手写 Map<string, number>
来源：http://mdm.smart0.xyz

Java: // 手写 HashMap
来源：http://puv.ybcxt.top

Go:   // 手写 map[int]int
来源：http://dam.daria6918.cn

Ruby: // 手写 Hash
来源：http://ehk.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://ybu.gotoacloud.top

[N08] 生成全排列
来源：http://pys.epnwcf.com

Py:   itertools.permutations(arr)
来源：http://avt.jyoumei.cn

PHP:  // 手写递归交换
来源：http://jhn.snrcjt.cn

JS:   // 手写回溯递归
来源：http://cfb.gaohongyu789.top

TS:   // 手写回溯递归
来源：http://dhs.ehwqpu.com

Java: // 手写回溯递归
来源：http://ukh.cqqwz.cn

Go:   // 手写回溯递归
来源：http://mgw.sjlbkw.cn

Ruby: arr.permutation.to_a
来源：http://uon.daria6918.cn

C#:   // 手写回溯递归
来源：http://cdj.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://abh.birdmap.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xzn.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gjo.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yfz.nanxinkj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vcm.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tig.chenzaomai.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hja.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uor.nanxuanxn.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bcg.zhongyouzk.top

[N10] 链表节点定义
来源：http://jyw.fzhhl.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ihf.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zmw.52xcode.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qrw.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ktr.zdqjudy.top

Java: class Node { int v; Node next; }
来源：http://bqy.epnwcf.com

Go:   type Node struct { V int; Next *Node }
来源：http://zot.cashguo.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hge.svipenyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pph.aibaodan.cn

[N11] 二叉树中序遍历
来源：http://rcr.hfpthk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ghx.cashguo.top

PHP:  // 手写递归函数
来源：http://anq.zhijiandao.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fod.jyoumei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xty.cashguo.top

Java: // 手写递归
来源：http://qny.bbcook.cn

Go:   // 手写递归
来源：http://wei.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tyt.ydzc1.top

C#:   // 手写递归
来源：http://xet.yvedp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uqq.xingfuxueyuan.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nzf.sysykeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://koz.hongshengwenyu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mkf.yonumen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ctm.zhongyouzk.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cns.andypj.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ayl.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kyr.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pgx.dianchejie.cn

================================================================================
来源：http://bsl.hongshengwenyu.top

O. 并发与异步
来源：http://nlk.xingfuxueyuan.xyz

================================================================================
来源：http://zen.cqqwz.cn

[O01] 启动一个线程
来源：http://ndf.shzxlz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pnw.yangfankeji.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ked.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pmg.dashuyun.cn

TS:   // 同 JS
来源：http://uwd.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://frn.hcnkem.com

Go:   go f()
来源：http://zsu.daxiang520.top

Ruby: Thread.new { f }
来源：http://bfr.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://bpr.52xcode.cn

[O02] 使用线程池
来源：http://vkj.uphjek.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://aan.pengpengdd.cyou

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://usz.meibo888.top

JS:   // worker_threads 线程池
来源：http://bif.aibaodan.cn

TS:   // worker_threads 线程池
来源：http://fba.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xyw.ydjk.org.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rwa.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://byw.shangyingyoupin.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mbf.xziqi.cn

[O03] 加锁保护共享数据
来源：http://gki.vehdjk.com

Py:   with lock: shared += 1
来源：http://ruv.yonumen.top

PHP:  // 用 flock() 做文件锁
来源：http://ihp.9152youxi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gcs.yonumen.top

TS:   // 同 JS
来源：http://omf.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://aoq.jlsjyb.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rry.9152youxi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bph.hesvh.cn

C#:   lock (gate) { shared++; }
来源：http://wdv.zhoulong.xyz

[O04] 定义异步函数并等待
来源：http://wec.yvedp.cn

Py:   async def f():⏎    await g()
来源：http://rqv.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lgl.fanxiaobao.xyz

JS:   async function f() { await g(); }
来源：http://dks.guannengcc.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://epl.aibaodan.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://erw.fzhhl.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tbj.fehbvm.com

Ruby: # 用 Fiber 或 async gem
来源：http://kie.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://gpv.yuanzhike.top

[O05] 并发执行并等待全部完成
来源：http://gnl.jiagoushi.top

Py:   asyncio.gather(*tasks)
来源：http://czu.aizwys.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://etn.xuanzx.com

JS:   await Promise.all(tasks)
来源：http://ani.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://buf.hcnkem.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rww.zhongyouzk.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vpx.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://pbd.zdqjudy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zxr.shanyushiyangtech.top


<!-- 参考信息 -->