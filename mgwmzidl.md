代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vkl.yfazqb.com

JS:   await fetch(url)
来源：http://msg.zhixingplan.top

TS:   await fetch(url)
来源：http://rkr.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uzn.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://dvk.gzhubu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cwk.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kgh.iojbl.cn

[L02] 发送 POST JSON
来源：http://jjh.yanxiufei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rep.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://luw.hysaishi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pgf.xziqi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vku.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dyf.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kou.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://abd.bbcook.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vpx.shanyushiyangtech.top

[L03] 设置自定义请求头
来源：http://qlq.zhixingplan.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cgr.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jlr.zhiwuduotai.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hir.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lsx.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://laa.sufxvd.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xsa.c1oappe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jrs.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iqu.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://kav.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://rou.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cfj.yj20258.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qbl.ydzc1.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ifd.gotoacloud.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uos.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xmu.ehwqpu.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pgk.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eve.shuidangran.top

[L05] 上传文件（multipart）
来源：http://bmo.jinyuanbaomall.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://msm.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://evt.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://stx.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ejr.cucudq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bkv.dashuyun.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nth.yangfankeji.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zud.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hfu.ydjk.org.cn

[L06] 解析响应为 JSON
来源：http://cco.guowangkeji.top

Py:   resp.json()
来源：http://azr.hongshengwenyu.top

PHP:  json_decode($body, true);
来源：http://tcq.tanke756.top

JS:   await resp.json()
来源：http://bim.ydjk.org.cn

TS:   await resp.json()
来源：http://mwd.hesvh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lpn.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rot.sjlbkw.cn

Ruby: JSON.parse(resp.body)
来源：http://zjv.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mng.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://mko.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bze.guannengcc.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wir.ydzc1.top

JS:   resp.ok;  resp.status
来源：http://jxq.xylfe.cn

TS:   resp.ok;  resp.status
来源：http://zow.yfazqb.com

Java: resp.statusCode()
来源：http://kez.ydzc1.top

Go:   resp.StatusCode
来源：http://cjr.ivvv.top

Ruby: resp.code.to_i
来源：http://lfa.0kj1m.cn

C#:   (int)resp.StatusCode
来源：http://mbw.9152youxi.cn

[L08] 并发请求多个地址
来源：http://xga.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ryn.fengsongda.top

PHP:  curl_multi_init() 系列
来源：http://bdj.jianghu66.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ein.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ndu.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://imq.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hwi.zycfv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wqn.zdqjudy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ilj.sjlbkw.cn

================================================================================
来源：http://zcv.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://jub.yuxming.cn

================================================================================
来源：http://lsg.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://emx.birdmap.top

Py:   sys.argv[1:]
来源：http://nwu.fengsongda.top

PHP:  $argv;  $argc;
来源：http://ykd.xuanzx.com

JS:   process.argv.slice(2)
来源：http://axq.bbcook.cn

TS:   process.argv.slice(2)
来源：http://ytq.gotoacloud.top

Java: args 数组（main 方法参数）
来源：http://lef.ydjk.org.cn

Go:   os.Args[1:]
来源：http://twd.zhengqikj.top

Ruby: ARGV
来源：http://ksf.vqdsnc.cn

C#:   args 数组（Main 方法参数）
来源：http://lam.tarul.cn

[M02] 读取环境变量
来源：http://pqb.gotoacloud.top

Py:   os.environ.get("HOME")
来源：http://bii.xinyue.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kzn.nanxuanxn.top

JS:   process.env.HOME
来源：http://whx.xuanzx.com

TS:   process.env.HOME
来源：http://mqy.zhaomingkeji.xyz

Java: System.getenv("HOME")
来源：http://lqu.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kbl.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://wfx.52xcode.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wdf.ywan-chungtsiang.top

[M03] 执行外部命令
来源：http://ado.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tjb.shanyushiyangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xtf.yuxming.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gtr.zdbjq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wtt.redwolf501.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nrx.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rdk.yj202588.top

Ruby: system("ls -l");  `ls -l`
来源：http://usw.guowangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://ari.xingfuxueyuan.xyz

[M04] 获取当前工作目录
来源：http://myl.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://sfg.jqgufenzy.top

PHP:  getcwd();
来源：http://ole.yangfankeji.com

JS:   process.cwd()
来源：http://dwp.yj20258888.top

TS:   process.cwd()
来源：http://mlq.pycfn.com

Java: Path.of("").toAbsolutePath()
来源：http://vfd.daria6918.cn

Go:   os.Getwd()
来源：http://jxt.smart0.xyz

Ruby: Dir.pwd
来源：http://vdm.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://jzm.mhx1999.top

[M05] 设置退出码
来源：http://iez.hesvh.cn

Py:   sys.exit(1)
来源：http://inz.vqdsnc.cn

PHP:  exit(1);
来源：http://qco.316326.xyz

JS:   process.exit(1)
来源：http://psk.nanxuanxn.top

TS:   process.exit(1)
来源：http://hje.xuetiantiany.cn

Java: System.exit(1)
来源：http://alw.cashguo.top

Go:   os.Exit(1)
来源：http://hcz.shzxlz.cn

Ruby: exit 1
来源：http://ahd.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ich.0kj1m.cn

[M06] 向标准错误输出
来源：http://luu.fehbvm.com

Py:   print("err", file=sys.stderr)
来源：http://ziy.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://sxl.cheryme.top

JS:   console.error("err")
来源：http://uki.xziqi.cn

TS:   console.error("err")
来源：http://bld.yvedp.cn

Java: System.err.println("err")
来源：http://syo.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mtr.ehwqpu.com

Ruby: warn "err"
来源：http://imn.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://xvi.guannengcc.top

[M07] 判断是否为主入口
来源：http://ozm.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://vwy.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://erc.sysykeji.top

JS:   require.main === module
来源：http://xyj.cqqwz.cn

TS:   require.main === module
来源：http://trv.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://ymk.wangdashe.top

Go:   func main()
来源：http://vqg.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pwq.fehbvm.com

C#:   static void Main(string[] args)
来源：http://zhc.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://vcm.vehdjk.com

Py:   platform.system();  platform.python_version()
来源：http://elw.sweek.top

PHP:  PHP_OS;  phpversion();
来源：http://voy.wangdashe.top

JS:   process.platform;  process.version
来源：http://ezd.jinqigfzy.top

TS:   process.platform;  process.version
来源：http://anw.ywan-chungtsiang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sxs.yj20258888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fvg.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iqy.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://tqh.xuetiantiany.cn

================================================================================
来源：http://sdf.yuanzhike.top

N. 数据结构与算法
来源：http://kor.chenzaomai.com

================================================================================
来源：http://iel.svipenyu.cn

[N01] 二分查找（有序数组）
来源：http://prx.jinghuilouyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tch.ppjwa.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ugg.hywenlv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mbt.hcnkem.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cfu.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://tzu.jinyuanbaomall.cn

Go:   sort.SearchInts(arr, x)
来源：http://ayq.dashuyun.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hwq.nanxinkj.top

C#:   Array.BinarySearch(arr, x)
来源：http://opa.daria6918.cn

[N02] 排序（工程实践用内置实现）
来源：http://lte.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://zsu.yanxiufei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://onx.vehdjk.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://rab.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gxt.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yxu.9152youxi.cn

Go:   slices.Sort(arr)
来源：http://nbl.zhongyouzk.top

Ruby: arr.sort
来源：http://dtl.dianchejie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zsy.jinqigufen.top

[N03] 快速排序（分治示例）
来源：http://xty.gaohongyu789.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zuu.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://hds.hnqzz.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://elq.sufxvd.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vaa.daxiang520.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kap.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bzm.zhijiandao.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fls.sufxvd.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gsc.yongpay.top

[N04] 斐波那契数列
来源：http://haz.aibaodan.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tdt.jinqigufen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ure.jyoumei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ero.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iuk.jqgufenzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tvj.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nlc.aizwys.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pbj.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sgw.fehbvm.com

[N05] 最大公约数
来源：http://rlh.fktsv.cn

Py:   math.gcd(a, b)
来源：http://fby.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oeu.haohaochexian.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ofz.hysaishi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cfm.hongshengwenyu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jdi.hfpthk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uro.yuxming.cn

Ruby: a.gcd(b)
来源：http://rfc.ywan-chungtsiang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tab.ppjwa.cn

[N06] 判断回文字符串
来源：http://cmn.xylfe.cn

Py:   s == s[::-1]
来源：http://yvi.cucudq.cn

PHP:  $s === strrev($s);
来源：http://jfk.fzhhl.top

JS:   s === [...s].reverse().join("")
来源：http://msw.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://qvw.ydjk.org.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bvg.guannengcc.top

Go:   // 双指针从两端比较
来源：http://mzb.ivvv.top

Ruby: s == s.reverse
来源：http://npv.tianlin.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://fqe.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://efp.hfpthk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vye.jinyuanbaomall.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sqe.haohaochexian.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dik.fengsongda.top

TS:   // 手写 Map<string, number>
来源：http://kpf.havefunace.top

Java: // 手写 HashMap
来源：http://ijh.shzxlz.cn

Go:   // 手写 map[int]int
来源：http://zox.nwbrower.top

Ruby: // 手写 Hash
来源：http://cxw.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://sqb.xuanzx.com

[N08] 生成全排列
来源：http://lcu.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://ktb.hysaishi.cn

PHP:  // 手写递归交换
来源：http://cor.zhengqikj.top

JS:   // 手写回溯递归
来源：http://gtt.meibo888.top

TS:   // 手写回溯递归
来源：http://bqh.xziqi.cn

Java: // 手写回溯递归
来源：http://yde.hcnkem.com

Go:   // 手写回溯递归
来源：http://veh.yuanzhike.top

Ruby: arr.permutation.to_a
来源：http://mxe.daxiang520.top

C#:   // 手写回溯递归
来源：http://evw.gzhubu.top

[N09] 栈与队列
来源：http://klb.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vmj.smart0.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nuy.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hcc.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tfv.gzhubu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rtv.havefunace.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gyz.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ewu.yuxming.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qqb.cashguo.top

[N10] 链表节点定义
来源：http://mva.andypj.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cqa.aizwys.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ztu.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nbc.tianlin.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qyx.chenzaomai.com

Java: class Node { int v; Node next; }
来源：http://zvc.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ism.haohaochexian.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hok.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://grk.smart0.xyz

[N11] 二叉树中序遍历
来源：http://djp.yuanzhike.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hae.jinyuanbaomall.cn

PHP:  // 手写递归函数
来源：http://thf.chenlongwang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mea.jqgufenzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dqd.uphjek.com

Java: // 手写递归
来源：http://pxv.jlsjyb.cn

Go:   // 手写递归
来源：http://mcn.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://isw.smart0.xyz

C#:   // 手写递归
来源：http://skg.yj202588.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rud.xuanzx.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ero.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jxd.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wbc.jyoumei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oen.daxiang520.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ksw.gaohongyu789.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://frj.ivvv.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vyb.ywan-chungtsiang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://itu.yanxiufei.cn

================================================================================
来源：http://vql.jiagoushi.top

O. 并发与异步
来源：http://qmj.ivvv.top

================================================================================
来源：http://kaf.uphjek.com

[O01] 启动一个线程
来源：http://yws.hnxiangtu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vfe.0kj1m.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kyd.uphjek.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jws.sweek.top

TS:   // 同 JS
来源：http://dki.yangfankeji.com

Java: new Thread(() -> f()).start()
来源：http://xcr.sysykeji.top

Go:   go f()
来源：http://xyc.sxryk.cn

Ruby: Thread.new { f }
来源：http://jgq.cucudq.cn

C#:   Task.Run(() => F());
来源：http://dbm.zhixingplan.top

[O02] 使用线程池
来源：http://bad.hongshengwenyu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://slp.xuanzx.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nnk.chenjidiqi.icu

JS:   // worker_threads 线程池
来源：http://cre.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://bbl.yueranfly.top

Java: Executors.newFixedThreadPool(4)
来源：http://yjv.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://joy.gogol.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wog.uphjek.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://min.ywan-chungtsiang.top

[O03] 加锁保护共享数据
来源：http://fng.snrcjt.cn

Py:   with lock: shared += 1
来源：http://zom.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://sfk.fanxiaobao.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zek.yueranfly.top

TS:   // 同 JS
来源：http://cnq.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://euz.jianghu66.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sfm.jinqigufen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zah.daria6918.cn

C#:   lock (gate) { shared++; }
来源：http://ies.jqgufenzy.top

[O04] 定义异步函数并等待
来源：http://uoi.daxiang520.top

Py:   async def f():⏎    await g()
来源：http://fih.zdqjudy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dlh.sjlbkw.cn

JS:   async function f() { await g(); }
来源：http://mys.hcnkem.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://mfk.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dym.cdnleiting.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xih.xziqi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bkb.yj20258.top

C#:   async Task F() { await G(); }
来源：http://okn.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://mne.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://sof.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qfj.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://whk.sxryk.cn

TS:   await Promise.all(tasks)
来源：http://xrl.shangyingyoupin.top


<!-- 参考信息 -->