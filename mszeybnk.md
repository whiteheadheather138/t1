代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://ajv.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://xez.wangshuangyany.cn

TS:   v8.serialize(obj)        // Node
来源：http://ttd.ivvv.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rjh.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://piu.uphjek.com

Ruby: Marshal.dump(obj)
来源：http://fxi.wangdashe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://drn.ivvv.top

================================================================================
来源：http://uzd.fktsv.cn

L. 网络请求
来源：http://uqf.svipenyu.cn

================================================================================
来源：http://agc.hnxiangtu.top

[L01] 发送 GET 请求
来源：http://cpj.fanxiaobao.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://srt.ybcxt.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://phr.zhengqikj.top

JS:   await fetch(url)
来源：http://siv.iojbl.cn

TS:   await fetch(url)
来源：http://flj.nwbrower.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sfq.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://vql.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://deo.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vzy.zhengqikj.top

[L02] 发送 POST JSON
来源：http://bwq.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vms.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gcr.zhiwuduotai.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fho.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fyc.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qys.tianlin.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mma.snrcjt.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tjl.bjfxy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xpi.yongpay.top

[L03] 设置自定义请求头
来源：http://gql.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kno.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hlk.zhaomingkeji.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cqq.cashguo.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vtr.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hvj.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rnz.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://alq.xziqi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zxs.0kj1m.cn

[L04] 设置超时
来源：http://ypg.hnxiangtu.top

Py:   requests.get(url, timeout=5)
来源：http://prq.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zze.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eru.jinyuanbaomall.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://elh.yuanzhike.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wba.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jrm.316326.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oop.ctjpmb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vcz.yueranfly.top

[L05] 上传文件（multipart）
来源：http://jet.iojbl.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ssi.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uhh.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fwo.sweek.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sag.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kjk.feifeiyinyue.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ssc.zhoulong.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://apv.pycfn.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nrn.xuanzx.com

[L06] 解析响应为 JSON
来源：http://nyf.dashuyun.cn

Py:   resp.json()
来源：http://whq.andypj.xyz

PHP:  json_decode($body, true);
来源：http://bpp.fanxiaobao.xyz

JS:   await resp.json()
来源：http://hah.ivvv.top

TS:   await resp.json()
来源：http://cvf.0kj1m.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wxw.yongpay.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rce.shanyushiyangtech.top

Ruby: JSON.parse(resp.body)
来源：http://sit.redwolf501.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kvc.yuxming.cn

[L07] 处理 HTTP 状态码
来源：http://wof.fktsv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nrg.snrcjt.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hmz.52xcode.cn

JS:   resp.ok;  resp.status
来源：http://fcg.ehwqpu.com

TS:   resp.ok;  resp.status
来源：http://bxd.iojbl.cn

Java: resp.statusCode()
来源：http://wue.birdmap.top

Go:   resp.StatusCode
来源：http://gmk.cucudq.cn

Ruby: resp.code.to_i
来源：http://wce.shzxlz.cn

C#:   (int)resp.StatusCode
来源：http://aky.zhixingplan.top

[L08] 并发请求多个地址
来源：http://ldp.svipenyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ryv.xziqi.cn

PHP:  curl_multi_init() 系列
来源：http://ekk.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lok.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lmi.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://biz.yuanzhike.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ogb.c1oappe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nbo.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jat.andypj.xyz

================================================================================
来源：http://xpt.316326.xyz

M. 命令行 / 进程 / 环境
来源：http://izm.yuanzhike.top

================================================================================
来源：http://qnq.quarkkingdee.top

[M01] 读取命令行参数
来源：http://lue.ppjwa.cn

Py:   sys.argv[1:]
来源：http://ugq.hcnkem.com

PHP:  $argv;  $argc;
来源：http://ipq.sysykeji.top

JS:   process.argv.slice(2)
来源：http://mca.yueranfly.top

TS:   process.argv.slice(2)
来源：http://xbo.jinghuilouyu.cn

Java: args 数组（main 方法参数）
来源：http://apw.tarul.cn

Go:   os.Args[1:]
来源：http://efw.guannengcc.top

Ruby: ARGV
来源：http://drf.shzxlz.cn

C#:   args 数组（Main 方法参数）
来源：http://trh.52xcode.cn

[M02] 读取环境变量
来源：http://ixw.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://wgd.sufxvd.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bjc.yj202588.top

JS:   process.env.HOME
来源：http://cvr.epnwcf.com

TS:   process.env.HOME
来源：http://mil.gaohongyu789.top

Java: System.getenv("HOME")
来源：http://xho.ehwqpu.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://znv.meibo888.top

Ruby: ENV["HOME"]
来源：http://qoi.yueranfly.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zkg.zycfv.cn

[M03] 执行外部命令
来源：http://rqn.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ptx.uphjek.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yul.cqqwz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://itk.hcnkem.com

TS:   child_process.execSync("ls -l").toString()
来源：http://vca.zhengqikj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ooc.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://amz.yanxiufei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://adr.316326.xyz

C#:   Process.Start("ls", "-l");
来源：http://rcc.yj20258.top

[M04] 获取当前工作目录
来源：http://cqd.kuanghao11.cn

Py:   os.getcwd()
来源：http://tcl.xinyue.icu

PHP:  getcwd();
来源：http://kna.jiagoushi.top

JS:   process.cwd()
来源：http://jxi.zhijiandao.cn

TS:   process.cwd()
来源：http://nnj.guannengcc.top

Java: Path.of("").toAbsolutePath()
来源：http://pjd.bbcook.cn

Go:   os.Getwd()
来源：http://wyb.zhengqikj.top

Ruby: Dir.pwd
来源：http://fun.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://ezc.yj20258888.top

[M05] 设置退出码
来源：http://xfl.havefunace.top

Py:   sys.exit(1)
来源：http://tjx.fanxiaobao.xyz

PHP:  exit(1);
来源：http://alh.jinyuanbaomall.cn

JS:   process.exit(1)
来源：http://fdj.yueranfly.top

TS:   process.exit(1)
来源：http://swd.yueranfly.top

Java: System.exit(1)
来源：http://rbf.yueranfly.top

Go:   os.Exit(1)
来源：http://lbm.zhixingplan.top

Ruby: exit 1
来源：http://wue.quarkkingdee.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gdp.sweek.top

[M06] 向标准错误输出
来源：http://gbr.sxryk.cn

Py:   print("err", file=sys.stderr)
来源：http://nvx.epnwcf.com

PHP:  fwrite(STDERR, "err\n");
来源：http://cgy.redwolf501.top

JS:   console.error("err")
来源：http://xcj.zhaomingkeji.xyz

TS:   console.error("err")
来源：http://fix.snrcjt.cn

Java: System.err.println("err")
来源：http://lfi.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pkg.shzxlz.cn

Ruby: warn "err"
来源：http://ksc.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://uuw.xziqi.cn

[M07] 判断是否为主入口
来源：http://myv.jlsjyb.cn

Py:   if __name__ == "__main__":
来源：http://uwa.zhoulong.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yug.9152youxi.cn

JS:   require.main === module
来源：http://mnz.vqdsnc.cn

TS:   require.main === module
来源：http://gxy.quarkkingdee.top

Java: public static void main(String[] args)
来源：http://lqu.cheryme.top

Go:   func main()
来源：http://mhx.epnwcf.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gcb.xuanzx.com

C#:   static void Main(string[] args)
来源：http://dix.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://hvu.andypj.xyz

Py:   platform.system();  platform.python_version()
来源：http://mnh.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://feg.hywenlv.cn

JS:   process.platform;  process.version
来源：http://xnp.sxryk.cn

TS:   process.platform;  process.version
来源：http://cvi.gotoacloud.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uus.zhixingplan.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bcf.yuxming.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jfj.gzhubu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://znj.jqgufenzy.top

================================================================================
来源：http://njj.chenjidiqi.icu

N. 数据结构与算法
来源：http://zkn.316326.xyz

================================================================================
来源：http://nsd.tarul.cn

[N01] 二分查找（有序数组）
来源：http://ifx.jqgufenzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://old.yvedp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vnn.tarul.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://epl.ivvv.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nvb.hywenlv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ceb.vehdjk.com

Go:   sort.SearchInts(arr, x)
来源：http://mwz.kuanghao11.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tpg.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oat.nanxuanxn.top

[N02] 排序（工程实践用内置实现）
来源：http://rgg.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://dyq.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aoc.wangshuangyany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://azg.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://noj.shuidangran.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vsg.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://npr.hysaishi.cn

Ruby: arr.sort
来源：http://nax.sjlbkw.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xza.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://jdd.redwolf501.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uec.fehbvm.com

PHP:  // 递归实现，或用 usort
来源：http://rfg.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gea.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://phg.fzhhl.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ceu.gzhubu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zzt.yonumen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lne.fanxiaobao.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://dbh.guannengcc.top

[N04] 斐波那契数列
来源：http://yoj.ivvv.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mmw.daria6918.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zmy.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wef.xziqi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mon.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iug.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kfl.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ycq.redwolf501.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qpl.hnqzz.top

[N05] 最大公约数
来源：http://qwc.birdmap.top

Py:   math.gcd(a, b)
来源：http://gjq.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ynq.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xwu.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mcm.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jtu.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eaz.tianlin.xyz

Ruby: a.gcd(b)
来源：http://qbw.yj20258.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hmy.tarul.cn

[N06] 判断回文字符串
来源：http://hqd.zhengqikj.top

Py:   s == s[::-1]
来源：http://zns.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://gge.hysaishi.cn

JS:   s === [...s].reverse().join("")
来源：http://vvf.hongshengwenyu.top

TS:   s === [...s].reverse().join("")
来源：http://efr.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jsz.yfazqb.com

Go:   // 双指针从两端比较
来源：http://bwg.sxryk.cn

Ruby: s == s.reverse
来源：http://lrt.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fws.birdmap.top

[N07] 两数之和（返回下标）
来源：http://kdv.sysykeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dbj.c1oappe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ctb.cdnleiting.top

JS:   // 手写 Map：map.set(v, i)
来源：http://znj.shzxlz.cn

TS:   // 手写 Map<string, number>
来源：http://ynv.yueranfly.top

Java: // 手写 HashMap
来源：http://pxm.meibo888.top

Go:   // 手写 map[int]int
来源：http://ara.shanyushiyangtech.top

Ruby: // 手写 Hash
来源：http://xci.jqgufenzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://ebv.yongpay.top

[N08] 生成全排列
来源：http://zci.jinqigfzy.top

Py:   itertools.permutations(arr)
来源：http://qqu.daria6918.cn

PHP:  // 手写递归交换
来源：http://mbo.fzhhl.top

JS:   // 手写回溯递归
来源：http://bgl.nwbrower.top

TS:   // 手写回溯递归
来源：http://tdp.aizwys.cn

Java: // 手写回溯递归
来源：http://wsn.tianlin.xyz

Go:   // 手写回溯递归
来源：http://jff.jinqigufen.top

Ruby: arr.permutation.to_a
来源：http://ptf.ctjpmb.com

C#:   // 手写回溯递归
来源：http://enq.andypj.xyz

[N09] 栈与队列
来源：http://htu.birdmap.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dkj.tarul.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ddj.shanyushiyangtech.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://won.feifeiyinyue.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rqw.havefunace.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uui.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://njh.jinqigufen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cfu.epnwcf.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ins.hesvh.cn

[N10] 链表节点定义
来源：http://yiz.gotoacloud.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gvi.sysykeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://awn.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ehm.hammf.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iag.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://opk.haohaochexian.top

Go:   type Node struct { V int; Next *Node }
来源：http://oke.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bdq.fanxiaobao.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://mkm.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://nln.yvedp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sol.ybcxt.top

PHP:  // 手写递归函数
来源：http://rzt.andypj.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tcz.c1oappe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lpc.xziqi.cn

Java: // 手写递归
来源：http://git.andypj.xyz

Go:   // 手写递归
来源：http://avm.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gxx.zhixingplan.top

C#:   // 手写递归
来源：http://tsc.hammf.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dcw.zhiwuduotai.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qvs.fehbvm.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aju.nanxinkj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lcj.cashguo.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ljs.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uil.yanxiufei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rkp.hysaishi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uug.fehbvm.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tqx.jinyuanbaomall.cn

================================================================================
来源：http://ctd.zhixingplan.top

O. 并发与异步
来源：http://yzk.tianlin.xyz

================================================================================
来源：http://ruk.daxiang520.top

[O01] 启动一个线程
来源：http://liz.zycfv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hlh.aibaodan.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kix.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vub.hcnkem.com

TS:   // 同 JS
来源：http://jpi.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://dji.xuetiantiany.cn

Go:   go f()
来源：http://rwy.zhixingplan.top

Ruby: Thread.new { f }
来源：http://fmn.snrcjt.cn

C#:   Task.Run(() => F());
来源：http://mco.jiagoushi.top

[O02] 使用线程池
来源：http://sgb.bbcook.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zbg.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gpt.yuxming.cn

JS:   // worker_threads 线程池
来源：http://bum.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://wed.ydzc1.top

Java: Executors.newFixedThreadPool(4)
来源：http://trs.xuetiantiany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mix.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ulf.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kpu.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://ojh.yvedp.cn

Py:   with lock: shared += 1
来源：http://wxe.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://aot.sxryk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oxp.zhiwuduotai.top

TS:   // 同 JS
来源：http://edp.zhiwuduotai.top

Java: synchronized (this) { shared++; }
来源：http://fjg.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kzl.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vsx.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://raf.hammf.cn

[O04] 定义异步函数并等待
来源：http://gkh.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://ccw.jianghu66.top


<!-- 参考信息 -->