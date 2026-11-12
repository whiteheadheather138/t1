代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://tzy.svipenyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qml.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ojr.kuanghao11.cn

[L02] 发送 POST JSON
来源：http://aaf.andypj.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://dcy.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wlk.sysykeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jjm.hesvh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qaj.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rcc.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mba.ydzc1.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://egz.zhixingplan.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://apo.aizwys.cn

[L03] 设置自定义请求头
来源：http://esc.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://okk.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bzk.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fth.dashuyun.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uep.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tdk.xinyue.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sch.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vwz.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jhd.hesvh.cn

[L04] 设置超时
来源：http://jms.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://pdj.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cem.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vjo.zdbjq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tcr.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pxl.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fuy.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rvi.gaohongyu789.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kcp.bjfxy.top

[L05] 上传文件（multipart）
来源：http://eky.meibo888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ijm.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kyv.yj202588.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cam.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fwk.chenjidiqi.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://igq.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hil.vehdjk.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://utj.haohaochexian.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iqb.ivvv.top

[L06] 解析响应为 JSON
来源：http://gaf.zdqjudy.top

Py:   resp.json()
来源：http://thc.tianlin.xyz

PHP:  json_decode($body, true);
来源：http://oec.gotoacloud.top

JS:   await resp.json()
来源：http://tmi.gogol.net.cn

TS:   await resp.json()
来源：http://cvn.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wxr.hnqzz.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://whd.hcnkem.com

Ruby: JSON.parse(resp.body)
来源：http://gkw.hywenlv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qnl.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://wsa.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ilp.uphjek.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jrq.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://dpa.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://ihh.vqdsnc.cn

Java: resp.statusCode()
来源：http://ypc.meibo888.top

Go:   resp.StatusCode
来源：http://evw.shangyingyoupin.top

Ruby: resp.code.to_i
来源：http://djb.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://suy.yuanzhike.top

[L08] 并发请求多个地址
来源：http://eox.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eue.yj20258.top

PHP:  curl_multi_init() 系列
来源：http://qfx.uphjek.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ilj.redwolf501.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bbr.sysykeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ede.yongpay.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tsp.fanxiaobao.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qks.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lnn.hongshengwenyu.top

================================================================================
来源：http://uge.yj20258888.top

M. 命令行 / 进程 / 环境
来源：http://ope.yanxiufei.cn

================================================================================
来源：http://zob.chenjidiqi.icu

[M01] 读取命令行参数
来源：http://ewj.xziqi.cn

Py:   sys.argv[1:]
来源：http://reh.jqgfzy.top

PHP:  $argv;  $argc;
来源：http://gaf.sysykeji.top

JS:   process.argv.slice(2)
来源：http://qqk.xingfuxueyuan.xyz

TS:   process.argv.slice(2)
来源：http://xui.cashguo.top

Java: args 数组（main 方法参数）
来源：http://fey.shuidangran.top

Go:   os.Args[1:]
来源：http://vdo.yuanzhike.top

Ruby: ARGV
来源：http://ezp.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://azy.ydjk.org.cn

[M02] 读取环境变量
来源：http://qzf.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://lqm.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wyp.xinyue.icu

JS:   process.env.HOME
来源：http://xll.zhijiandao.cn

TS:   process.env.HOME
来源：http://ptx.316326.xyz

Java: System.getenv("HOME")
来源：http://jir.shanyushiyangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gvr.fktsv.cn

Ruby: ENV["HOME"]
来源：http://gfm.hfpthk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fgw.feifeiyinyue.top

[M03] 执行外部命令
来源：http://uou.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nwi.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ier.iojbl.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wdu.chenlongwang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hlk.ehwqpu.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rhk.epnwcf.com

Go:   exec.Command("ls", "-l").Output()
来源：http://iml.ywan-chungtsiang.top

Ruby: system("ls -l");  `ls -l`
来源：http://nsv.cucudq.cn

C#:   Process.Start("ls", "-l");
来源：http://qio.yongpay.top

[M04] 获取当前工作目录
来源：http://cxb.zhixingplan.top

Py:   os.getcwd()
来源：http://hfo.shangyingyoupin.top

PHP:  getcwd();
来源：http://mlb.xuanzx.com

JS:   process.cwd()
来源：http://zvi.mhx1999.top

TS:   process.cwd()
来源：http://tkq.yj20258.top

Java: Path.of("").toAbsolutePath()
来源：http://sob.nanxinkj.top

Go:   os.Getwd()
来源：http://ufp.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://mnw.ctjpmb.com

C#:   Directory.GetCurrentDirectory()
来源：http://ovx.gzhubu.top

[M05] 设置退出码
来源：http://fni.xuanzx.com

Py:   sys.exit(1)
来源：http://zdz.epnwcf.com

PHP:  exit(1);
来源：http://rgf.0kj1m.cn

JS:   process.exit(1)
来源：http://pft.epnwcf.com

TS:   process.exit(1)
来源：http://kps.epnwcf.com

Java: System.exit(1)
来源：http://arp.cdnleiting.top

Go:   os.Exit(1)
来源：http://zxq.gotoacloud.top

Ruby: exit 1
来源：http://kud.pycfn.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sho.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://fck.hysaishi.cn

Py:   print("err", file=sys.stderr)
来源：http://sbz.birdmap.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ufi.hysaishi.cn

JS:   console.error("err")
来源：http://edz.ivvv.top

TS:   console.error("err")
来源：http://keh.daria6918.cn

Java: System.err.println("err")
来源：http://iga.shanyushiyangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wxv.smart0.xyz

Ruby: warn "err"
来源：http://flj.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://lhx.shzxlz.cn

[M07] 判断是否为主入口
来源：http://upy.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://wyr.sufxvd.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gwa.wangdashe.top

JS:   require.main === module
来源：http://mks.zhijiandao.cn

TS:   require.main === module
来源：http://hfn.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://srg.shuidangran.top

Go:   func main()
来源：http://psr.tarul.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://giw.hnxiangtu.top

C#:   static void Main(string[] args)
来源：http://imm.chenjidiqi.icu

[M08] 获取系统与运行时信息
来源：http://gxl.tarul.cn

Py:   platform.system();  platform.python_version()
来源：http://ywg.cdnleiting.top

PHP:  PHP_OS;  phpversion();
来源：http://mbm.ivvv.top

JS:   process.platform;  process.version
来源：http://ard.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://wcg.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zsl.snrcjt.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gjy.fehbvm.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jnn.meibo888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dpg.cheryme.top

================================================================================
来源：http://rga.fktsv.cn

N. 数据结构与算法
来源：http://ugs.fehbvm.com

================================================================================
来源：http://izp.cashguo.top

[N01] 二分查找（有序数组）
来源：http://kku.dianchejie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://axw.zhiwuduotai.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bza.yueranfly.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eea.hesvh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wsu.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xvk.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://lgw.fktsv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hdl.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://jsw.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://sey.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://vuc.guannengcc.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hkk.vehdjk.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://yjh.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://jkb.nanxuanxn.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kgi.fktsv.cn

Go:   slices.Sort(arr)
来源：http://xpp.pycfn.com

Ruby: arr.sort
来源：http://bfj.sweek.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rmq.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://uab.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://drc.yfazqb.com

PHP:  // 递归实现，或用 usort
来源：http://jdx.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nsx.xziqi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xdg.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jxh.gogol.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ckp.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://upu.52xcode.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cza.cashguo.top

[N04] 斐波那契数列
来源：http://cns.shuidangran.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ytw.xingfuxueyuan.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sxg.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kfl.jqgfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ehu.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xtc.cqqwz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jes.vqdsnc.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gyr.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gmt.xingfuxueyuan.xyz

[N05] 最大公约数
来源：http://wgl.yj202588.top

Py:   math.gcd(a, b)
来源：http://suy.yuanzhike.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oek.wangshuangyany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dhx.shangyingyoupin.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vpm.aizwys.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zxq.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://urh.chenjidiqi.icu

Ruby: a.gcd(b)
来源：http://eci.cdnleiting.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uqv.yj20258.top

[N06] 判断回文字符串
来源：http://qxe.jqgfzy.top

Py:   s == s[::-1]
来源：http://vnn.ybcxt.top

PHP:  $s === strrev($s);
来源：http://lez.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://vef.xuanzx.com

TS:   s === [...s].reverse().join("")
来源：http://goe.jinqigufen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://snk.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://dqo.ywan-chungtsiang.top

Ruby: s == s.reverse
来源：http://cyq.snrcjt.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://iiu.havefunace.top

[N07] 两数之和（返回下标）
来源：http://vxd.daria6918.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cnu.hfpthk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://thf.redwolf501.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mry.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://gdf.chenzaomai.com

Java: // 手写 HashMap
来源：http://lfm.jianghu66.top

Go:   // 手写 map[int]int
来源：http://hax.jinqigufen.top

Ruby: // 手写 Hash
来源：http://jmt.316326.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://yaf.tian-w.cn

[N08] 生成全排列
来源：http://sbt.sjlbkw.cn

Py:   itertools.permutations(arr)
来源：http://igm.yj20258888.top

PHP:  // 手写递归交换
来源：http://bqd.xylfe.cn

JS:   // 手写回溯递归
来源：http://eqw.fanxiaobao.xyz

TS:   // 手写回溯递归
来源：http://hdz.aibaodan.cn

Java: // 手写回溯递归
来源：http://pmi.shangyingyoupin.top

Go:   // 手写回溯递归
来源：http://bld.tianlin.xyz

Ruby: arr.permutation.to_a
来源：http://ukv.iojbl.cn

C#:   // 手写回溯递归
来源：http://pee.havefunace.top

[N09] 栈与队列
来源：http://wnq.zhaomingkeji.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kvx.andypj.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kei.uphjek.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mhr.jinqigufen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eov.meibo888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eaa.nanxuanxn.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dcs.nanxinkj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eir.vehdjk.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lgh.yj202588.top

[N10] 链表节点定义
来源：http://vyv.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nyh.andypj.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://vry.hnxiangtu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://odu.zhongyouzk.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hvd.redwolf501.top

Java: class Node { int v; Node next; }
来源：http://bhj.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://txs.ivvv.top

Ruby: Node = Struct.new(:v, :next)
来源：http://isx.nanxinkj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wgn.daxiang520.top

[N11] 二叉树中序遍历
来源：http://shn.mhx1999.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ntd.sufxvd.cn

PHP:  // 手写递归函数
来源：http://wyf.havefunace.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kch.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sps.sweek.top

Java: // 手写递归
来源：http://xjw.gogol.net.cn

Go:   // 手写递归
来源：http://zim.gzhubu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ioo.fehbvm.com

C#:   // 手写递归
来源：http://ypz.zhongyouzk.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vcy.xingfuxueyuan.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vuz.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fwo.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eon.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bvb.ydzc1.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lhb.pengpengdd.cyou

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ifm.yfazqb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zhg.nwbrower.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nfg.dianchejie.cn

================================================================================
来源：http://mba.zhoulong.xyz

O. 并发与异步
来源：http://xjv.hammf.cn

================================================================================
来源：http://dvh.ywan-chungtsiang.top

[O01] 启动一个线程
来源：http://rrn.fehbvm.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vng.xziqi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vuv.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cld.sxryk.cn

TS:   // 同 JS
来源：http://pgi.gogol.net.cn

Java: new Thread(() -> f()).start()
来源：http://bdn.gotoacloud.top

Go:   go f()
来源：http://kul.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://kdt.jinghuilouyu.cn

C#:   Task.Run(() => F());
来源：http://rzk.yongpay.top

[O02] 使用线程池
来源：http://neq.cheryme.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jof.birdmap.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rro.snrcjt.cn

JS:   // worker_threads 线程池
来源：http://ciq.sufxvd.cn

TS:   // worker_threads 线程池
来源：http://ntz.mhx1999.top

Java: Executors.newFixedThreadPool(4)
来源：http://sbp.wangdashe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://plk.yj20258888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bvi.316326.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ila.fzhhl.top

[O03] 加锁保护共享数据
来源：http://otg.yj20258888.top

Py:   with lock: shared += 1
来源：http://rkb.sufxvd.cn

PHP:  // 用 flock() 做文件锁
来源：http://ovc.52xcode.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tjs.fanxiaobao.xyz

TS:   // 同 JS
来源：http://wsc.yvedp.cn

Java: synchronized (this) { shared++; }
来源：http://xzp.xylfe.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nuh.316326.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://qsq.andypj.xyz

C#:   lock (gate) { shared++; }
来源：http://ydu.shanyushiyangtech.top

[O04] 定义异步函数并等待
来源：http://lbj.hysaishi.cn

Py:   async def f():⏎    await g()
来源：http://lgs.cheryme.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ggm.andypj.xyz

JS:   async function f() { await g(); }
来源：http://gxq.yonumen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fff.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wio.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zop.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://kfc.yj20258.top

C#:   async Task F() { await G(); }
来源：http://mnv.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://thf.sysykeji.top

Py:   asyncio.gather(*tasks)
来源：http://zue.vehdjk.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hdc.epnwcf.com

JS:   await Promise.all(tasks)
来源：http://mab.fzhhl.top

TS:   await Promise.all(tasks)
来源：http://xcb.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fta.wangdashe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://snp.redwolf501.top

Ruby: threads.map(&:join)
来源：http://hcu.jlsjyb.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dyp.chenzaomai.com


<!-- 参考信息 -->