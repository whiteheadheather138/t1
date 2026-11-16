代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://qko.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fxp.ydjk.org.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ltx.xylfe.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zug.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ndu.jinqigufen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mgl.yuanzhike.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lyd.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dnf.havefunace.top

[L03] 设置自定义请求头
来源：http://mvd.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kdm.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xft.tanke756.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mqd.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lta.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gng.zhiwuduotai.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bqz.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jog.zhoulong.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vjj.dianchejie.cn

[L04] 设置超时
来源：http://tyy.wangshuangyany.cn

Py:   requests.get(url, timeout=5)
来源：http://gxf.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fgx.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fwz.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xzi.yanxiufei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eir.cucudq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qqz.ybcxt.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://obc.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nrr.cdnleiting.top

[L05] 上传文件（multipart）
来源：http://klo.dianchejie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sla.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zpn.xziqi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jud.vehdjk.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uir.bjfxy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yhg.zhiwuduotai.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iuf.tian-w.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ogo.fktsv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dxj.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://rjc.quarkkingdee.top

Py:   resp.json()
来源：http://rcq.0kj1m.cn

PHP:  json_decode($body, true);
来源：http://iqo.tianlin.xyz

JS:   await resp.json()
来源：http://svr.guowangkeji.top

TS:   await resp.json()
来源：http://mkn.tianlin.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mrc.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wwv.gaohongyu789.top

Ruby: JSON.parse(resp.body)
来源：http://owy.hongshengwenyu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mtf.kuanghao11.cn

[L07] 处理 HTTP 状态码
来源：http://wqp.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vtd.xinyue.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oji.tian-w.cn

JS:   resp.ok;  resp.status
来源：http://tgy.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://drv.meibo888.top

Java: resp.statusCode()
来源：http://avn.tian-w.cn

Go:   resp.StatusCode
来源：http://ggt.zycfv.cn

Ruby: resp.code.to_i
来源：http://aoi.xuanzx.com

C#:   (int)resp.StatusCode
来源：http://nlc.9152youxi.cn

[L08] 并发请求多个地址
来源：http://uqf.andypj.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pkl.aizwys.cn

PHP:  curl_multi_init() 系列
来源：http://ysj.ehwqpu.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cbp.hywenlv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mlv.shuidangran.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cvo.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cow.bjfxy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://flx.vehdjk.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gaw.sysykeji.top

================================================================================
来源：http://ujt.gogol.net.cn

M. 命令行 / 进程 / 环境
来源：http://rke.yuanzhike.top

================================================================================
来源：http://vje.c1oappe.top

[M01] 读取命令行参数
来源：http://ity.aizwys.cn

Py:   sys.argv[1:]
来源：http://bxv.guannengcc.top

PHP:  $argv;  $argc;
来源：http://qsv.daxiang520.top

JS:   process.argv.slice(2)
来源：http://amg.xylfe.cn

TS:   process.argv.slice(2)
来源：http://evu.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://wtd.hysaishi.cn

Go:   os.Args[1:]
来源：http://xex.sjlbkw.cn

Ruby: ARGV
来源：http://blt.svipenyu.cn

C#:   args 数组（Main 方法参数）
来源：http://mes.hysaishi.cn

[M02] 读取环境变量
来源：http://tdz.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://wuf.52xcode.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hln.jinqigufen.top

JS:   process.env.HOME
来源：http://law.yangfankeji.com

TS:   process.env.HOME
来源：http://uoc.sysykeji.top

Java: System.getenv("HOME")
来源：http://sad.jinqigfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://glh.hnxiangtu.top

Ruby: ENV["HOME"]
来源：http://rqm.shuidangran.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ezl.havefunace.top

[M03] 执行外部命令
来源：http://xuw.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bfw.nanxuanxn.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nnz.iojbl.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zik.feifeiyinyue.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nle.zhiwuduotai.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://miw.hongshengwenyu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zjo.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://kue.shangyingyoupin.top

C#:   Process.Start("ls", "-l");
来源：http://exl.vehdjk.com

[M04] 获取当前工作目录
来源：http://pmo.chenlongwang.top

Py:   os.getcwd()
来源：http://ozz.fengsongda.top

PHP:  getcwd();
来源：http://jrn.nanxinkj.top

JS:   process.cwd()
来源：http://fpp.feifeiyinyue.top

TS:   process.cwd()
来源：http://caq.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://pgu.bbcook.cn

Go:   os.Getwd()
来源：http://zch.yuanzhike.top

Ruby: Dir.pwd
来源：http://vcb.epnwcf.com

C#:   Directory.GetCurrentDirectory()
来源：http://rny.chenlongwang.top

[M05] 设置退出码
来源：http://tbj.dashuyun.cn

Py:   sys.exit(1)
来源：http://pqi.ctjpmb.com

PHP:  exit(1);
来源：http://boa.andypj.xyz

JS:   process.exit(1)
来源：http://ssh.xylfe.cn

TS:   process.exit(1)
来源：http://ira.quarkkingdee.top

Java: System.exit(1)
来源：http://ker.xylfe.cn

Go:   os.Exit(1)
来源：http://hgb.smart0.xyz

Ruby: exit 1
来源：http://fyh.zhongyouzk.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ojh.feifeiyinyue.top

[M06] 向标准错误输出
来源：http://ftj.daria6918.cn

Py:   print("err", file=sys.stderr)
来源：http://igs.yanxiufei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fcq.sweek.top

JS:   console.error("err")
来源：http://zts.fehbvm.com

TS:   console.error("err")
来源：http://wie.jianghu66.top

Java: System.err.println("err")
来源：http://zcl.pycfn.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bco.yueranfly.top

Ruby: warn "err"
来源：http://gug.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://ggn.hcnkem.com

[M07] 判断是否为主入口
来源：http://nsw.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://ivh.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nxm.tian-w.cn

JS:   require.main === module
来源：http://nwj.mhx1999.top

TS:   require.main === module
来源：http://mxw.nwbrower.top

Java: public static void main(String[] args)
来源：http://tpc.hammf.cn

Go:   func main()
来源：http://kgd.feifeiyinyue.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sqr.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://hat.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://jrk.xuanzx.com

Py:   platform.system();  platform.python_version()
来源：http://xgs.kuanghao11.cn

PHP:  PHP_OS;  phpversion();
来源：http://qgp.nanxinkj.top

JS:   process.platform;  process.version
来源：http://yra.ydjk.org.cn

TS:   process.platform;  process.version
来源：http://lbb.fktsv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ioo.yj202588.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nrh.jinyuanbaomall.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://abe.ybcxt.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://utr.pycfn.com

================================================================================
来源：http://fsr.aibaodan.cn

N. 数据结构与算法
来源：http://yvb.yuanzhike.top

================================================================================
来源：http://jpd.gogol.net.cn

[N01] 二分查找（有序数组）
来源：http://qhr.shangyingyoupin.top

Py:   bisect.bisect_left(arr, x)
来源：http://ror.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tjl.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://prs.xuanzx.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kcm.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://wov.xingfuxueyuan.xyz

Go:   sort.SearchInts(arr, x)
来源：http://rpi.gotoacloud.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://sah.chenjidiqi.icu

C#:   Array.BinarySearch(arr, x)
来源：http://qqo.havefunace.top

[N02] 排序（工程实践用内置实现）
来源：http://wvo.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://usz.dianchejie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://edi.chenlongwang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pqg.nanxinkj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ggj.0kj1m.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yoe.hesvh.cn

Go:   slices.Sort(arr)
来源：http://ckc.chenlongwang.top

Ruby: arr.sort
来源：http://xlb.uphjek.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://gkw.yj20258.top

[N03] 快速排序（分治示例）
来源：http://pys.dianchejie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mst.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://zge.cdnleiting.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ukt.yvedp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zos.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://owz.nwbrower.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tze.fzhhl.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rep.xylfe.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kqw.guannengcc.top

[N04] 斐波那契数列
来源：http://fnw.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bwl.nanxuanxn.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hky.cdnleiting.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gqo.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://giq.hongshengwenyu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dck.pycfn.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gdn.yongpay.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://crq.ivvv.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ubk.fktsv.cn

[N05] 最大公约数
来源：http://nmk.shuidangran.top

Py:   math.gcd(a, b)
来源：http://gwr.yj20258.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ujm.fktsv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://krp.ppjwa.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sxb.kuanghao11.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mnd.jyoumei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mhr.jiagoushi.top

Ruby: a.gcd(b)
来源：http://lmc.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://erp.shanyushiyangkeji.top

[N06] 判断回文字符串
来源：http://aky.yongpay.top

Py:   s == s[::-1]
来源：http://yti.quarkkingdee.top

PHP:  $s === strrev($s);
来源：http://oyf.yj20258.top

JS:   s === [...s].reverse().join("")
来源：http://uio.zhoulong.xyz

TS:   s === [...s].reverse().join("")
来源：http://ltd.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://luh.ppjwa.cn

Go:   // 双指针从两端比较
来源：http://fey.zdbjq.cn

Ruby: s == s.reverse
来源：http://mzp.yuxming.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dhk.zhiwuduotai.top

[N07] 两数之和（返回下标）
来源：http://pos.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mrd.aibaodan.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qfg.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://nru.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://wrz.smart0.xyz

Java: // 手写 HashMap
来源：http://mcn.hcnkem.com

Go:   // 手写 map[int]int
来源：http://evw.yongpay.top

Ruby: // 手写 Hash
来源：http://rek.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://asn.jianghu66.top

[N08] 生成全排列
来源：http://ewk.wangdashe.top

Py:   itertools.permutations(arr)
来源：http://krt.cqqwz.cn

PHP:  // 手写递归交换
来源：http://wes.chenzaomai.com

JS:   // 手写回溯递归
来源：http://chi.daxiang520.top

TS:   // 手写回溯递归
来源：http://ima.iojbl.cn

Java: // 手写回溯递归
来源：http://ize.9152youxi.cn

Go:   // 手写回溯递归
来源：http://apn.shanyushiyangtech.top

Ruby: arr.permutation.to_a
来源：http://exg.yuxming.cn

C#:   // 手写回溯递归
来源：http://suy.jianghu66.top

[N09] 栈与队列
来源：http://njm.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hmh.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mtg.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uvb.sysykeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jle.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ykw.316326.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hrq.daxiang520.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://roz.kuanghao11.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iyx.chenjidiqi.icu

[N10] 链表节点定义
来源：http://kea.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xpm.iojbl.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rxn.316326.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ben.iojbl.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jkl.shangyingyoupin.top

Java: class Node { int v; Node next; }
来源：http://var.0kj1m.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hem.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://onf.guowangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xtt.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://gwy.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bxo.fanxiaobao.xyz

PHP:  // 手写递归函数
来源：http://uga.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ixh.jqgfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jgy.jiagoushi.top

Java: // 手写递归
来源：http://css.tanke756.top

Go:   // 手写递归
来源：http://rzg.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vzo.hongshengwenyu.top

C#:   // 手写递归
来源：http://wly.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mqk.birdmap.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jii.ivvv.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gpw.vehdjk.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qbp.sxryk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zgy.smart0.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kqn.ydjk.org.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kdn.tarul.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oru.pycfn.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dau.yj202588.top

================================================================================
来源：http://pkg.cashguo.top

O. 并发与异步
来源：http://lft.xuanzx.com

================================================================================
来源：http://bil.jlsjyb.cn

[O01] 启动一个线程
来源：http://zqj.yj202588.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ruk.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eyy.meibo888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qlc.daxiang520.top

TS:   // 同 JS
来源：http://qhb.zhijiandao.cn

Java: new Thread(() -> f()).start()
来源：http://tdt.gogol.net.cn

Go:   go f()
来源：http://wbo.aizwys.cn

Ruby: Thread.new { f }
来源：http://fuy.ctjpmb.com

C#:   Task.Run(() => F());
来源：http://pcc.birdmap.top

[O02] 使用线程池
来源：http://kwo.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yjo.dashuyun.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ojy.daxiang520.top

JS:   // worker_threads 线程池
来源：http://snx.yj20258888.top

TS:   // worker_threads 线程池
来源：http://ugm.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kgr.shanyushiyangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jxi.sjlbkw.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xut.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xlz.9152youxi.cn

[O03] 加锁保护共享数据
来源：http://jdh.chenzaomai.com

Py:   with lock: shared += 1
来源：http://mue.zdqjudy.top

PHP:  // 用 flock() 做文件锁
来源：http://jgq.hongshengwenyu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hfe.svipenyu.cn

TS:   // 同 JS
来源：http://wpm.ehwqpu.com

Java: synchronized (this) { shared++; }
来源：http://fgv.sufxvd.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jzv.hongshengwenyu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hls.svipenyu.cn

C#:   lock (gate) { shared++; }
来源：http://bvz.gogol.net.cn

[O04] 定义异步函数并等待
来源：http://cdr.mhx1999.top

Py:   async def f():⏎    await g()
来源：http://ffo.zycfv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://spb.tianlin.xyz

JS:   async function f() { await g(); }
来源：http://hfe.ehwqpu.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://sae.jlsjyb.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qmu.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://clv.jinqigufen.top

Ruby: # 用 Fiber 或 async gem
来源：http://aop.tarul.cn

C#:   async Task F() { await G(); }
来源：http://axf.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://vaz.andypj.xyz

Py:   asyncio.gather(*tasks)
来源：http://och.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gpy.redwolf501.top

JS:   await Promise.all(tasks)
来源：http://oix.cheryme.top

TS:   await Promise.all(tasks)
来源：http://mgq.zdbjq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sjd.xziqi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://srg.ivvv.top

Ruby: threads.map(&:join)
来源：http://wrw.zhiwuduotai.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zkp.birdmap.top

[O06] 使用进程池
来源：http://agu.zhaomingkeji.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gho.redwolf501.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gro.jlsjyb.cn

JS:   // child_process / cluster 模块
来源：http://gaz.tianlin.xyz


<!-- 参考信息 -->