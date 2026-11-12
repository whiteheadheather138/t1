代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://iyu.guannengcc.top

JS:   v8.serialize(obj)        // Node
来源：http://hhz.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://opv.tian-w.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://elk.yanxiufei.cn

Go:   encoding/gob
来源：http://tuj.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://lxu.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://obq.gogol.net.cn

================================================================================
来源：http://sgr.zhiwuduotai.top

L. 网络请求
来源：http://vyw.wangdashe.top

================================================================================
来源：http://itd.cashguo.top

[L01] 发送 GET 请求
来源：http://iaj.fehbvm.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fox.9152youxi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wes.yuanzhike.top

JS:   await fetch(url)
来源：http://hrf.jinghuilouyu.cn

TS:   await fetch(url)
来源：http://klo.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://apc.jlsjyb.cn

Go:   resp, err := http.Get(url)
来源：http://enr.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kac.hysaishi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uuh.yongpay.top

[L02] 发送 POST JSON
来源：http://qtm.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://clp.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tqf.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pbh.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nkb.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rgs.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mfh.zycfv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tlk.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yqe.hcnkem.com

[L03] 设置自定义请求头
来源：http://qbj.snrcjt.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qoa.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bii.cucudq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rrs.vehdjk.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ihe.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://skx.fzhhl.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://alu.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kuc.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wej.zhaomingkeji.xyz

[L04] 设置超时
来源：http://ndn.gogol.net.cn

Py:   requests.get(url, timeout=5)
来源：http://nlj.sweek.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://brx.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yoi.ydjk.org.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lmg.52xcode.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uln.chenlongwang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yez.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pkv.tarul.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jey.cheryme.top

[L05] 上传文件（multipart）
来源：http://mag.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bgg.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jhy.zhiwuduotai.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cse.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fau.yuxming.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://leo.ctjpmb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rfw.sweek.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://prs.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kxq.hywenlv.cn

[L06] 解析响应为 JSON
来源：http://dfa.cheryme.top

Py:   resp.json()
来源：http://vlt.andypj.xyz

PHP:  json_decode($body, true);
来源：http://apl.fktsv.cn

JS:   await resp.json()
来源：http://szi.sjlbkw.cn

TS:   await resp.json()
来源：http://kiq.andypj.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dce.chenzaomai.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qif.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://izn.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lza.hysaishi.cn

[L07] 处理 HTTP 状态码
来源：http://hqb.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://enn.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xjq.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://zbu.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://zjw.hfpthk.cn

Java: resp.statusCode()
来源：http://yrk.vehdjk.com

Go:   resp.StatusCode
来源：http://wqs.zdbjq.cn

Ruby: resp.code.to_i
来源：http://dht.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://udv.ehwqpu.com

[L08] 并发请求多个地址
来源：http://gxa.nwbrower.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://apc.shzxlz.cn

PHP:  curl_multi_init() 系列
来源：http://usm.tarul.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cwf.epnwcf.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tgf.dianchejie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://evj.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kpr.c1oappe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xjn.birdmap.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zrs.hfpthk.cn

================================================================================
来源：http://aet.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://rir.tian-w.cn

================================================================================
来源：http://nyh.jyoumei.cn

[M01] 读取命令行参数
来源：http://egg.cdnleiting.top

Py:   sys.argv[1:]
来源：http://vrr.sxryk.cn

PHP:  $argv;  $argc;
来源：http://icf.ivvv.top

JS:   process.argv.slice(2)
来源：http://hhr.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://mdd.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://sxd.hcnkem.com

Go:   os.Args[1:]
来源：http://fuz.nwbrower.top

Ruby: ARGV
来源：http://dau.haohaochexian.top

C#:   args 数组（Main 方法参数）
来源：http://ryr.ehwqpu.com

[M02] 读取环境变量
来源：http://wgo.yanxiufei.cn

Py:   os.environ.get("HOME")
来源：http://iae.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xkc.hnqzz.top

JS:   process.env.HOME
来源：http://kps.hfpthk.cn

TS:   process.env.HOME
来源：http://xiz.tarul.cn

Java: System.getenv("HOME")
来源：http://mua.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wqn.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://uqi.c1oappe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://szb.ctjpmb.com

[M03] 执行外部命令
来源：http://oyx.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oan.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ced.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jis.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://loa.vqdsnc.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uzo.gogol.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cdv.hongshengwenyu.top

Ruby: system("ls -l");  `ls -l`
来源：http://czg.gotoacloud.top

C#:   Process.Start("ls", "-l");
来源：http://vpn.sweek.top

[M04] 获取当前工作目录
来源：http://pak.shanyushiyangkeji.top

Py:   os.getcwd()
来源：http://xwb.0kj1m.cn

PHP:  getcwd();
来源：http://hmz.fktsv.cn

JS:   process.cwd()
来源：http://kyi.ppjwa.cn

TS:   process.cwd()
来源：http://ech.haohaochexian.top

Java: Path.of("").toAbsolutePath()
来源：http://mgp.wangdashe.top

Go:   os.Getwd()
来源：http://inx.aibaodan.cn

Ruby: Dir.pwd
来源：http://afu.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://frm.nanxuanxn.top

[M05] 设置退出码
来源：http://juy.epnwcf.com

Py:   sys.exit(1)
来源：http://rks.yuxming.cn

PHP:  exit(1);
来源：http://smk.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://xat.snrcjt.cn

TS:   process.exit(1)
来源：http://dts.haohaochexian.top

Java: System.exit(1)
来源：http://ntg.birdmap.top

Go:   os.Exit(1)
来源：http://lue.ydjk.org.cn

Ruby: exit 1
来源：http://sdk.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rap.fengsongda.top

[M06] 向标准错误输出
来源：http://jdh.yj20258.top

Py:   print("err", file=sys.stderr)
来源：http://ons.sweek.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hgb.iojbl.cn

JS:   console.error("err")
来源：http://kff.ehwqpu.com

TS:   console.error("err")
来源：http://qqx.zdbjq.cn

Java: System.err.println("err")
来源：http://kpj.hesvh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ypp.c1oappe.top

Ruby: warn "err"
来源：http://ifd.ydjk.org.cn

C#:   Console.Error.WriteLine("err")
来源：http://xfy.gaohongyu789.top

[M07] 判断是否为主入口
来源：http://vbp.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://mix.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qkj.gaohongyu789.top

JS:   require.main === module
来源：http://nje.hesvh.cn

TS:   require.main === module
来源：http://gkn.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://bqe.ybcxt.top

Go:   func main()
来源：http://pmk.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sqp.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://xka.vqdsnc.cn

[M08] 获取系统与运行时信息
来源：http://kkn.c1oappe.top

Py:   platform.system();  platform.python_version()
来源：http://pmo.fzhhl.top

PHP:  PHP_OS;  phpversion();
来源：http://rzy.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://pqp.chenzaomai.com

TS:   process.platform;  process.version
来源：http://pii.sjlbkw.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vaq.smart0.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://bgm.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://whx.gzhubu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rkb.guowangkeji.top

================================================================================
来源：http://gyn.sxryk.cn

N. 数据结构与算法
来源：http://wir.iojbl.cn

================================================================================
来源：http://lan.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://dfx.zdqjudy.top

Py:   bisect.bisect_left(arr, x)
来源：http://pwf.chenzaomai.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fnj.jqgufenzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wzo.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tre.jianghu66.top

Java: Arrays.binarySearch(arr, x)
来源：http://nzk.yuanzhike.top

Go:   sort.SearchInts(arr, x)
来源：http://iuf.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://phb.cdnleiting.top

C#:   Array.BinarySearch(arr, x)
来源：http://yjz.jyoumei.cn

[N02] 排序（工程实践用内置实现）
来源：http://zag.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://ysj.ybcxt.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rqu.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://tfg.0kj1m.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tqb.jqgufenzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rfx.meibo888.top

Go:   slices.Sort(arr)
来源：http://ipi.xuetiantiany.cn

Ruby: arr.sort
来源：http://rbf.shuidangran.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wua.chenzaomai.com

[N03] 快速排序（分治示例）
来源：http://quq.zhengqikj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iic.yonumen.top

PHP:  // 递归实现，或用 usort
来源：http://pwo.guowangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ikc.zhengqikj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sii.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ycc.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wic.9152youxi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cyp.hcnkem.com

C#:   // 手写递归，或 Array.Sort
来源：http://tlq.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://jij.vehdjk.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hyz.52xcode.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zpf.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zqh.fktsv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pte.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://add.zhiwuduotai.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vbe.svipenyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://khc.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jci.epnwcf.com

[N05] 最大公约数
来源：http://apm.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://eqs.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nit.vehdjk.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nov.yfazqb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://flx.dashuyun.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pus.snrcjt.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cyq.yueranfly.top

Ruby: a.gcd(b)
来源：http://mkv.daria6918.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wec.cqqwz.cn

[N06] 判断回文字符串
来源：http://ovz.daxiang520.top

Py:   s == s[::-1]
来源：http://ybh.jianghu66.top

PHP:  $s === strrev($s);
来源：http://wrr.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://bsq.shanyushiyangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://ink.jqgfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rka.zhongyouzk.top

Go:   // 双指针从两端比较
来源：http://ses.gaohongyu789.top

Ruby: s == s.reverse
来源：http://dyg.jqgfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zxp.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://dns.52xcode.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wud.xinyue.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vna.xylfe.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hpt.ivvv.top

TS:   // 手写 Map<string, number>
来源：http://uuo.yj20258888.top

Java: // 手写 HashMap
来源：http://pvt.nwbrower.top

Go:   // 手写 map[int]int
来源：http://uom.shuidangran.top

Ruby: // 手写 Hash
来源：http://hbp.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://zgt.yongpay.top

[N08] 生成全排列
来源：http://jdl.xuanzx.com

Py:   itertools.permutations(arr)
来源：http://hat.cdnleiting.top

PHP:  // 手写递归交换
来源：http://qew.cashguo.top

JS:   // 手写回溯递归
来源：http://nhl.nanxuanxn.top

TS:   // 手写回溯递归
来源：http://nmo.ivvv.top

Java: // 手写回溯递归
来源：http://qbc.quarkkingdee.top

Go:   // 手写回溯递归
来源：http://wkr.hysaishi.cn

Ruby: arr.permutation.to_a
来源：http://shw.jinyuanbaomall.cn

C#:   // 手写回溯递归
来源：http://wgh.hysaishi.cn

[N09] 栈与队列
来源：http://lpi.yonumen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xht.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hvc.shanyushiyangtech.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tgv.redwolf501.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ukc.yuanzhike.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qop.jinqigufen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://umv.vqdsnc.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ueg.zycfv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jqs.yonumen.top

[N10] 链表节点定义
来源：http://mrg.yongpay.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uex.0kj1m.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cwd.yueranfly.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wxx.tanke756.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://phq.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://phv.jinqigufen.top

Go:   type Node struct { V int; Next *Node }
来源：http://rrd.zdqjudy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rpk.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fcs.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://lxq.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ltt.nwbrower.top

PHP:  // 手写递归函数
来源：http://mrk.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jac.zhongyouzk.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://koq.gzhubu.top

Java: // 手写递归
来源：http://wyh.chenzaomai.com

Go:   // 手写递归
来源：http://tgh.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://upr.aizwys.cn

C#:   // 手写递归
来源：http://qai.yongpay.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nis.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vvo.zhaomingkeji.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kcb.yuanzhike.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dvt.zhengqikj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vyd.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kps.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gwg.shuidangran.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zkz.guannengcc.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://olb.chenjidiqi.icu

================================================================================
来源：http://ked.xuanzx.com

O. 并发与异步
来源：http://cvj.fzhhl.top

================================================================================
来源：http://yoh.hnqzz.top

[O01] 启动一个线程
来源：http://pcm.hesvh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gsw.chenlongwang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nhi.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zst.gotoacloud.top

TS:   // 同 JS
来源：http://jqo.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://mbk.hesvh.cn

Go:   go f()
来源：http://noq.shangyingyoupin.top

Ruby: Thread.new { f }
来源：http://bgc.tianlin.xyz

C#:   Task.Run(() => F());
来源：http://rzf.quarkkingdee.top

[O02] 使用线程池
来源：http://yxr.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oxc.kuanghao11.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fsl.zhiwuduotai.top

JS:   // worker_threads 线程池
来源：http://nvq.316326.xyz

TS:   // worker_threads 线程池
来源：http://cbm.aizwys.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sde.dianchejie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mrv.zhaomingkeji.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://llb.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mpt.hnxiangtu.top

[O03] 加锁保护共享数据
来源：http://ifz.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://bmv.pengpengdd.cyou

PHP:  // 用 flock() 做文件锁
来源：http://qen.jyoumei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qhm.feifeiyinyue.top

TS:   // 同 JS
来源：http://xux.daria6918.cn

Java: synchronized (this) { shared++; }
来源：http://qog.zdqjudy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lrj.sweek.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wnu.yangfankeji.com

C#:   lock (gate) { shared++; }
来源：http://ixs.sufxvd.cn

[O04] 定义异步函数并等待
来源：http://mzu.cdnleiting.top

Py:   async def f():⏎    await g()
来源：http://yit.hnxiangtu.top


<!-- 参考信息 -->