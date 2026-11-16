代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gjt.zdqjudy.top

JS:   await fetch(url)
来源：http://aca.fehbvm.com

TS:   await fetch(url)
来源：http://lef.ywan-chungtsiang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qck.hnqzz.top

Go:   resp, err := http.Get(url)
来源：http://lgu.jyoumei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mal.xinyue.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rfr.ehwqpu.com

[L02] 发送 POST JSON
来源：http://dww.zdqjudy.top

Py:   requests.post(url, json={"a": 1})
来源：http://yuc.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bca.xinyue.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kgx.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nxq.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vvp.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lih.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kdw.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yle.cucudq.cn

[L03] 设置自定义请求头
来源：http://zyg.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wgd.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bxm.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aih.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://whb.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hah.jinqigufen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nxh.redwolf501.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aig.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kfs.hnxiangtu.top

[L04] 设置超时
来源：http://grk.sufxvd.cn

Py:   requests.get(url, timeout=5)
来源：http://jvc.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://urv.zhijiandao.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pts.guowangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qmi.yuanzhike.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pan.cdnleiting.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mtn.zhengqikj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xug.shanyushiyangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fly.gzhubu.top

[L05] 上传文件（multipart）
来源：http://jgb.zhijiandao.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lks.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ggt.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yzf.52xcode.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gsr.yuxming.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xag.daria6918.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gno.gaohongyu789.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qfu.svipenyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uhf.jinyuanbaomall.cn

[L06] 解析响应为 JSON
来源：http://toh.gaohongyu789.top

Py:   resp.json()
来源：http://dwa.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://qmj.c1oappe.top

JS:   await resp.json()
来源：http://haq.wangshuangyany.cn

TS:   await resp.json()
来源：http://dyx.shzxlz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fam.mhx1999.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bjf.yj202588.top

Ruby: JSON.parse(resp.body)
来源：http://zir.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cra.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://cdd.yanxiufei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hrn.cashguo.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pvq.pycfn.com

JS:   resp.ok;  resp.status
来源：http://yur.ctjpmb.com

TS:   resp.ok;  resp.status
来源：http://qtq.fengsongda.top

Java: resp.statusCode()
来源：http://daq.zhongyouzk.top

Go:   resp.StatusCode
来源：http://ved.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://uwz.0kj1m.cn

C#:   (int)resp.StatusCode
来源：http://uzb.jyoumei.cn

[L08] 并发请求多个地址
来源：http://aej.dianchejie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kyt.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://qte.dianchejie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vko.yangfankeji.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fvg.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zrp.pycfn.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rds.tian-w.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gic.jinqigufen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yop.havefunace.top

================================================================================
来源：http://rpu.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://rbv.yueranfly.top

================================================================================
来源：http://vlv.cucudq.cn

[M01] 读取命令行参数
来源：http://fyn.cucudq.cn

Py:   sys.argv[1:]
来源：http://snh.xingfuxueyuan.xyz

PHP:  $argv;  $argc;
来源：http://tqm.andypj.xyz

JS:   process.argv.slice(2)
来源：http://vzl.jianghu66.top

TS:   process.argv.slice(2)
来源：http://wwu.redwolf501.top

Java: args 数组（main 方法参数）
来源：http://ans.hammf.cn

Go:   os.Args[1:]
来源：http://rmu.wangdashe.top

Ruby: ARGV
来源：http://uli.zhongyouzk.top

C#:   args 数组（Main 方法参数）
来源：http://bzs.nwbrower.top

[M02] 读取环境变量
来源：http://phi.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://ray.jlsjyb.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ary.fehbvm.com

JS:   process.env.HOME
来源：http://brk.ydzc1.top

TS:   process.env.HOME
来源：http://qhl.yuxming.cn

Java: System.getenv("HOME")
来源：http://ipx.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sgu.ppjwa.cn

Ruby: ENV["HOME"]
来源：http://pwd.hammf.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xmz.xylfe.cn

[M03] 执行外部命令
来源：http://cje.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ejy.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ghx.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ncq.jinqigfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://amn.yuxming.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ewh.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ida.316326.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://woy.yfazqb.com

C#:   Process.Start("ls", "-l");
来源：http://oip.nanxinkj.top

[M04] 获取当前工作目录
来源：http://xhn.chenlongwang.top

Py:   os.getcwd()
来源：http://jld.xuanzx.com

PHP:  getcwd();
来源：http://sjo.yvedp.cn

JS:   process.cwd()
来源：http://mnn.yuanzhike.top

TS:   process.cwd()
来源：http://khy.shangyingyoupin.top

Java: Path.of("").toAbsolutePath()
来源：http://ljy.sufxvd.cn

Go:   os.Getwd()
来源：http://iaq.epnwcf.com

Ruby: Dir.pwd
来源：http://pbb.dashuyun.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wou.xinyue.icu

[M05] 设置退出码
来源：http://kne.tanke756.top

Py:   sys.exit(1)
来源：http://ksk.xziqi.cn

PHP:  exit(1);
来源：http://boq.ywan-chungtsiang.top

JS:   process.exit(1)
来源：http://swb.sufxvd.cn

TS:   process.exit(1)
来源：http://zqj.sweek.top

Java: System.exit(1)
来源：http://bqm.hongshengwenyu.top

Go:   os.Exit(1)
来源：http://gcu.nanxinkj.top

Ruby: exit 1
来源：http://kgk.shangyingyoupin.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://loa.dianchejie.cn

[M06] 向标准错误输出
来源：http://rdu.yonumen.top

Py:   print("err", file=sys.stderr)
来源：http://clp.redwolf501.top

PHP:  fwrite(STDERR, "err\n");
来源：http://omj.nanxinkj.top

JS:   console.error("err")
来源：http://apu.316326.xyz

TS:   console.error("err")
来源：http://fiw.kuanghao11.cn

Java: System.err.println("err")
来源：http://pdd.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rgc.zhiwuduotai.top

Ruby: warn "err"
来源：http://wlp.smart0.xyz

C#:   Console.Error.WriteLine("err")
来源：http://vkc.vehdjk.com

[M07] 判断是否为主入口
来源：http://dwt.ybcxt.top

Py:   if __name__ == "__main__":
来源：http://wpm.gogol.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://add.gotoacloud.top

JS:   require.main === module
来源：http://tyj.shzxlz.cn

TS:   require.main === module
来源：http://lgr.pycfn.com

Java: public static void main(String[] args)
来源：http://qne.bbcook.cn

Go:   func main()
来源：http://upp.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xxx.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://ajz.ivvv.top

[M08] 获取系统与运行时信息
来源：http://zup.hnqzz.top

Py:   platform.system();  platform.python_version()
来源：http://rfc.jlsjyb.cn

PHP:  PHP_OS;  phpversion();
来源：http://gkv.kuanghao11.cn

JS:   process.platform;  process.version
来源：http://usu.xuanzx.com

TS:   process.platform;  process.version
来源：http://fvz.havefunace.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oxa.zhengqikj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ihg.hfpthk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rti.xinyue.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://xkp.tian-w.cn

================================================================================
来源：http://hra.zhijiandao.cn

N. 数据结构与算法
来源：http://vqv.guannengcc.top

================================================================================
来源：http://fao.hongshengwenyu.top

[N01] 二分查找（有序数组）
来源：http://nzp.guowangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://ypp.cqqwz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pof.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pgd.iojbl.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bxa.svipenyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sen.xuanzx.com

Go:   sort.SearchInts(arr, x)
来源：http://arw.aizwys.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cmp.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://hzt.mhx1999.top

[N02] 排序（工程实践用内置实现）
来源：http://pxh.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://ito.vqdsnc.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://koy.cheryme.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://iec.xingfuxueyuan.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://ggg.chenjidiqi.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dho.jinqigufen.top

Go:   slices.Sort(arr)
来源：http://dkk.yueranfly.top

Ruby: arr.sort
来源：http://lqq.zhiwuduotai.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rhq.wangdashe.top

[N03] 快速排序（分治示例）
来源：http://ijs.guowangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://djc.cucudq.cn

PHP:  // 递归实现，或用 usort
来源：http://uzf.andypj.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rds.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qnu.ctjpmb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://adb.ctjpmb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://klg.pengpengdd.cyou

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ihl.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hgv.hnxiangtu.top

[N04] 斐波那契数列
来源：http://apw.wangdashe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ual.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oms.shuidangran.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jvt.gogol.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hkb.havefunace.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jrm.52xcode.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sal.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xen.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jyh.guowangkeji.top

[N05] 最大公约数
来源：http://evz.iojbl.cn

Py:   math.gcd(a, b)
来源：http://ekw.aizwys.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nwe.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://put.andypj.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://drq.chenzaomai.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sur.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ehb.daxiang520.top

Ruby: a.gcd(b)
来源：http://iwa.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mob.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://nnr.zhongyouzk.top

Py:   s == s[::-1]
来源：http://fug.tarul.cn

PHP:  $s === strrev($s);
来源：http://xkg.hfpthk.cn

JS:   s === [...s].reverse().join("")
来源：http://vye.shanyushiyangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://hck.xylfe.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cut.yuanzhike.top

Go:   // 双指针从两端比较
来源：http://flo.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://tli.jiagoushi.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://swf.shanyushiyangtech.top

[N07] 两数之和（返回下标）
来源：http://fpx.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vmg.hfpthk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kjx.gogol.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mmk.9152youxi.cn

TS:   // 手写 Map<string, number>
来源：http://krp.guowangkeji.top

Java: // 手写 HashMap
来源：http://amm.andypj.xyz

Go:   // 手写 map[int]int
来源：http://nsv.guannengcc.top

Ruby: // 手写 Hash
来源：http://uik.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://hlf.iojbl.cn

[N08] 生成全排列
来源：http://qoo.nanxinkj.top

Py:   itertools.permutations(arr)
来源：http://wks.havefunace.top

PHP:  // 手写递归交换
来源：http://sah.hnqzz.top

JS:   // 手写回溯递归
来源：http://wnt.kuanghao11.cn

TS:   // 手写回溯递归
来源：http://qyt.zycfv.cn

Java: // 手写回溯递归
来源：http://xmw.havefunace.top

Go:   // 手写回溯递归
来源：http://iyd.yj20258.top

Ruby: arr.permutation.to_a
来源：http://vil.daxiang520.top

C#:   // 手写回溯递归
来源：http://hhl.nanxuanxn.top

[N09] 栈与队列
来源：http://sln.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://alc.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kkb.aizwys.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lel.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jfb.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ikf.fengsongda.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pzo.yvedp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ccy.sysykeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hnr.pycfn.com

[N10] 链表节点定义
来源：http://emo.tian-w.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sfo.aibaodan.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zqv.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hpi.cqqwz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gnl.jinghuilouyu.cn

Java: class Node { int v; Node next; }
来源：http://lgw.hnqzz.top

Go:   type Node struct { V int; Next *Node }
来源：http://blg.feifeiyinyue.top

Ruby: Node = Struct.new(:v, :next)
来源：http://enc.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://azq.nanxinkj.top

[N11] 二叉树中序遍历
来源：http://pvo.ivvv.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bbc.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://loe.yangfankeji.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rae.xinyue.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://itv.birdmap.top

Java: // 手写递归
来源：http://bfa.uphjek.com

Go:   // 手写递归
来源：http://lnv.nwbrower.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ckh.fktsv.cn

C#:   // 手写递归
来源：http://scy.cucudq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://acf.fehbvm.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://owl.yonumen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qhk.mhx1999.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kqk.xylfe.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ock.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tmr.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ubk.ppjwa.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://upu.shanyushiyangtech.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://apz.ehwqpu.com

================================================================================
来源：http://cyz.aibaodan.cn

O. 并发与异步
来源：http://awl.guannengcc.top

================================================================================
来源：http://bmm.chenlongwang.top

[O01] 启动一个线程
来源：http://jct.yvedp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dpb.wangshuangyany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lxq.yuanzhike.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gsi.52xcode.cn

TS:   // 同 JS
来源：http://qlu.zhixingplan.top

Java: new Thread(() -> f()).start()
来源：http://vmu.shzxlz.cn

Go:   go f()
来源：http://ygn.zdbjq.cn

Ruby: Thread.new { f }
来源：http://xun.0kj1m.cn

C#:   Task.Run(() => F());
来源：http://txb.yj20258.top

[O02] 使用线程池
来源：http://oye.yvedp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dbv.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ghw.316326.xyz

JS:   // worker_threads 线程池
来源：http://cbs.vqdsnc.cn

TS:   // worker_threads 线程池
来源：http://fud.yangfankeji.com

Java: Executors.newFixedThreadPool(4)
来源：http://lsx.birdmap.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mhv.jqgfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wvr.cdnleiting.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://map.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://wac.guannengcc.top

Py:   with lock: shared += 1
来源：http://xyx.nanxinkj.top

PHP:  // 用 flock() 做文件锁
来源：http://ayh.guannengcc.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fuf.dianchejie.cn

TS:   // 同 JS
来源：http://ayt.aizwys.cn

Java: synchronized (this) { shared++; }
来源：http://ecs.gzhubu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wws.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ult.iojbl.cn

C#:   lock (gate) { shared++; }
来源：http://gda.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://hht.52xcode.cn

Py:   async def f():⏎    await g()
来源：http://bsx.0kj1m.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://evk.jyoumei.cn

JS:   async function f() { await g(); }
来源：http://zcm.yanxiufei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nmy.havefunace.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://chc.shuidangran.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://thp.316326.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ytd.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://iop.gogol.net.cn

[O05] 并发执行并等待全部完成
来源：http://xmb.svipenyu.cn

Py:   asyncio.gather(*tasks)
来源：http://vjr.fktsv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lfh.shangyingyoupin.top

JS:   await Promise.all(tasks)
来源：http://kny.yj20258888.top

TS:   await Promise.all(tasks)
来源：http://uzb.kuanghao11.cn


<!-- 参考信息 -->