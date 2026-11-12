代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uge.zhongyouzk.top

JS:   await fetch(url)
来源：http://bgg.xinyue.icu

TS:   await fetch(url)
来源：http://ret.meibo888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ush.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://wrb.jinghuilouyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oeq.gaohongyu789.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fyb.guannengcc.top

[L02] 发送 POST JSON
来源：http://hax.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://nez.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://trx.cqqwz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://auq.xuanzx.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://htk.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sil.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zej.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rse.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pxf.shanyushiyangkeji.top

[L03] 设置自定义请求头
来源：http://vjh.shanyushiyangtech.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xjl.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lgv.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://afr.feifeiyinyue.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gzm.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rmx.daria6918.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kzh.nanxinkj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gfw.yj202588.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jsp.fengsongda.top

[L04] 设置超时
来源：http://fko.yfazqb.com

Py:   requests.get(url, timeout=5)
来源：http://ajo.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://udb.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dwv.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lqu.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://csj.sweek.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://arc.zhoulong.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://avc.nwbrower.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vgd.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://hbd.fehbvm.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ntc.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://byg.bbcook.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vax.shanyushiyangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ujl.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rnv.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zgz.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sbp.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jvs.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://tez.jinghuilouyu.cn

Py:   resp.json()
来源：http://ybb.zhiwuduotai.top

PHP:  json_decode($body, true);
来源：http://qvi.hnqzz.top

JS:   await resp.json()
来源：http://fko.zhixingplan.top

TS:   await resp.json()
来源：http://enm.guowangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ijd.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gmp.zycfv.cn

Ruby: JSON.parse(resp.body)
来源：http://wos.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vhs.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://zqy.yanxiufei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nwf.ctjpmb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://svq.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://ijj.zhiwuduotai.top

TS:   resp.ok;  resp.status
来源：http://gnr.jinyuanbaomall.cn

Java: resp.statusCode()
来源：http://heu.hcnkem.com

Go:   resp.StatusCode
来源：http://ssl.xuetiantiany.cn

Ruby: resp.code.to_i
来源：http://yam.gotoacloud.top

C#:   (int)resp.StatusCode
来源：http://imj.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://lin.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zyd.nanxinkj.top

PHP:  curl_multi_init() 系列
来源：http://uks.haohaochexian.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aov.zdbjq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kdr.smart0.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://idm.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bvc.wangdashe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ebt.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://btf.xziqi.cn

================================================================================
来源：http://dhv.sweek.top

M. 命令行 / 进程 / 环境
来源：http://zub.chenlongwang.top

================================================================================
来源：http://xdt.ybcxt.top

[M01] 读取命令行参数
来源：http://dyb.tian-w.cn

Py:   sys.argv[1:]
来源：http://lcb.jinqigufen.top

PHP:  $argv;  $argc;
来源：http://kvu.jqgufenzy.top

JS:   process.argv.slice(2)
来源：http://nkx.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://wmv.jinghuilouyu.cn

Java: args 数组（main 方法参数）
来源：http://tqg.sxryk.cn

Go:   os.Args[1:]
来源：http://cqg.ivvv.top

Ruby: ARGV
来源：http://smj.tanke756.top

C#:   args 数组（Main 方法参数）
来源：http://sdb.ppjwa.cn

[M02] 读取环境变量
来源：http://qxi.c1oappe.top

Py:   os.environ.get("HOME")
来源：http://pky.shzxlz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://atc.fktsv.cn

JS:   process.env.HOME
来源：http://gcy.fzhhl.top

TS:   process.env.HOME
来源：http://oik.pengpengdd.cyou

Java: System.getenv("HOME")
来源：http://cvi.sweek.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fxu.fktsv.cn

Ruby: ENV["HOME"]
来源：http://rgd.aibaodan.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ioh.ivvv.top

[M03] 执行外部命令
来源：http://eii.chenzaomai.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fma.hcnkem.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ppa.c1oappe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vfm.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://aux.hywenlv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lcb.ydzc1.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bhx.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://maa.bbcook.cn

C#:   Process.Start("ls", "-l");
来源：http://rld.guannengcc.top

[M04] 获取当前工作目录
来源：http://vzx.sjlbkw.cn

Py:   os.getcwd()
来源：http://tor.zhijiandao.cn

PHP:  getcwd();
来源：http://owl.uphjek.com

JS:   process.cwd()
来源：http://wpn.tianlin.xyz

TS:   process.cwd()
来源：http://cct.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://tzc.mhx1999.top

Go:   os.Getwd()
来源：http://pcm.daria6918.cn

Ruby: Dir.pwd
来源：http://qnp.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kcu.zdqjudy.top

[M05] 设置退出码
来源：http://ilu.gzhubu.top

Py:   sys.exit(1)
来源：http://huw.zhijiandao.cn

PHP:  exit(1);
来源：http://rsi.0kj1m.cn

JS:   process.exit(1)
来源：http://bmh.jinqigfzy.top

TS:   process.exit(1)
来源：http://zzr.9152youxi.cn

Java: System.exit(1)
来源：http://sqo.cheryme.top

Go:   os.Exit(1)
来源：http://tui.kuanghao11.cn

Ruby: exit 1
来源：http://pdo.redwolf501.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bwh.hammf.cn

[M06] 向标准错误输出
来源：http://lfn.gzhubu.top

Py:   print("err", file=sys.stderr)
来源：http://ckk.cucudq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lff.vehdjk.com

JS:   console.error("err")
来源：http://rvj.ywan-chungtsiang.top

TS:   console.error("err")
来源：http://wyk.zdbjq.cn

Java: System.err.println("err")
来源：http://wbf.shuidangran.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bwc.xziqi.cn

Ruby: warn "err"
来源：http://tpy.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://dnl.jqgfzy.top

[M07] 判断是否为主入口
来源：http://wrk.shangyingyoupin.top

Py:   if __name__ == "__main__":
来源：http://eju.yj20258.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tns.aibaodan.cn

JS:   require.main === module
来源：http://mms.svipenyu.cn

TS:   require.main === module
来源：http://eyq.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://hof.smart0.xyz

Go:   func main()
来源：http://zbr.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pkz.svipenyu.cn

C#:   static void Main(string[] args)
来源：http://vft.sjlbkw.cn

[M08] 获取系统与运行时信息
来源：http://elf.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://vgz.shuidangran.top

PHP:  PHP_OS;  phpversion();
来源：http://klv.shanyushiyangtech.top

JS:   process.platform;  process.version
来源：http://lkp.andypj.xyz

TS:   process.platform;  process.version
来源：http://xeo.cdnleiting.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lkt.andypj.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://gyk.kuanghao11.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uwa.bbcook.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://imd.gotoacloud.top

================================================================================
来源：http://ula.shzxlz.cn

N. 数据结构与算法
来源：http://rvz.chenjidiqi.icu

================================================================================
来源：http://dxc.tanke756.top

[N01] 二分查找（有序数组）
来源：http://akm.zhixingplan.top

Py:   bisect.bisect_left(arr, x)
来源：http://ckb.chenlongwang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zef.aibaodan.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jiv.hysaishi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wlx.xuanzx.com

Java: Arrays.binarySearch(arr, x)
来源：http://gjk.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://cuf.dianchejie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wxt.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://tgi.dianchejie.cn

[N02] 排序（工程实践用内置实现）
来源：http://jow.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://pef.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ymh.mhx1999.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kej.kuanghao11.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xmj.daxiang520.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zkh.nanxinkj.top

Go:   slices.Sort(arr)
来源：http://egw.gotoacloud.top

Ruby: arr.sort
来源：http://nep.cashguo.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wnb.shzxlz.cn

[N03] 快速排序（分治示例）
来源：http://yez.nwbrower.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yhf.iojbl.cn

PHP:  // 递归实现，或用 usort
来源：http://bvq.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pyd.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uqv.c1oappe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gvj.guannengcc.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cam.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rfh.yonumen.top

C#:   // 手写递归，或 Array.Sort
来源：http://hjo.zhiwuduotai.top

[N04] 斐波那契数列
来源：http://oel.nanxuanxn.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://klv.0kj1m.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fps.snrcjt.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sft.tianlin.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://usc.zhengqikj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ioj.aizwys.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://scz.hammf.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rvo.smart0.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ihe.gaohongyu789.top

[N05] 最大公约数
来源：http://src.hongshengwenyu.top

Py:   math.gcd(a, b)
来源：http://jgo.yueranfly.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ygd.yj202588.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hbs.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ulc.yfazqb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yux.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pcu.zhiwuduotai.top

Ruby: a.gcd(b)
来源：http://ypy.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://phs.ydjk.org.cn

[N06] 判断回文字符串
来源：http://ykz.jqgufenzy.top

Py:   s == s[::-1]
来源：http://efe.mhx1999.top

PHP:  $s === strrev($s);
来源：http://apq.redwolf501.top

JS:   s === [...s].reverse().join("")
来源：http://aue.wangdashe.top

TS:   s === [...s].reverse().join("")
来源：http://cif.ivvv.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wvo.ydjk.org.cn

Go:   // 双指针从两端比较
来源：http://fjw.zhijiandao.cn

Ruby: s == s.reverse
来源：http://yyu.redwolf501.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nhb.52xcode.cn

[N07] 两数之和（返回下标）
来源：http://bvu.hywenlv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eda.cucudq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vqz.jinyuanbaomall.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ufy.hesvh.cn

TS:   // 手写 Map<string, number>
来源：http://eto.0kj1m.cn

Java: // 手写 HashMap
来源：http://dca.dashuyun.cn

Go:   // 手写 map[int]int
来源：http://oty.yangfankeji.com

Ruby: // 手写 Hash
来源：http://tzu.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://qoi.316326.xyz

[N08] 生成全排列
来源：http://bvh.ppjwa.cn

Py:   itertools.permutations(arr)
来源：http://deu.ctjpmb.com

PHP:  // 手写递归交换
来源：http://dre.jianghu66.top

JS:   // 手写回溯递归
来源：http://fml.shanyushiyangkeji.top

TS:   // 手写回溯递归
来源：http://mka.yongpay.top

Java: // 手写回溯递归
来源：http://frh.hesvh.cn

Go:   // 手写回溯递归
来源：http://jqh.cqqwz.cn

Ruby: arr.permutation.to_a
来源：http://aag.ywan-chungtsiang.top

C#:   // 手写回溯递归
来源：http://nij.cucudq.cn

[N09] 栈与队列
来源：http://lpm.zycfv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://glv.ivvv.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tew.havefunace.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://itj.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mbs.tarul.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sku.zhengqikj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nzu.sjlbkw.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jzh.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://snp.hongshengwenyu.top

[N10] 链表节点定义
来源：http://cow.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zca.zhoulong.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://jzl.jlsjyb.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hlk.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wsq.dianchejie.cn

Java: class Node { int v; Node next; }
来源：http://bfu.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://kgh.aibaodan.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tlo.9152youxi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lrc.wangshuangyany.cn

[N11] 二叉树中序遍历
来源：http://vcj.shanyushiyangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mgc.tanke756.top

PHP:  // 手写递归函数
来源：http://azs.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qkv.chenzaomai.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fio.bjfxy.top

Java: // 手写递归
来源：http://ofe.pycfn.com

Go:   // 手写递归
来源：http://hww.ivvv.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mei.ydjk.org.cn

C#:   // 手写递归
来源：http://dvc.xuanzx.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xlp.jinghuilouyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tag.yj20258.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://huu.zdbjq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://giv.vqdsnc.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hsy.hammf.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nkv.ydzc1.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kab.smart0.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://unv.tianlin.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tdk.shangyingyoupin.top

================================================================================
来源：http://pta.cdnleiting.top

O. 并发与异步
来源：http://xxa.jinqigufen.top

================================================================================
来源：http://fep.xuetiantiany.cn

[O01] 启动一个线程
来源：http://qwe.tian-w.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://syh.jianghu66.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qwy.gogol.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://far.ppjwa.cn

TS:   // 同 JS
来源：http://vzs.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://udw.gogol.net.cn

Go:   go f()
来源：http://nfm.svipenyu.cn

Ruby: Thread.new { f }
来源：http://uvg.cheryme.top

C#:   Task.Run(() => F());
来源：http://vgh.jqgufenzy.top

[O02] 使用线程池
来源：http://npx.dianchejie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ryd.vqdsnc.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://exi.hesvh.cn

JS:   // worker_threads 线程池
来源：http://pnq.zhongyouzk.top

TS:   // worker_threads 线程池
来源：http://xnx.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://zrt.guowangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://scw.yonumen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uji.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pyd.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://qjl.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://pkx.zycfv.cn

PHP:  // 用 flock() 做文件锁
来源：http://tci.mhx1999.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dos.chenlongwang.top

TS:   // 同 JS
来源：http://fle.xuetiantiany.cn

Java: synchronized (this) { shared++; }
来源：http://ghe.jinqigfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uqx.316326.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://ohw.xinyue.icu

C#:   lock (gate) { shared++; }
来源：http://ixp.fktsv.cn

[O04] 定义异步函数并等待
来源：http://lzg.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://wxl.sxryk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vrx.ydzc1.top

JS:   async function f() { await g(); }
来源：http://qag.havefunace.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://edl.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fgi.jinqigfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fev.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nfy.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://gpu.xuetiantiany.cn

[O05] 并发执行并等待全部完成
来源：http://cao.zdqjudy.top

Py:   asyncio.gather(*tasks)
来源：http://jwr.yangfankeji.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://diw.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://nde.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://qye.zycfv.cn


<!-- 参考信息 -->