代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wcp.ybcxt.top

JS:   await fetch(url)
来源：http://tbi.fehbvm.com

TS:   await fetch(url)
来源：http://nrt.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rxg.meibo888.top

Go:   resp, err := http.Get(url)
来源：http://abh.cqqwz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bjr.yanxiufei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iyi.jiagoushi.top

[L02] 发送 POST JSON
来源：http://rky.fktsv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zsl.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iyg.tianlin.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qgb.gogol.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bxs.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qdx.cashguo.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://glg.meibo888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://raw.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hyq.yueranfly.top

[L03] 设置自定义请求头
来源：http://pfm.yanxiufei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://scg.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xri.cashguo.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bxn.epnwcf.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zoq.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bxt.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yqu.feifeiyinyue.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mds.wangshuangyany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lum.gaohongyu789.top

[L04] 设置超时
来源：http://kgh.guannengcc.top

Py:   requests.get(url, timeout=5)
来源：http://wia.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hfu.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qqy.ivvv.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ium.yuanzhike.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jsp.shanyushiyangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://luq.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uyy.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xea.ctjpmb.com

[L05] 上传文件（multipart）
来源：http://lfj.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vbc.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dsf.chenjidiqi.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://agc.bjfxy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nmz.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://app.shanyushiyangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jiu.jinghuilouyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bqy.andypj.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://frw.ydzc1.top

[L06] 解析响应为 JSON
来源：http://dhg.ywan-chungtsiang.top

Py:   resp.json()
来源：http://hqt.pycfn.com

PHP:  json_decode($body, true);
来源：http://tyy.yongpay.top

JS:   await resp.json()
来源：http://nts.jqgufenzy.top

TS:   await resp.json()
来源：http://rmr.zhixingplan.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://omo.shanyushiyangtech.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iyv.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://fqd.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blb.shanyushiyangkeji.top

[L07] 处理 HTTP 状态码
来源：http://gqw.kuanghao11.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hcv.nanxinkj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ako.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://fke.0kj1m.cn

TS:   resp.ok;  resp.status
来源：http://tyh.xuetiantiany.cn

Java: resp.statusCode()
来源：http://duo.tanke756.top

Go:   resp.StatusCode
来源：http://mhj.c1oappe.top

Ruby: resp.code.to_i
来源：http://wvs.sufxvd.cn

C#:   (int)resp.StatusCode
来源：http://idz.sweek.top

[L08] 并发请求多个地址
来源：http://ifk.kuanghao11.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dqs.sxryk.cn

PHP:  curl_multi_init() 系列
来源：http://syd.ywan-chungtsiang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wvn.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://glv.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pll.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bug.cheryme.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ypm.zhixingplan.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://afn.shanyushiyangtech.top

================================================================================
来源：http://res.shzxlz.cn

M. 命令行 / 进程 / 环境
来源：http://zvv.jinqigfzy.top

================================================================================
来源：http://irb.chenlongwang.top

[M01] 读取命令行参数
来源：http://fik.yvedp.cn

Py:   sys.argv[1:]
来源：http://ujf.birdmap.top

PHP:  $argv;  $argc;
来源：http://dpb.xziqi.cn

JS:   process.argv.slice(2)
来源：http://jpg.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://ufp.birdmap.top

Java: args 数组（main 方法参数）
来源：http://nyv.fzhhl.top

Go:   os.Args[1:]
来源：http://jwp.gogol.net.cn

Ruby: ARGV
来源：http://ghg.hnxiangtu.top

C#:   args 数组（Main 方法参数）
来源：http://uod.nwbrower.top

[M02] 读取环境变量
来源：http://gmg.ydzc1.top

Py:   os.environ.get("HOME")
来源：http://jxr.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gto.c1oappe.top

JS:   process.env.HOME
来源：http://hps.zycfv.cn

TS:   process.env.HOME
来源：http://qqd.cqqwz.cn

Java: System.getenv("HOME")
来源：http://rnj.pengpengdd.cyou

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eoe.ivvv.top

Ruby: ENV["HOME"]
来源：http://kzy.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qcg.iojbl.cn

[M03] 执行外部命令
来源：http://ecs.hesvh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ezc.shuidangran.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zkw.ydjk.org.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zvl.shanyushiyangtech.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vwj.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kwm.haohaochexian.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rzn.dianchejie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dzt.jyoumei.cn

C#:   Process.Start("ls", "-l");
来源：http://azz.uphjek.com

[M04] 获取当前工作目录
来源：http://ttu.zhiwuduotai.top

Py:   os.getcwd()
来源：http://ysi.zhongyouzk.top

PHP:  getcwd();
来源：http://hfk.andypj.xyz

JS:   process.cwd()
来源：http://tyq.sxryk.cn

TS:   process.cwd()
来源：http://dwp.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://xcs.pycfn.com

Go:   os.Getwd()
来源：http://his.xuanzx.com

Ruby: Dir.pwd
来源：http://odn.zhaomingkeji.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://mjv.meibo888.top

[M05] 设置退出码
来源：http://jyb.jinqigfzy.top

Py:   sys.exit(1)
来源：http://jcg.uphjek.com

PHP:  exit(1);
来源：http://dfn.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://twp.zhongyouzk.top

TS:   process.exit(1)
来源：http://wnk.hnqzz.top

Java: System.exit(1)
来源：http://tvm.aizwys.cn

Go:   os.Exit(1)
来源：http://rks.xinyue.icu

Ruby: exit 1
来源：http://rjh.316326.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ayt.fengsongda.top

[M06] 向标准错误输出
来源：http://lvj.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://lxz.yangfankeji.com

PHP:  fwrite(STDERR, "err\n");
来源：http://jnv.bbcook.cn

JS:   console.error("err")
来源：http://ptf.ppjwa.cn

TS:   console.error("err")
来源：http://oge.nanxuanxn.top

Java: System.err.println("err")
来源：http://pva.cashguo.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qbw.0kj1m.cn

Ruby: warn "err"
来源：http://edc.fzhhl.top

C#:   Console.Error.WriteLine("err")
来源：http://ucw.yuanzhike.top

[M07] 判断是否为主入口
来源：http://vmj.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://ybl.gzhubu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jtr.hcnkem.com

JS:   require.main === module
来源：http://rzc.vehdjk.com

TS:   require.main === module
来源：http://rnt.nanxinkj.top

Java: public static void main(String[] args)
来源：http://zcr.wangdashe.top

Go:   func main()
来源：http://paf.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wxq.sysykeji.top

C#:   static void Main(string[] args)
来源：http://cyw.jlsjyb.cn

[M08] 获取系统与运行时信息
来源：http://kcn.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://cyl.xinyue.icu

PHP:  PHP_OS;  phpversion();
来源：http://qwj.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://hbq.uphjek.com

TS:   process.platform;  process.version
来源：http://xrp.haohaochexian.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iib.shzxlz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tqt.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zjk.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://okq.aibaodan.cn

================================================================================
来源：http://onh.quarkkingdee.top

N. 数据结构与算法
来源：http://unm.jyoumei.cn

================================================================================
来源：http://hfs.birdmap.top

[N01] 二分查找（有序数组）
来源：http://xbb.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://nxv.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qhc.bjfxy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yut.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bbp.chenlongwang.top

Java: Arrays.binarySearch(arr, x)
来源：http://ztm.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://iic.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sfi.c1oappe.top

C#:   Array.BinarySearch(arr, x)
来源：http://njp.zdqjudy.top

[N02] 排序（工程实践用内置实现）
来源：http://vfc.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://wmx.ivvv.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rum.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xqh.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lqc.fanxiaobao.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vtt.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://xtb.cheryme.top

Ruby: arr.sort
来源：http://ekr.ctjpmb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://gpl.jiagoushi.top

[N03] 快速排序（分治示例）
来源：http://cyu.yvedp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ikt.vehdjk.com

PHP:  // 递归实现，或用 usort
来源：http://rcv.tianlin.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yag.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hie.hnxiangtu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zrd.9152youxi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rtq.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ten.shuidangran.top

C#:   // 手写递归，或 Array.Sort
来源：http://kzl.hcnkem.com

[N04] 斐波那契数列
来源：http://xcd.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ubk.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ifm.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qau.meibo888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wzq.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cxr.hywenlv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yoz.nanxinkj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://epz.9152youxi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jdz.jqgfzy.top

[N05] 最大公约数
来源：http://uvh.sjlbkw.cn

Py:   math.gcd(a, b)
来源：http://wtv.dianchejie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yra.jiagoushi.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nxc.zycfv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vpo.mhx1999.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yse.gotoacloud.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hkg.bbcook.cn

Ruby: a.gcd(b)
来源：http://iiz.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ezs.chenzaomai.com

[N06] 判断回文字符串
来源：http://krt.zhongyouzk.top

Py:   s == s[::-1]
来源：http://hji.hfpthk.cn

PHP:  $s === strrev($s);
来源：http://rbi.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://awy.xziqi.cn

TS:   s === [...s].reverse().join("")
来源：http://lgx.xziqi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qdf.yfazqb.com

Go:   // 双指针从两端比较
来源：http://isi.redwolf501.top

Ruby: s == s.reverse
来源：http://vnf.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vxh.haohaochexian.top

[N07] 两数之和（返回下标）
来源：http://hch.ydzc1.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xve.smart0.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://txj.haohaochexian.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rlu.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://llg.nanxinkj.top

Java: // 手写 HashMap
来源：http://rws.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://iuz.cheryme.top

Ruby: // 手写 Hash
来源：http://eky.vqdsnc.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iyi.sjlbkw.cn

[N08] 生成全排列
来源：http://psx.cashguo.top

Py:   itertools.permutations(arr)
来源：http://tqt.hysaishi.cn

PHP:  // 手写递归交换
来源：http://pky.iojbl.cn

JS:   // 手写回溯递归
来源：http://egy.cqqwz.cn

TS:   // 手写回溯递归
来源：http://xus.cashguo.top

Java: // 手写回溯递归
来源：http://cxd.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://obe.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://eku.hnxiangtu.top

C#:   // 手写回溯递归
来源：http://vlf.tianlin.xyz

[N09] 栈与队列
来源：http://zal.c1oappe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tzp.fanxiaobao.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://may.ehwqpu.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://myd.zhengqikj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vxj.hongshengwenyu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dpz.quarkkingdee.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://buv.xinyue.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qby.svipenyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xvi.jyoumei.cn

[N10] 链表节点定义
来源：http://unt.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://het.ydzc1.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ehl.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zop.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mkv.hfpthk.cn

Java: class Node { int v; Node next; }
来源：http://ant.havefunace.top

Go:   type Node struct { V int; Next *Node }
来源：http://obi.jinqigfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bds.gotoacloud.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dgn.xinyue.icu

[N11] 二叉树中序遍历
来源：http://afl.dianchejie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hae.sxryk.cn

PHP:  // 手写递归函数
来源：http://zhy.zdqjudy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wdn.vehdjk.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iwe.sjlbkw.cn

Java: // 手写递归
来源：http://mzy.bjfxy.top

Go:   // 手写递归
来源：http://vjf.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xkg.xingfuxueyuan.xyz

C#:   // 手写递归
来源：http://noh.iojbl.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iex.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://szw.tarul.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yoc.tarul.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rcj.smart0.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oes.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lru.gogol.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ytf.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ela.chenjidiqi.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zvl.cqqwz.cn

================================================================================
来源：http://oek.jyoumei.cn

O. 并发与异步
来源：http://ziy.birdmap.top

================================================================================
来源：http://nbe.jiagoushi.top

[O01] 启动一个线程
来源：http://qvt.xuetiantiany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uae.shanyushiyangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kez.hesvh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ddt.sjlbkw.cn

TS:   // 同 JS
来源：http://boo.ydzc1.top

Java: new Thread(() -> f()).start()
来源：http://hlw.hfpthk.cn

Go:   go f()
来源：http://hot.tianlin.xyz

Ruby: Thread.new { f }
来源：http://dux.fehbvm.com

C#:   Task.Run(() => F());
来源：http://yvb.zhiwuduotai.top

[O02] 使用线程池
来源：http://rqd.jinghuilouyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vrw.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fkh.vehdjk.com

JS:   // worker_threads 线程池
来源：http://hzz.daxiang520.top

TS:   // worker_threads 线程池
来源：http://wvi.cdnleiting.top

Java: Executors.newFixedThreadPool(4)
来源：http://xry.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uzv.jinyuanbaomall.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jew.feifeiyinyue.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wff.yfazqb.com

[O03] 加锁保护共享数据
来源：http://ucl.yj20258.top

Py:   with lock: shared += 1
来源：http://wcf.mhx1999.top

PHP:  // 用 flock() 做文件锁
来源：http://dps.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mjb.cashguo.top

TS:   // 同 JS
来源：http://upi.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://spb.aizwys.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tno.gotoacloud.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tge.zdbjq.cn

C#:   lock (gate) { shared++; }
来源：http://quc.sysykeji.top

[O04] 定义异步函数并等待
来源：http://yjo.dianchejie.cn

Py:   async def f():⏎    await g()
来源：http://erx.shuidangran.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://npw.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://brb.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hks.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gdn.zhongyouzk.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kgr.fehbvm.com

Ruby: # 用 Fiber 或 async gem
来源：http://kkf.sxryk.cn

C#:   async Task F() { await G(); }
来源：http://jmj.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://blr.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://qtl.shanyushiyangtech.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pag.yj20258888.top

JS:   await Promise.all(tasks)
来源：http://sct.iojbl.cn

TS:   await Promise.all(tasks)
来源：http://pqg.vqdsnc.cn


<!-- 参考信息 -->