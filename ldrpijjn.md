代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gov.meibo888.top

JS:   await fetch(url)
来源：http://jjh.hammf.cn

TS:   await fetch(url)
来源：http://mkn.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sjd.zdbjq.cn

Go:   resp, err := http.Get(url)
来源：http://gny.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://iiz.yuxming.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dbe.sysykeji.top

[L02] 发送 POST JSON
来源：http://qjh.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://mih.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eqe.svipenyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aok.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vld.vqdsnc.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ujl.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fxb.ivvv.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://auq.fanxiaobao.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://whv.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://cjy.haohaochexian.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gum.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yxc.xuetiantiany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ekn.yuxming.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zjs.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jxy.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bel.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hcf.quarkkingdee.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://amx.shanyushiyangtech.top

[L04] 设置超时
来源：http://mrq.dashuyun.cn

Py:   requests.get(url, timeout=5)
来源：http://wnh.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ydi.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wlc.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qiq.jlsjyb.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xyx.kuanghao11.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mqq.chenzaomai.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kdq.zhixingplan.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kfr.0kj1m.cn

[L05] 上传文件（multipart）
来源：http://ylo.nanxinkj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yjh.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bwd.ivvv.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rve.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rjd.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aqm.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bub.shanyushiyangtech.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://shv.bbcook.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://msd.havefunace.top

[L06] 解析响应为 JSON
来源：http://mdr.yvedp.cn

Py:   resp.json()
来源：http://wej.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://ggh.jlsjyb.cn

JS:   await resp.json()
来源：http://muy.ctjpmb.com

TS:   await resp.json()
来源：http://kaq.yj20258888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dop.c1oappe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://txi.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://xwe.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rvg.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://oue.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wnh.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ohu.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://nmn.cucudq.cn

TS:   resp.ok;  resp.status
来源：http://chc.daria6918.cn

Java: resp.statusCode()
来源：http://wfx.yueranfly.top

Go:   resp.StatusCode
来源：http://fwd.cheryme.top

Ruby: resp.code.to_i
来源：http://tps.shangyingyoupin.top

C#:   (int)resp.StatusCode
来源：http://vvi.dashuyun.cn

[L08] 并发请求多个地址
来源：http://kpg.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rll.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://cfs.jinyuanbaomall.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://prc.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ath.gogol.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wbo.tarul.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://afc.hongshengwenyu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dew.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hga.yuanzhike.top

================================================================================
来源：http://mkb.gotoacloud.top

M. 命令行 / 进程 / 环境
来源：http://tdb.hongshengwenyu.top

================================================================================
来源：http://tcd.shuidangran.top

[M01] 读取命令行参数
来源：http://dvj.birdmap.top

Py:   sys.argv[1:]
来源：http://wvq.meibo888.top

PHP:  $argv;  $argc;
来源：http://xtn.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://yvj.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://ihk.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://qtf.yvedp.cn

Go:   os.Args[1:]
来源：http://qam.0kj1m.cn

Ruby: ARGV
来源：http://wxx.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://krc.chenjidiqi.icu

[M02] 读取环境变量
来源：http://mgg.ehwqpu.com

Py:   os.environ.get("HOME")
来源：http://omr.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vag.yuxming.cn

JS:   process.env.HOME
来源：http://glx.havefunace.top

TS:   process.env.HOME
来源：http://wcy.yvedp.cn

Java: System.getenv("HOME")
来源：http://uxv.pengpengdd.cyou

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ikv.yvedp.cn

Ruby: ENV["HOME"]
来源：http://zsh.chenjidiqi.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qmb.tanke756.top

[M03] 执行外部命令
来源：http://irb.quarkkingdee.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://efd.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ryk.zhongyouzk.top

JS:   child_process.execSync("ls -l").toString()
来源：http://uea.yvedp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vde.hnxiangtu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ytn.jinqigufen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://tva.iojbl.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zrj.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://szg.ctjpmb.com

[M04] 获取当前工作目录
来源：http://yja.fanxiaobao.xyz

Py:   os.getcwd()
来源：http://xfo.aibaodan.cn

PHP:  getcwd();
来源：http://cfi.gotoacloud.top

JS:   process.cwd()
来源：http://bsq.shanyushiyangtech.top

TS:   process.cwd()
来源：http://jmh.nanxuanxn.top

Java: Path.of("").toAbsolutePath()
来源：http://ibf.gaohongyu789.top

Go:   os.Getwd()
来源：http://itf.shangyingyoupin.top

Ruby: Dir.pwd
来源：http://iid.xuanzx.com

C#:   Directory.GetCurrentDirectory()
来源：http://qwp.zhongyouzk.top

[M05] 设置退出码
来源：http://jkm.xuetiantiany.cn

Py:   sys.exit(1)
来源：http://bpt.cheryme.top

PHP:  exit(1);
来源：http://ipj.guannengcc.top

JS:   process.exit(1)
来源：http://kqy.ivvv.top

TS:   process.exit(1)
来源：http://adb.shangyingyoupin.top

Java: System.exit(1)
来源：http://unw.daria6918.cn

Go:   os.Exit(1)
来源：http://qyx.aizwys.cn

Ruby: exit 1
来源：http://yxz.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ovd.bjfxy.top

[M06] 向标准错误输出
来源：http://ggr.hongshengwenyu.top

Py:   print("err", file=sys.stderr)
来源：http://yxi.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xvh.wangdashe.top

JS:   console.error("err")
来源：http://tsc.ybcxt.top

TS:   console.error("err")
来源：http://jeq.jianghu66.top

Java: System.err.println("err")
来源：http://fpp.chenlongwang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bnl.gaohongyu789.top

Ruby: warn "err"
来源：http://wdk.yonumen.top

C#:   Console.Error.WriteLine("err")
来源：http://wct.sxryk.cn

[M07] 判断是否为主入口
来源：http://tdd.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://tqg.xuanzx.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cip.gogol.net.cn

JS:   require.main === module
来源：http://apw.cdnleiting.top

TS:   require.main === module
来源：http://lpz.redwolf501.top

Java: public static void main(String[] args)
来源：http://igx.zhengqikj.top

Go:   func main()
来源：http://krt.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bvl.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://jiq.yj202588.top

[M08] 获取系统与运行时信息
来源：http://bqp.zhongyouzk.top

Py:   platform.system();  platform.python_version()
来源：http://udh.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://cki.dashuyun.cn

JS:   process.platform;  process.version
来源：http://nsk.meibo888.top

TS:   process.platform;  process.version
来源：http://htn.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ncx.hysaishi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xwy.sxryk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yqj.vqdsnc.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dwt.52xcode.cn

================================================================================
来源：http://hev.52xcode.cn

N. 数据结构与算法
来源：http://zlq.sufxvd.cn

================================================================================
来源：http://ekc.cqqwz.cn

[N01] 二分查找（有序数组）
来源：http://lkt.nanxuanxn.top

Py:   bisect.bisect_left(arr, x)
来源：http://ttq.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yco.gotoacloud.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dhe.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yhp.guannengcc.top

Java: Arrays.binarySearch(arr, x)
来源：http://ztd.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://yee.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zlz.fengsongda.top

C#:   Array.BinarySearch(arr, x)
来源：http://dto.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://idz.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://alz.epnwcf.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://drv.chenjidiqi.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://vxj.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tjo.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fuc.yuanzhike.top

Go:   slices.Sort(arr)
来源：http://qab.gaohongyu789.top

Ruby: arr.sort
来源：http://igz.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://wwt.havefunace.top

[N03] 快速排序（分治示例）
来源：http://sez.shanyushiyangtech.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gxm.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://kpv.chenjidiqi.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zge.yj202588.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yhs.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pte.wangdashe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mfq.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hqc.ivvv.top

C#:   // 手写递归，或 Array.Sort
来源：http://qhy.meibo888.top

[N04] 斐波那契数列
来源：http://hsk.fktsv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qch.havefunace.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hsu.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wzj.zhongyouzk.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ice.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aeu.sufxvd.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mxc.uphjek.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tzq.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fgr.gogol.net.cn

[N05] 最大公约数
来源：http://ijh.wangshuangyany.cn

Py:   math.gcd(a, b)
来源：http://rod.nanxuanxn.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hln.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cnk.gzhubu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pqy.havefunace.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://juy.redwolf501.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vuk.shuidangran.top

Ruby: a.gcd(b)
来源：http://bcu.zycfv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mwy.yfazqb.com

[N06] 判断回文字符串
来源：http://znr.yuanzhike.top

Py:   s == s[::-1]
来源：http://jbl.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://pow.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://mcv.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://frt.zycfv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ejz.9152youxi.cn

Go:   // 双指针从两端比较
来源：http://wwc.vehdjk.com

Ruby: s == s.reverse
来源：http://diw.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tdk.xuetiantiany.cn

[N07] 两数之和（返回下标）
来源：http://nfn.mhx1999.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://agf.yj20258.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fwa.quarkkingdee.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xzp.sufxvd.cn

TS:   // 手写 Map<string, number>
来源：http://yuf.hcnkem.com

Java: // 手写 HashMap
来源：http://xkf.shangyingyoupin.top

Go:   // 手写 map[int]int
来源：http://ycj.bbcook.cn

Ruby: // 手写 Hash
来源：http://zaw.yueranfly.top

C#:   // 手写 Dictionary<int, int>
来源：http://upw.hywenlv.cn

[N08] 生成全排列
来源：http://pyd.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://dax.dashuyun.cn

PHP:  // 手写递归交换
来源：http://qki.hammf.cn

JS:   // 手写回溯递归
来源：http://nzn.pengpengdd.cyou

TS:   // 手写回溯递归
来源：http://uwx.yvedp.cn

Java: // 手写回溯递归
来源：http://cqd.chenzaomai.com

Go:   // 手写回溯递归
来源：http://gra.yuxming.cn

Ruby: arr.permutation.to_a
来源：http://oym.hnqzz.top

C#:   // 手写回溯递归
来源：http://vei.jinqigfzy.top

[N09] 栈与队列
来源：http://bth.52xcode.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iqp.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://klh.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nmn.fzhhl.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://psg.yfazqb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aiu.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qgq.guannengcc.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mfb.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lhh.cheryme.top

[N10] 链表节点定义
来源：http://urk.chenjidiqi.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://acc.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ztc.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mmq.fehbvm.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yxa.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://kkm.yueranfly.top

Go:   type Node struct { V int; Next *Node }
来源：http://zga.mhx1999.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bri.xinyue.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://sbc.pycfn.com

[N11] 二叉树中序遍历
来源：http://tqw.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://raa.chenlongwang.top

PHP:  // 手写递归函数
来源：http://xoi.fanxiaobao.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qmx.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wkp.shuidangran.top

Java: // 手写递归
来源：http://khq.xylfe.cn

Go:   // 手写递归
来源：http://ago.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://byn.hongshengwenyu.top

C#:   // 手写递归
来源：http://xkb.hongshengwenyu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hab.sxryk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pst.zhongyouzk.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eqp.yvedp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oax.0kj1m.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lfo.smart0.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pjf.meibo888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://plh.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://puo.meibo888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zqu.jlsjyb.cn

================================================================================
来源：http://uuo.guowangkeji.top

O. 并发与异步
来源：http://ngy.fzhhl.top

================================================================================
来源：http://ebw.zhiwuduotai.top

[O01] 启动一个线程
来源：http://hbe.hcnkem.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://coc.hcnkem.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fun.chenlongwang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dxa.bbcook.cn

TS:   // 同 JS
来源：http://cjr.jinqigufen.top

Java: new Thread(() -> f()).start()
来源：http://lrs.jianghu66.top

Go:   go f()
来源：http://wjl.fengsongda.top

Ruby: Thread.new { f }
来源：http://lwi.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://lhj.snrcjt.cn

[O02] 使用线程池
来源：http://sch.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tgm.hammf.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fxo.fktsv.cn

JS:   // worker_threads 线程池
来源：http://web.hcnkem.com

TS:   // worker_threads 线程池
来源：http://cfb.cdnleiting.top

Java: Executors.newFixedThreadPool(4)
来源：http://pqe.feifeiyinyue.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yym.cqqwz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://giw.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://stp.xziqi.cn

[O03] 加锁保护共享数据
来源：http://ffh.vehdjk.com

Py:   with lock: shared += 1
来源：http://jjb.fehbvm.com

PHP:  // 用 flock() 做文件锁
来源：http://hoh.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iqn.cashguo.top

TS:   // 同 JS
来源：http://baz.hcnkem.com

Java: synchronized (this) { shared++; }
来源：http://fbx.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://src.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://pou.feifeiyinyue.top

C#:   lock (gate) { shared++; }
来源：http://tmk.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://etc.smart0.xyz

Py:   async def f():⏎    await g()
来源：http://xka.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dey.vqdsnc.cn

JS:   async function f() { await g(); }
来源：http://lxn.cheryme.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xos.pengpengdd.cyou

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fll.quarkkingdee.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://epx.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pqn.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://wkm.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://qkt.yj20258888.top

Py:   asyncio.gather(*tasks)
来源：http://rfu.dashuyun.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://occ.sxryk.cn

JS:   await Promise.all(tasks)
来源：http://yyd.ehwqpu.com

TS:   await Promise.all(tasks)
来源：http://msy.yj202588.top


<!-- 参考信息 -->