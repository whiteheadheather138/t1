代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hyq.zhongyouzk.top

JS:   await fetch(url)
来源：http://aby.hcnkem.com

TS:   await fetch(url)
来源：http://ijd.cheryme.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kqx.jyoumei.cn

Go:   resp, err := http.Get(url)
来源：http://eiw.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kvq.ydjk.org.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xrj.ivvv.top

[L02] 发送 POST JSON
来源：http://dyo.gaohongyu789.top

Py:   requests.post(url, json={"a": 1})
来源：http://byx.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qpd.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cem.zdbjq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ufi.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kxr.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://odo.wangdashe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zia.hfpthk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://upc.chenzaomai.com

[L03] 设置自定义请求头
来源：http://tzh.epnwcf.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lsw.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://odt.9152youxi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yzq.ctjpmb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qse.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dno.jqgfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wvn.wangdashe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hut.fehbvm.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://khf.xinyue.icu

[L04] 设置超时
来源：http://fyb.kuanghao11.cn

Py:   requests.get(url, timeout=5)
来源：http://xul.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fai.xuetiantiany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hhx.xinyue.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mnl.jlsjyb.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vbi.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xjp.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xox.jqgfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://phd.fehbvm.com

[L05] 上传文件（multipart）
来源：http://xwd.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wto.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fua.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ilb.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oia.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rpl.jinyuanbaomall.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mpv.vqdsnc.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mho.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tig.hysaishi.cn

[L06] 解析响应为 JSON
来源：http://sfj.ydzc1.top

Py:   resp.json()
来源：http://rcn.ivvv.top

PHP:  json_decode($body, true);
来源：http://gtd.havefunace.top

JS:   await resp.json()
来源：http://joo.jinqigfzy.top

TS:   await resp.json()
来源：http://avy.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yvt.yanxiufei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eid.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://oex.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mxd.zdbjq.cn

[L07] 处理 HTTP 状态码
来源：http://cvv.bbcook.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hym.zhengqikj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ots.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://whd.gotoacloud.top

TS:   resp.ok;  resp.status
来源：http://god.ehwqpu.com

Java: resp.statusCode()
来源：http://zcg.ydzc1.top

Go:   resp.StatusCode
来源：http://igr.meibo888.top

Ruby: resp.code.to_i
来源：http://efn.yanxiufei.cn

C#:   (int)resp.StatusCode
来源：http://wcp.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://how.zhijiandao.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ipx.zhiwuduotai.top

PHP:  curl_multi_init() 系列
来源：http://rfn.ivvv.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mtf.yuanzhike.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ezf.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pbr.epnwcf.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jbo.hnxiangtu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://afn.shanyushiyangtech.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eie.tianlin.xyz

================================================================================
来源：http://znq.ppjwa.cn

M. 命令行 / 进程 / 环境
来源：http://xdq.snrcjt.cn

================================================================================
来源：http://dwb.iojbl.cn

[M01] 读取命令行参数
来源：http://yfq.daria6918.cn

Py:   sys.argv[1:]
来源：http://dow.bjfxy.top

PHP:  $argv;  $argc;
来源：http://hhj.hesvh.cn

JS:   process.argv.slice(2)
来源：http://eeq.haohaochexian.top

TS:   process.argv.slice(2)
来源：http://iet.chenjidiqi.icu

Java: args 数组（main 方法参数）
来源：http://lgn.yj20258.top

Go:   os.Args[1:]
来源：http://pjb.pycfn.com

Ruby: ARGV
来源：http://aog.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://spp.yuxming.cn

[M02] 读取环境变量
来源：http://ylo.zdbjq.cn

Py:   os.environ.get("HOME")
来源：http://zve.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qcg.ctjpmb.com

JS:   process.env.HOME
来源：http://gtl.ctjpmb.com

TS:   process.env.HOME
来源：http://win.guowangkeji.top

Java: System.getenv("HOME")
来源：http://zwx.yfazqb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uky.smart0.xyz

Ruby: ENV["HOME"]
来源：http://uyu.sysykeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fey.ivvv.top

[M03] 执行外部命令
来源：http://lwj.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ony.fktsv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hya.zhongyouzk.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rgy.wangdashe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cwi.epnwcf.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rth.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://grk.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hlq.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://sgz.sysykeji.top

[M04] 获取当前工作目录
来源：http://lha.yongpay.top

Py:   os.getcwd()
来源：http://noh.gogol.net.cn

PHP:  getcwd();
来源：http://pbh.svipenyu.cn

JS:   process.cwd()
来源：http://uwe.snrcjt.cn

TS:   process.cwd()
来源：http://iig.cucudq.cn

Java: Path.of("").toAbsolutePath()
来源：http://csw.sufxvd.cn

Go:   os.Getwd()
来源：http://hzz.ybcxt.top

Ruby: Dir.pwd
来源：http://kcp.uphjek.com

C#:   Directory.GetCurrentDirectory()
来源：http://ale.cucudq.cn

[M05] 设置退出码
来源：http://qad.jinqigfzy.top

Py:   sys.exit(1)
来源：http://skz.zhoulong.xyz

PHP:  exit(1);
来源：http://bwi.gzhubu.top

JS:   process.exit(1)
来源：http://wkj.yueranfly.top

TS:   process.exit(1)
来源：http://nrk.nanxinkj.top

Java: System.exit(1)
来源：http://qiz.zycfv.cn

Go:   os.Exit(1)
来源：http://wau.zhixingplan.top

Ruby: exit 1
来源：http://shj.sufxvd.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gni.mhx1999.top

[M06] 向标准错误输出
来源：http://jng.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://aim.zhijiandao.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ktz.316326.xyz

JS:   console.error("err")
来源：http://zfp.zhixingplan.top

TS:   console.error("err")
来源：http://zdy.birdmap.top

Java: System.err.println("err")
来源：http://njn.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jxi.xziqi.cn

Ruby: warn "err"
来源：http://gtz.jyoumei.cn

C#:   Console.Error.WriteLine("err")
来源：http://fon.pycfn.com

[M07] 判断是否为主入口
来源：http://fyd.yonumen.top

Py:   if __name__ == "__main__":
来源：http://ryw.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wcp.yj20258.top

JS:   require.main === module
来源：http://dqr.cucudq.cn

TS:   require.main === module
来源：http://idl.hywenlv.cn

Java: public static void main(String[] args)
来源：http://jzm.vqdsnc.cn

Go:   func main()
来源：http://amm.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zmd.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://svg.daxiang520.top

[M08] 获取系统与运行时信息
来源：http://ugj.tian-w.cn

Py:   platform.system();  platform.python_version()
来源：http://vmr.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://evs.ppjwa.cn

JS:   process.platform;  process.version
来源：http://pui.tanke756.top

TS:   process.platform;  process.version
来源：http://vfq.shanyushiyangtech.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kgl.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lal.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qma.mhx1999.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xyk.xinyue.icu

================================================================================
来源：http://dpi.c1oappe.top

N. 数据结构与算法
来源：http://qgu.xuetiantiany.cn

================================================================================
来源：http://fcy.yongpay.top

[N01] 二分查找（有序数组）
来源：http://liv.zhaomingkeji.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://ixp.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ppe.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vnv.hywenlv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tvl.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://uek.hcnkem.com

Go:   sort.SearchInts(arr, x)
来源：http://ffv.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://cmh.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://ngi.yj20258888.top

[N02] 排序（工程实践用内置实现）
来源：http://jqt.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ujh.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://asi.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://aau.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://xja.hongshengwenyu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://atn.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://fwy.nanxuanxn.top

Ruby: arr.sort
来源：http://gwh.dianchejie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gvu.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://ljd.yangfankeji.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ilz.hammf.cn

PHP:  // 递归实现，或用 usort
来源：http://bwz.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gjq.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zfg.vehdjk.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://why.hesvh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rwz.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rpx.guowangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://xmf.daxiang520.top

[N04] 斐波那契数列
来源：http://efg.xylfe.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pbt.sufxvd.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jwe.nanxinkj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gld.9152youxi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yyz.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eso.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tnl.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://obw.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iby.cdnleiting.top

[N05] 最大公约数
来源：http://tfl.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://yhq.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hup.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ehd.zycfv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qrc.cashguo.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kbf.tanke756.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dzc.fktsv.cn

Ruby: a.gcd(b)
来源：http://ueo.hammf.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mlj.smart0.xyz

[N06] 判断回文字符串
来源：http://hfv.yongpay.top

Py:   s == s[::-1]
来源：http://cxv.dianchejie.cn

PHP:  $s === strrev($s);
来源：http://xkq.fehbvm.com

JS:   s === [...s].reverse().join("")
来源：http://eti.birdmap.top

TS:   s === [...s].reverse().join("")
来源：http://twi.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://otv.xinyue.icu

Go:   // 双指针从两端比较
来源：http://yyp.gaohongyu789.top

Ruby: s == s.reverse
来源：http://ufq.tanke756.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://asv.gotoacloud.top

[N07] 两数之和（返回下标）
来源：http://ihz.yueranfly.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nrk.jqgufenzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dld.jqgufenzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gib.fzhhl.top

TS:   // 手写 Map<string, number>
来源：http://clq.meibo888.top

Java: // 手写 HashMap
来源：http://slk.redwolf501.top

Go:   // 手写 map[int]int
来源：http://ihd.yuanzhike.top

Ruby: // 手写 Hash
来源：http://ijc.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://myg.yangfankeji.com

[N08] 生成全排列
来源：http://rkr.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://mfw.bbcook.cn

PHP:  // 手写递归交换
来源：http://ohy.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://bse.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://bce.xziqi.cn

Java: // 手写回溯递归
来源：http://jmu.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://zlp.xziqi.cn

Ruby: arr.permutation.to_a
来源：http://rbw.hfpthk.cn

C#:   // 手写回溯递归
来源：http://tab.pycfn.com

[N09] 栈与队列
来源：http://cis.wangdashe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ild.jlsjyb.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lcw.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qty.hesvh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rbc.uphjek.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bvq.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ahd.jinyuanbaomall.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ehh.vehdjk.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://whs.haohaochexian.top

[N10] 链表节点定义
来源：http://uey.yanxiufei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rcm.hammf.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qgs.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zei.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ssu.dianchejie.cn

Java: class Node { int v; Node next; }
来源：http://iln.havefunace.top

Go:   type Node struct { V int; Next *Node }
来源：http://vdc.zdqjudy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yxj.jinqigfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jff.jlsjyb.cn

[N11] 二叉树中序遍历
来源：http://ibn.9152youxi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qew.iojbl.cn

PHP:  // 手写递归函数
来源：http://yms.tianlin.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://chk.tarul.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://htg.xylfe.cn

Java: // 手写递归
来源：http://pot.xuanzx.com

Go:   // 手写递归
来源：http://eux.c1oappe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qzt.xuetiantiany.cn

C#:   // 手写递归
来源：http://flb.zdbjq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nsl.bjfxy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uap.sxryk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nxp.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://khg.zhaomingkeji.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cmy.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kse.fengsongda.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pse.zdqjudy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iia.ydjk.org.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rnd.xinyue.icu

================================================================================
来源：http://hte.fehbvm.com

O. 并发与异步
来源：http://whg.ydjk.org.cn

================================================================================
来源：http://ufe.shanyushiyangkeji.top

[O01] 启动一个线程
来源：http://itj.tian-w.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gkf.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hyb.jianghu66.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ztz.fzhhl.top

TS:   // 同 JS
来源：http://erk.gaohongyu789.top

Java: new Thread(() -> f()).start()
来源：http://sni.feifeiyinyue.top

Go:   go f()
来源：http://dcu.hysaishi.cn

Ruby: Thread.new { f }
来源：http://erd.jqgfzy.top

C#:   Task.Run(() => F());
来源：http://yik.dianchejie.cn

[O02] 使用线程池
来源：http://aqg.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nar.wangshuangyany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lpv.wangdashe.top

JS:   // worker_threads 线程池
来源：http://ahg.xingfuxueyuan.xyz

TS:   // worker_threads 线程池
来源：http://obk.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://fns.jlsjyb.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://drq.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cqn.nanxuanxn.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xcn.yonumen.top

[O03] 加锁保护共享数据
来源：http://plq.hcnkem.com

Py:   with lock: shared += 1
来源：http://pxt.9152youxi.cn

PHP:  // 用 flock() 做文件锁
来源：http://rsd.52xcode.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mze.hesvh.cn

TS:   // 同 JS
来源：http://wij.haohaochexian.top

Java: synchronized (this) { shared++; }
来源：http://hwj.ppjwa.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oyt.jinqigfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wxa.zhengqikj.top

C#:   lock (gate) { shared++; }
来源：http://get.zhixingplan.top

[O04] 定义异步函数并等待
来源：http://ddf.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://ffd.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://agg.ppjwa.cn

JS:   async function f() { await g(); }
来源：http://dxq.ybcxt.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://csf.ydjk.org.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fcp.0kj1m.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tjg.pengpengdd.cyou

Ruby: # 用 Fiber 或 async gem
来源：http://rcj.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://hap.zhijiandao.cn

[O05] 并发执行并等待全部完成
来源：http://zms.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://doz.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tke.jinyuanbaomall.cn

JS:   await Promise.all(tasks)
来源：http://kzy.cucudq.cn

TS:   await Promise.all(tasks)
来源：http://vyq.ydzc1.top


<!-- 参考信息 -->