代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rqi.aibaodan.cn

JS:   await fetch(url)
来源：http://pqg.cdnleiting.top

TS:   await fetch(url)
来源：http://mxw.bbcook.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://njw.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://bcf.yvedp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dfz.zdbjq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bmq.mhx1999.top

[L02] 发送 POST JSON
来源：http://wnt.shangyingyoupin.top

Py:   requests.post(url, json={"a": 1})
来源：http://kfd.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ykg.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rvv.zdbjq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://stb.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fjk.quarkkingdee.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hve.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://suu.cqqwz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pea.shuidangran.top

[L03] 设置自定义请求头
来源：http://amt.jqgfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vkb.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jhl.316326.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kpm.nanxuanxn.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kwe.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tsx.cqqwz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://obv.chenzaomai.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://drl.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lod.snrcjt.cn

[L04] 设置超时
来源：http://adn.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://vks.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://byy.wangdashe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cpb.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ymt.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ndn.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rhh.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bwo.bjfxy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gby.redwolf501.top

[L05] 上传文件（multipart）
来源：http://nlr.yvedp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xjg.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nvk.nwbrower.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://myc.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://moh.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ddg.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pcm.0kj1m.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ivg.yongpay.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sga.chenjidiqi.icu

[L06] 解析响应为 JSON
来源：http://lde.tianlin.xyz

Py:   resp.json()
来源：http://stf.daria6918.cn

PHP:  json_decode($body, true);
来源：http://zjt.ydjk.org.cn

JS:   await resp.json()
来源：http://bql.tian-w.cn

TS:   await resp.json()
来源：http://pmi.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qpn.svipenyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pia.hywenlv.cn

Ruby: JSON.parse(resp.body)
来源：http://gpo.iojbl.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qtj.zhengqikj.top

[L07] 处理 HTTP 状态码
来源：http://zba.tianlin.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://abd.0kj1m.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ype.xuanzx.com

JS:   resp.ok;  resp.status
来源：http://avl.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://ojg.ywan-chungtsiang.top

Java: resp.statusCode()
来源：http://zwb.tian-w.cn

Go:   resp.StatusCode
来源：http://bnn.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://fox.tian-w.cn

C#:   (int)resp.StatusCode
来源：http://vwg.gzhubu.top

[L08] 并发请求多个地址
来源：http://drv.zhengqikj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ejn.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://lxm.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hqq.yfazqb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sma.yj202588.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eqw.zhoulong.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dfv.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oob.zhaomingkeji.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wzs.bjfxy.top

================================================================================
来源：http://lnp.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://err.wangdashe.top

================================================================================
来源：http://uwb.fengsongda.top

[M01] 读取命令行参数
来源：http://jmp.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://ppf.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://fza.redwolf501.top

JS:   process.argv.slice(2)
来源：http://egx.jlsjyb.cn

TS:   process.argv.slice(2)
来源：http://yuc.shzxlz.cn

Java: args 数组（main 方法参数）
来源：http://ebg.andypj.xyz

Go:   os.Args[1:]
来源：http://pna.xingfuxueyuan.xyz

Ruby: ARGV
来源：http://hdw.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://ddv.sysykeji.top

[M02] 读取环境变量
来源：http://hcf.zhijiandao.cn

Py:   os.environ.get("HOME")
来源：http://wer.ehwqpu.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nhj.nanxuanxn.top

JS:   process.env.HOME
来源：http://szx.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://vaz.yangfankeji.com

Java: System.getenv("HOME")
来源：http://sno.chenjidiqi.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wnv.yongpay.top

Ruby: ENV["HOME"]
来源：http://nub.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xrk.9152youxi.cn

[M03] 执行外部命令
来源：http://hol.daria6918.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ryx.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fdh.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hqe.c1oappe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ydq.redwolf501.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kif.sweek.top

Go:   exec.Command("ls", "-l").Output()
来源：http://apk.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://zzy.yuanzhike.top

C#:   Process.Start("ls", "-l");
来源：http://vgg.sxryk.cn

[M04] 获取当前工作目录
来源：http://jfr.jinqigufen.top

Py:   os.getcwd()
来源：http://tcv.ctjpmb.com

PHP:  getcwd();
来源：http://nhc.pengpengdd.cyou

JS:   process.cwd()
来源：http://rcd.wangshuangyany.cn

TS:   process.cwd()
来源：http://wbc.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://xek.ppjwa.cn

Go:   os.Getwd()
来源：http://vma.hesvh.cn

Ruby: Dir.pwd
来源：http://beh.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://zbo.xuetiantiany.cn

[M05] 设置退出码
来源：http://lcj.jlsjyb.cn

Py:   sys.exit(1)
来源：http://sru.yuanzhike.top

PHP:  exit(1);
来源：http://seq.yj20258.top

JS:   process.exit(1)
来源：http://hau.daxiang520.top

TS:   process.exit(1)
来源：http://cso.yangfankeji.com

Java: System.exit(1)
来源：http://duj.chenjidiqi.icu

Go:   os.Exit(1)
来源：http://cnz.dashuyun.cn

Ruby: exit 1
来源：http://qdi.hnxiangtu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pzz.pengpengdd.cyou

[M06] 向标准错误输出
来源：http://emu.jinghuilouyu.cn

Py:   print("err", file=sys.stderr)
来源：http://alt.chenlongwang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ypm.bjfxy.top

JS:   console.error("err")
来源：http://vtq.ydjk.org.cn

TS:   console.error("err")
来源：http://lpt.shanyushiyangtech.top

Java: System.err.println("err")
来源：http://oty.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fcd.wangdashe.top

Ruby: warn "err"
来源：http://orm.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://fpy.tianlin.xyz

[M07] 判断是否为主入口
来源：http://kwo.tarul.cn

Py:   if __name__ == "__main__":
来源：http://xsu.haohaochexian.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sav.dianchejie.cn

JS:   require.main === module
来源：http://msh.ybcxt.top

TS:   require.main === module
来源：http://jis.jianghu66.top

Java: public static void main(String[] args)
来源：http://upd.birdmap.top

Go:   func main()
来源：http://oom.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fby.yj20258.top

C#:   static void Main(string[] args)
来源：http://ihz.chenlongwang.top

[M08] 获取系统与运行时信息
来源：http://nno.tanke756.top

Py:   platform.system();  platform.python_version()
来源：http://abm.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://avc.epnwcf.com

JS:   process.platform;  process.version
来源：http://run.vehdjk.com

TS:   process.platform;  process.version
来源：http://zdl.yj202588.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ens.tanke756.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ihu.sjlbkw.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nzz.kuanghao11.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ivz.vqdsnc.cn

================================================================================
来源：http://pbw.yvedp.cn

N. 数据结构与算法
来源：http://cyd.hammf.cn

================================================================================
来源：http://ybv.yj20258888.top

[N01] 二分查找（有序数组）
来源：http://bdv.gaohongyu789.top

Py:   bisect.bisect_left(arr, x)
来源：http://vsi.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mjw.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://plf.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mqc.52xcode.cn

Java: Arrays.binarySearch(arr, x)
来源：http://eoz.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://hpb.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://rjw.sxryk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pxi.yj20258888.top

[N02] 排序（工程实践用内置实现）
来源：http://wtc.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://qpu.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qiw.yuanzhike.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ped.svipenyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vqd.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://emp.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://rzr.ydjk.org.cn

Ruby: arr.sort
来源：http://bbr.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://amw.yangfankeji.com

[N03] 快速排序（分治示例）
来源：http://oms.yangfankeji.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ufm.wangdashe.top

PHP:  // 递归实现，或用 usort
来源：http://emc.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rjr.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zmk.jianghu66.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tqh.yongpay.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://adf.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eis.snrcjt.cn

C#:   // 手写递归，或 Array.Sort
来源：http://edp.vehdjk.com

[N04] 斐波那契数列
来源：http://kpg.wangshuangyany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mey.cucudq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://axa.quarkkingdee.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://muf.hesvh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://log.ybcxt.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yzv.9152youxi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://euo.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qsd.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ypb.yfazqb.com

[N05] 最大公约数
来源：http://yji.cashguo.top

Py:   math.gcd(a, b)
来源：http://zgt.sufxvd.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sts.yongpay.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oyx.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://noz.chenjidiqi.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xwb.daria6918.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ipx.jinghuilouyu.cn

Ruby: a.gcd(b)
来源：http://vza.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kqn.ehwqpu.com

[N06] 判断回文字符串
来源：http://owk.ehwqpu.com

Py:   s == s[::-1]
来源：http://ahq.c1oappe.top

PHP:  $s === strrev($s);
来源：http://zdy.9152youxi.cn

JS:   s === [...s].reverse().join("")
来源：http://nrs.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://zqa.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sta.shuidangran.top

Go:   // 双指针从两端比较
来源：http://vbc.hfpthk.cn

Ruby: s == s.reverse
来源：http://laq.yj20258888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tyd.pengpengdd.cyou

[N07] 两数之和（返回下标）
来源：http://yvi.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://njd.jqgfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vwz.vqdsnc.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wgr.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://cas.zhixingplan.top

Java: // 手写 HashMap
来源：http://fby.smart0.xyz

Go:   // 手写 map[int]int
来源：http://gge.ctjpmb.com

Ruby: // 手写 Hash
来源：http://wxu.yj20258.top

C#:   // 手写 Dictionary<int, int>
来源：http://jou.jianghu66.top

[N08] 生成全排列
来源：http://use.hcnkem.com

Py:   itertools.permutations(arr)
来源：http://zox.bbcook.cn

PHP:  // 手写递归交换
来源：http://pnj.gotoacloud.top

JS:   // 手写回溯递归
来源：http://xqi.ybcxt.top

TS:   // 手写回溯递归
来源：http://wnu.yangfankeji.com

Java: // 手写回溯递归
来源：http://das.tian-w.cn

Go:   // 手写回溯递归
来源：http://oug.dianchejie.cn

Ruby: arr.permutation.to_a
来源：http://xrj.guannengcc.top

C#:   // 手写回溯递归
来源：http://pzl.ydzc1.top

[N09] 栈与队列
来源：http://kny.yongpay.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oml.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yko.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cnd.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wrx.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mya.nanxuanxn.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bwj.vehdjk.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pta.chenjidiqi.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rbp.ehwqpu.com

[N10] 链表节点定义
来源：http://uwp.redwolf501.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yoe.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qgd.hesvh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uvk.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dbe.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://zsx.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qup.shanyushiyangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zfq.shanyushiyangtech.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gpk.dashuyun.cn

[N11] 二叉树中序遍历
来源：http://vws.nanxinkj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ywx.yueranfly.top

PHP:  // 手写递归函数
来源：http://rla.jyoumei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qip.chenzaomai.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xsm.daria6918.cn

Java: // 手写递归
来源：http://kaj.chenjidiqi.icu

Go:   // 手写递归
来源：http://hlj.bbcook.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yqw.zhiwuduotai.top

C#:   // 手写递归
来源：http://plf.pycfn.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fmx.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rtw.zycfv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ghb.jianghu66.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qxm.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://amu.zhixingplan.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wwx.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://efv.bjfxy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ayh.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pvq.chenjidiqi.icu

================================================================================
来源：http://tki.xylfe.cn

O. 并发与异步
来源：http://uwi.pengpengdd.cyou

================================================================================
来源：http://avf.aizwys.cn

[O01] 启动一个线程
来源：http://fut.xuanzx.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wux.svipenyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fwz.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gpn.sjlbkw.cn

TS:   // 同 JS
来源：http://oyu.yvedp.cn

Java: new Thread(() -> f()).start()
来源：http://sqt.pengpengdd.cyou

Go:   go f()
来源：http://xpl.kuanghao11.cn

Ruby: Thread.new { f }
来源：http://omh.chenjidiqi.icu

C#:   Task.Run(() => F());
来源：http://gar.gaohongyu789.top

[O02] 使用线程池
来源：http://djd.zhongyouzk.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://api.9152youxi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fnh.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://abj.tianlin.xyz

TS:   // worker_threads 线程池
来源：http://jpu.yangfankeji.com

Java: Executors.newFixedThreadPool(4)
来源：http://tvl.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uan.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://alp.yfazqb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sai.tian-w.cn

[O03] 加锁保护共享数据
来源：http://efp.jyoumei.cn

Py:   with lock: shared += 1
来源：http://sth.kuanghao11.cn

PHP:  // 用 flock() 做文件锁
来源：http://zbd.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mxs.yj20258888.top

TS:   // 同 JS
来源：http://bho.cdnleiting.top

Java: synchronized (this) { shared++; }
来源：http://hxc.dashuyun.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gkx.zhixingplan.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xgn.jiagoushi.top

C#:   lock (gate) { shared++; }
来源：http://gii.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://ccq.c1oappe.top

Py:   async def f():⏎    await g()
来源：http://jww.fehbvm.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uuq.316326.xyz

JS:   async function f() { await g(); }
来源：http://ozt.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ejj.chenlongwang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rgw.yfazqb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://avx.52xcode.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cai.hesvh.cn

C#:   async Task F() { await G(); }
来源：http://lqz.cqqwz.cn

[O05] 并发执行并等待全部完成
来源：http://uqr.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://xix.redwolf501.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aco.jinqigfzy.top

JS:   await Promise.all(tasks)
来源：http://hcn.fehbvm.com

TS:   await Promise.all(tasks)
来源：http://art.dianchejie.cn


<!-- 参考信息 -->