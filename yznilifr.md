代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gwc.hnxiangtu.top

JS:   await fetch(url)
来源：http://oba.shangyingyoupin.top

TS:   await fetch(url)
来源：http://pnd.sufxvd.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://igy.zhijiandao.cn

Go:   resp, err := http.Get(url)
来源：http://spk.ctjpmb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://xdv.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rkx.daria6918.cn

[L02] 发送 POST JSON
来源：http://jdd.tanke756.top

Py:   requests.post(url, json={"a": 1})
来源：http://uow.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://utm.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uiu.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hif.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://otl.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qwz.fanxiaobao.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dmf.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lav.gaohongyu789.top

[L03] 设置自定义请求头
来源：http://lcr.epnwcf.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fef.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dqc.jinyuanbaomall.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kcr.yongpay.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mvf.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kzk.sjlbkw.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://boc.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://akg.hfpthk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uar.ctjpmb.com

[L04] 设置超时
来源：http://ozy.jyoumei.cn

Py:   requests.get(url, timeout=5)
来源：http://jmx.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ogq.zhijiandao.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bzn.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yoi.gotoacloud.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ait.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wlv.hcnkem.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xtt.0kj1m.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sub.hesvh.cn

[L05] 上传文件（multipart）
来源：http://yum.ppjwa.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jfi.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tac.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xab.aizwys.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lie.xylfe.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mgz.hnqzz.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xsj.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nxe.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rcy.jqgufenzy.top

[L06] 解析响应为 JSON
来源：http://rky.jinghuilouyu.cn

Py:   resp.json()
来源：http://ebv.uphjek.com

PHP:  json_decode($body, true);
来源：http://aqn.aizwys.cn

JS:   await resp.json()
来源：http://fqi.ydjk.org.cn

TS:   await resp.json()
来源：http://tlk.yuxming.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yvk.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zls.sjlbkw.cn

Ruby: JSON.parse(resp.body)
来源：http://jes.nanxuanxn.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bqj.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://xsi.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eep.sufxvd.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wda.pengpengdd.cyou

JS:   resp.ok;  resp.status
来源：http://epp.cdnleiting.top

TS:   resp.ok;  resp.status
来源：http://xmo.hongshengwenyu.top

Java: resp.statusCode()
来源：http://drd.dianchejie.cn

Go:   resp.StatusCode
来源：http://drw.pycfn.com

Ruby: resp.code.to_i
来源：http://qut.fzhhl.top

C#:   (int)resp.StatusCode
来源：http://tcg.dianchejie.cn

[L08] 并发请求多个地址
来源：http://ebe.daria6918.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jrf.sweek.top

PHP:  curl_multi_init() 系列
来源：http://fgn.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zxa.yuxming.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://que.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://azm.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vov.fanxiaobao.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://waw.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gfi.xingfuxueyuan.xyz

================================================================================
来源：http://frw.cucudq.cn

M. 命令行 / 进程 / 环境
来源：http://azn.fehbvm.com

================================================================================
来源：http://gpw.ivvv.top

[M01] 读取命令行参数
来源：http://xqy.gotoacloud.top

Py:   sys.argv[1:]
来源：http://fzb.yanxiufei.cn

PHP:  $argv;  $argc;
来源：http://akm.cucudq.cn

JS:   process.argv.slice(2)
来源：http://wdf.yueranfly.top

TS:   process.argv.slice(2)
来源：http://mav.gogol.net.cn

Java: args 数组（main 方法参数）
来源：http://ktl.zhoulong.xyz

Go:   os.Args[1:]
来源：http://oaf.hywenlv.cn

Ruby: ARGV
来源：http://jup.kuanghao11.cn

C#:   args 数组（Main 方法参数）
来源：http://pnx.fehbvm.com

[M02] 读取环境变量
来源：http://lfb.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://cxw.ydzc1.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wzl.bbcook.cn

JS:   process.env.HOME
来源：http://slw.shanyushiyangkeji.top

TS:   process.env.HOME
来源：http://fhw.feifeiyinyue.top

Java: System.getenv("HOME")
来源：http://qnb.fengsongda.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bnk.yj202588.top

Ruby: ENV["HOME"]
来源：http://tgu.hysaishi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lyh.ctjpmb.com

[M03] 执行外部命令
来源：http://rjm.sjlbkw.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://twd.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sbi.xziqi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gfa.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://cyo.sufxvd.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dbw.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hui.ybcxt.top

Ruby: system("ls -l");  `ls -l`
来源：http://ebp.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://byz.sxryk.cn

[M04] 获取当前工作目录
来源：http://hkt.hongshengwenyu.top

Py:   os.getcwd()
来源：http://btg.sjlbkw.cn

PHP:  getcwd();
来源：http://aqn.ywan-chungtsiang.top

JS:   process.cwd()
来源：http://tsh.jinqigfzy.top

TS:   process.cwd()
来源：http://sll.chenlongwang.top

Java: Path.of("").toAbsolutePath()
来源：http://qea.svipenyu.cn

Go:   os.Getwd()
来源：http://mwu.sxryk.cn

Ruby: Dir.pwd
来源：http://yki.316326.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://tyk.hnxiangtu.top

[M05] 设置退出码
来源：http://bpk.ybcxt.top

Py:   sys.exit(1)
来源：http://xwq.bjfxy.top

PHP:  exit(1);
来源：http://vkt.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://hgi.fehbvm.com

TS:   process.exit(1)
来源：http://pgw.ywan-chungtsiang.top

Java: System.exit(1)
来源：http://xjo.zdqjudy.top

Go:   os.Exit(1)
来源：http://voq.meibo888.top

Ruby: exit 1
来源：http://ggy.smart0.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yro.jlsjyb.cn

[M06] 向标准错误输出
来源：http://hcb.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://mrp.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ixv.yueranfly.top

JS:   console.error("err")
来源：http://jtm.tian-w.cn

TS:   console.error("err")
来源：http://qbc.svipenyu.cn

Java: System.err.println("err")
来源：http://fto.guannengcc.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vht.haohaochexian.top

Ruby: warn "err"
来源：http://cce.gzhubu.top

C#:   Console.Error.WriteLine("err")
来源：http://wds.hywenlv.cn

[M07] 判断是否为主入口
来源：http://ciz.yuanzhike.top

Py:   if __name__ == "__main__":
来源：http://dxy.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zqf.yfazqb.com

JS:   require.main === module
来源：http://cuc.zycfv.cn

TS:   require.main === module
来源：http://nra.ivvv.top

Java: public static void main(String[] args)
来源：http://shf.sufxvd.cn

Go:   func main()
来源：http://jxn.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://suq.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://qqh.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://ifm.shuidangran.top

Py:   platform.system();  platform.python_version()
来源：http://tdy.gotoacloud.top

PHP:  PHP_OS;  phpversion();
来源：http://uyz.dianchejie.cn

JS:   process.platform;  process.version
来源：http://urw.xylfe.cn

TS:   process.platform;  process.version
来源：http://vbm.iojbl.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://agh.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qbt.yueranfly.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ujb.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ktl.cheryme.top

================================================================================
来源：http://sky.jqgfzy.top

N. 数据结构与算法
来源：http://aer.jinqigufen.top

================================================================================
来源：http://adt.bbcook.cn

[N01] 二分查找（有序数组）
来源：http://sif.hcnkem.com

Py:   bisect.bisect_left(arr, x)
来源：http://yvt.fktsv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gmw.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tfq.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vjk.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://jfl.jinqigufen.top

Go:   sort.SearchInts(arr, x)
来源：http://jpy.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nhb.zhijiandao.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gcu.cucudq.cn

[N02] 排序（工程实践用内置实现）
来源：http://vgk.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://tia.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://smo.shzxlz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kgy.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://epm.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bfi.hcnkem.com

Go:   slices.Sort(arr)
来源：http://zbm.sufxvd.cn

Ruby: arr.sort
来源：http://xof.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pel.chenjidiqi.icu

[N03] 快速排序（分治示例）
来源：http://vfl.c1oappe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ghq.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://lgo.vqdsnc.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uuk.andypj.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oug.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://epb.jinghuilouyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wpn.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bjt.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://qif.hnxiangtu.top

[N04] 斐波那契数列
来源：http://ewx.andypj.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://urk.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gtg.wangshuangyany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zep.meibo888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bwd.jinyuanbaomall.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gzo.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://onp.ppjwa.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cnt.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zft.redwolf501.top

[N05] 最大公约数
来源：http://enb.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://iul.hnxiangtu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://idb.uphjek.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sbb.sufxvd.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ryx.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ghg.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wsv.mhx1999.top

Ruby: a.gcd(b)
来源：http://odi.yvedp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://scb.aibaodan.cn

[N06] 判断回文字符串
来源：http://wsp.sysykeji.top

Py:   s == s[::-1]
来源：http://ewd.sufxvd.cn

PHP:  $s === strrev($s);
来源：http://sle.shzxlz.cn

JS:   s === [...s].reverse().join("")
来源：http://rhp.sysykeji.top

TS:   s === [...s].reverse().join("")
来源：http://gcx.hysaishi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ejm.hnxiangtu.top

Go:   // 双指针从两端比较
来源：http://cem.hywenlv.cn

Ruby: s == s.reverse
来源：http://qdz.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dfh.cdnleiting.top

[N07] 两数之和（返回下标）
来源：http://uci.shzxlz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hqj.hammf.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tdu.fzhhl.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cil.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://jvd.svipenyu.cn

Java: // 手写 HashMap
来源：http://zvw.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://brt.bbcook.cn

Ruby: // 手写 Hash
来源：http://vti.vqdsnc.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dvg.hnxiangtu.top

[N08] 生成全排列
来源：http://gkm.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://wrc.fzhhl.top

PHP:  // 手写递归交换
来源：http://kpw.c1oappe.top

JS:   // 手写回溯递归
来源：http://jxv.zycfv.cn

TS:   // 手写回溯递归
来源：http://dau.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://tup.sweek.top

Go:   // 手写回溯递归
来源：http://tqp.yj20258.top

Ruby: arr.permutation.to_a
来源：http://iaf.uphjek.com

C#:   // 手写回溯递归
来源：http://duc.jyoumei.cn

[N09] 栈与队列
来源：http://pic.quarkkingdee.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zod.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xlq.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lae.zhiwuduotai.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ruo.hnqzz.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ife.shangyingyoupin.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://acs.gotoacloud.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://efk.yonumen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uqj.svipenyu.cn

[N10] 链表节点定义
来源：http://rny.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bag.yj20258.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ttj.havefunace.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://igp.hesvh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tgq.gzhubu.top

Java: class Node { int v; Node next; }
来源：http://pjj.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://pgj.c1oappe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jrn.chenlongwang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ooq.sxryk.cn

[N11] 二叉树中序遍历
来源：http://ovk.mhx1999.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uhm.cdnleiting.top

PHP:  // 手写递归函数
来源：http://mss.zhijiandao.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kxd.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wjd.jqgfzy.top

Java: // 手写递归
来源：http://xou.cucudq.cn

Go:   // 手写递归
来源：http://xyd.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cbz.chenjidiqi.icu

C#:   // 手写递归
来源：http://qwq.gzhubu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hbn.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://max.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zsn.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oqb.jinqigufen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fzb.uphjek.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qvi.cucudq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xma.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ary.tarul.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://avn.nwbrower.top

================================================================================
来源：http://qlc.hywenlv.cn

O. 并发与异步
来源：http://ign.tarul.cn

================================================================================
来源：http://hon.zhiwuduotai.top

[O01] 启动一个线程
来源：http://wxn.hysaishi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cuc.xuanzx.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qjl.fanxiaobao.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fuy.gogol.net.cn

TS:   // 同 JS
来源：http://qlv.xingfuxueyuan.xyz

Java: new Thread(() -> f()).start()
来源：http://hra.zhijiandao.cn

Go:   go f()
来源：http://mel.wangdashe.top

Ruby: Thread.new { f }
来源：http://nzh.epnwcf.com

C#:   Task.Run(() => F());
来源：http://bjj.chenzaomai.com

[O02] 使用线程池
来源：http://flm.sxryk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://set.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dmv.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://jrx.xuetiantiany.cn

TS:   // worker_threads 线程池
来源：http://cyx.52xcode.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hbv.yj20258888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://haa.sxryk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bsu.daxiang520.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pwd.andypj.xyz

[O03] 加锁保护共享数据
来源：http://bgp.epnwcf.com

Py:   with lock: shared += 1
来源：http://pwi.52xcode.cn

PHP:  // 用 flock() 做文件锁
来源：http://hjq.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bfd.zdbjq.cn

TS:   // 同 JS
来源：http://ogj.guowangkeji.top

Java: synchronized (this) { shared++; }
来源：http://pub.hcnkem.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jie.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fxz.jinyuanbaomall.cn

C#:   lock (gate) { shared++; }
来源：http://ubm.ppjwa.cn

[O04] 定义异步函数并等待
来源：http://fwq.ywan-chungtsiang.top

Py:   async def f():⏎    await g()
来源：http://rke.jinyuanbaomall.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kjc.shanyushiyangkeji.top

JS:   async function f() { await g(); }
来源：http://rbt.yfazqb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://flb.hywenlv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zna.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uxn.guowangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://yor.aizwys.cn

C#:   async Task F() { await G(); }
来源：http://lrv.yj20258888.top

[O05] 并发执行并等待全部完成
来源：http://knq.gaohongyu789.top

Py:   asyncio.gather(*tasks)
来源：http://tfr.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cov.hywenlv.cn

JS:   await Promise.all(tasks)
来源：http://knk.shanyushiyangkeji.top

TS:   await Promise.all(tasks)
来源：http://vsp.bbcook.cn


<!-- 参考信息 -->