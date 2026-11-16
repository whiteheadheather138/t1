代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://qcb.svipenyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://xvi.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://jkw.guowangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dai.zhongyouzk.top

Go:   encoding/gob
来源：http://lvw.ivvv.top

Ruby: Marshal.dump(obj)
来源：http://qfx.andypj.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yja.quarkkingdee.top

================================================================================
来源：http://yij.zhaomingkeji.xyz

L. 网络请求
来源：http://xhi.sxryk.cn

================================================================================
来源：http://kms.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://frj.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ask.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ehf.guannengcc.top

JS:   await fetch(url)
来源：http://mpd.hysaishi.cn

TS:   await fetch(url)
来源：http://any.zhixingplan.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xtg.yuanzhike.top

Go:   resp, err := http.Get(url)
来源：http://xzc.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uuo.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mhm.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://dxt.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://fit.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://flo.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fab.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://agw.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rff.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lca.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kub.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nhx.hfpthk.cn

[L03] 设置自定义请求头
来源：http://rgb.316326.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zzx.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jhf.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uqx.ywan-chungtsiang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mku.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rms.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gxj.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ugw.tianlin.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zid.sysykeji.top

[L04] 设置超时
来源：http://wuz.52xcode.cn

Py:   requests.get(url, timeout=5)
来源：http://sic.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fud.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nud.9152youxi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pby.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tgq.svipenyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aav.redwolf501.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ezy.fehbvm.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bwo.xinyue.icu

[L05] 上传文件（multipart）
来源：http://ndd.zhixingplan.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uuq.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lvq.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mly.birdmap.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yeu.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ffp.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sch.aizwys.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pnk.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xli.tarul.cn

[L06] 解析响应为 JSON
来源：http://xtx.bbcook.cn

Py:   resp.json()
来源：http://bxs.meibo888.top

PHP:  json_decode($body, true);
来源：http://xnd.yj20258.top

JS:   await resp.json()
来源：http://yox.jinqigfzy.top

TS:   await resp.json()
来源：http://urd.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kmt.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://czf.quarkkingdee.top

Ruby: JSON.parse(resp.body)
来源：http://jga.havefunace.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ylb.pengpengdd.cyou

[L07] 处理 HTTP 状态码
来源：http://urx.zhongyouzk.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zvf.fzhhl.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://avu.sxryk.cn

JS:   resp.ok;  resp.status
来源：http://iku.smart0.xyz

TS:   resp.ok;  resp.status
来源：http://sln.xingfuxueyuan.xyz

Java: resp.statusCode()
来源：http://oll.dianchejie.cn

Go:   resp.StatusCode
来源：http://xkc.meibo888.top

Ruby: resp.code.to_i
来源：http://rsz.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://alt.cashguo.top

[L08] 并发请求多个地址
来源：http://zzz.jiagoushi.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yhe.jlsjyb.cn

PHP:  curl_multi_init() 系列
来源：http://byl.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://suw.ydjk.org.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vdn.sjlbkw.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sgr.c1oappe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cdw.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sjr.ydzc1.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kjx.xziqi.cn

================================================================================
来源：http://fzo.xuetiantiany.cn

M. 命令行 / 进程 / 环境
来源：http://kug.ppjwa.cn

================================================================================
来源：http://jdx.zdqjudy.top

[M01] 读取命令行参数
来源：http://ynq.zhijiandao.cn

Py:   sys.argv[1:]
来源：http://olw.sjlbkw.cn

PHP:  $argv;  $argc;
来源：http://obo.ydjk.org.cn

JS:   process.argv.slice(2)
来源：http://fsi.xinyue.icu

TS:   process.argv.slice(2)
来源：http://eip.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://apj.hammf.cn

Go:   os.Args[1:]
来源：http://xnn.yj202588.top

Ruby: ARGV
来源：http://rlg.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://oll.vehdjk.com

[M02] 读取环境变量
来源：http://api.jlsjyb.cn

Py:   os.environ.get("HOME")
来源：http://tre.chenzaomai.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://non.nwbrower.top

JS:   process.env.HOME
来源：http://kgi.yangfankeji.com

TS:   process.env.HOME
来源：http://oko.9152youxi.cn

Java: System.getenv("HOME")
来源：http://wpn.aibaodan.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ddt.zhijiandao.cn

Ruby: ENV["HOME"]
来源：http://bxe.aibaodan.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vja.quarkkingdee.top

[M03] 执行外部命令
来源：http://dif.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vtu.0kj1m.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gva.ydjk.org.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xvw.hywenlv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sul.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ime.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rjh.epnwcf.com

Ruby: system("ls -l");  `ls -l`
来源：http://atv.hnqzz.top

C#:   Process.Start("ls", "-l");
来源：http://cao.yonumen.top

[M04] 获取当前工作目录
来源：http://noa.shuidangran.top

Py:   os.getcwd()
来源：http://qwd.vehdjk.com

PHP:  getcwd();
来源：http://drq.zhijiandao.cn

JS:   process.cwd()
来源：http://tpt.uphjek.com

TS:   process.cwd()
来源：http://gaa.iojbl.cn

Java: Path.of("").toAbsolutePath()
来源：http://imm.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://ftl.gzhubu.top

Ruby: Dir.pwd
来源：http://gfs.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://rgi.guannengcc.top

[M05] 设置退出码
来源：http://eae.zdbjq.cn

Py:   sys.exit(1)
来源：http://qyo.zhengqikj.top

PHP:  exit(1);
来源：http://sce.xziqi.cn

JS:   process.exit(1)
来源：http://zoi.yj20258.top

TS:   process.exit(1)
来源：http://vfk.ybcxt.top

Java: System.exit(1)
来源：http://nzw.yonumen.top

Go:   os.Exit(1)
来源：http://kky.haohaochexian.top

Ruby: exit 1
来源：http://umb.sweek.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sji.cucudq.cn

[M06] 向标准错误输出
来源：http://suk.hnqzz.top

Py:   print("err", file=sys.stderr)
来源：http://ymf.sxryk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://luu.daxiang520.top

JS:   console.error("err")
来源：http://aau.316326.xyz

TS:   console.error("err")
来源：http://efs.pycfn.com

Java: System.err.println("err")
来源：http://pbw.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ulq.mhx1999.top

Ruby: warn "err"
来源：http://ukh.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://izv.sweek.top

[M07] 判断是否为主入口
来源：http://vrq.epnwcf.com

Py:   if __name__ == "__main__":
来源：http://ihv.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uiv.jinqigfzy.top

JS:   require.main === module
来源：http://nlt.sweek.top

TS:   require.main === module
来源：http://dyj.sweek.top

Java: public static void main(String[] args)
来源：http://chu.jinghuilouyu.cn

Go:   func main()
来源：http://ire.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mwb.tian-w.cn

C#:   static void Main(string[] args)
来源：http://bad.52xcode.cn

[M08] 获取系统与运行时信息
来源：http://pud.fanxiaobao.xyz

Py:   platform.system();  platform.python_version()
来源：http://ibl.hnqzz.top

PHP:  PHP_OS;  phpversion();
来源：http://veb.vehdjk.com

JS:   process.platform;  process.version
来源：http://khf.cashguo.top

TS:   process.platform;  process.version
来源：http://rlk.cqqwz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kec.hysaishi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vzx.ivvv.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hcb.xingfuxueyuan.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://cgg.ywan-chungtsiang.top

================================================================================
来源：http://qsm.fengsongda.top

N. 数据结构与算法
来源：http://qri.hongshengwenyu.top

================================================================================
来源：http://bzu.sxryk.cn

[N01] 二分查找（有序数组）
来源：http://ksz.ybcxt.top

Py:   bisect.bisect_left(arr, x)
来源：http://hll.9152youxi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vuh.pengpengdd.cyou

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lub.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pcm.jqgufenzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://tgb.zhongyouzk.top

Go:   sort.SearchInts(arr, x)
来源：http://wzh.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lmi.tarul.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mhf.ydzc1.top

[N02] 排序（工程实践用内置实现）
来源：http://leg.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://prv.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wbs.zycfv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cod.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://baq.redwolf501.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nun.redwolf501.top

Go:   slices.Sort(arr)
来源：http://wxu.fehbvm.com

Ruby: arr.sort
来源：http://glf.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fim.bbcook.cn

[N03] 快速排序（分治示例）
来源：http://rhr.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://buc.yuanzhike.top

PHP:  // 递归实现，或用 usort
来源：http://ofn.guowangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lpu.birdmap.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hxt.nanxinkj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rwp.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gek.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rit.wangdashe.top

C#:   // 手写递归，或 Array.Sort
来源：http://jsf.gogol.net.cn

[N04] 斐波那契数列
来源：http://mpm.gogol.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yhc.gotoacloud.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lig.hywenlv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://laz.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nuo.shuidangran.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xaj.hammf.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cgt.sjlbkw.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tia.hnxiangtu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oeh.wangshuangyany.cn

[N05] 最大公约数
来源：http://ftl.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://zsg.jiagoushi.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qtb.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ths.ydjk.org.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vvc.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yom.cqqwz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rmm.quarkkingdee.top

Ruby: a.gcd(b)
来源：http://vfo.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hdd.cashguo.top

[N06] 判断回文字符串
来源：http://dzt.hywenlv.cn

Py:   s == s[::-1]
来源：http://lhn.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://chj.zhongyouzk.top

JS:   s === [...s].reverse().join("")
来源：http://eju.hnqzz.top

TS:   s === [...s].reverse().join("")
来源：http://ksz.ywan-chungtsiang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://grl.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://ook.ppjwa.cn

Ruby: s == s.reverse
来源：http://cnc.havefunace.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tdp.feifeiyinyue.top

[N07] 两数之和（返回下标）
来源：http://qtt.yuxming.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hux.chenzaomai.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://irg.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://cmu.mhx1999.top

TS:   // 手写 Map<string, number>
来源：http://tmj.jyoumei.cn

Java: // 手写 HashMap
来源：http://vki.shzxlz.cn

Go:   // 手写 map[int]int
来源：http://bmm.tarul.cn

Ruby: // 手写 Hash
来源：http://pzt.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://mat.jianghu66.top

[N08] 生成全排列
来源：http://vly.316326.xyz

Py:   itertools.permutations(arr)
来源：http://pwk.yj202588.top

PHP:  // 手写递归交换
来源：http://yhr.iojbl.cn

JS:   // 手写回溯递归
来源：http://jve.xziqi.cn

TS:   // 手写回溯递归
来源：http://ldf.birdmap.top

Java: // 手写回溯递归
来源：http://uup.sweek.top

Go:   // 手写回溯递归
来源：http://acz.gogol.net.cn

Ruby: arr.permutation.to_a
来源：http://gru.xuanzx.com

C#:   // 手写回溯递归
来源：http://jqz.vqdsnc.cn

[N09] 栈与队列
来源：http://qgt.gzhubu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bzw.ppjwa.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cva.yuanzhike.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hvd.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cjf.nanxinkj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gtx.aibaodan.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://esk.ivvv.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://txy.mhx1999.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uvm.yfazqb.com

[N10] 链表节点定义
来源：http://ton.dianchejie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ydp.jiagoushi.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kmn.guowangkeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qyl.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dlb.tarul.cn

Java: class Node { int v; Node next; }
来源：http://psg.yanxiufei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mya.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://ism.nanxuanxn.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vvn.chenlongwang.top

[N11] 二叉树中序遍历
来源：http://qca.zdqjudy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rdc.daxiang520.top

PHP:  // 手写递归函数
来源：http://tfu.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xwx.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pto.zycfv.cn

Java: // 手写递归
来源：http://due.xingfuxueyuan.xyz

Go:   // 手写递归
来源：http://hoj.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lwb.zhijiandao.cn

C#:   // 手写递归
来源：http://pns.zhiwuduotai.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tdu.ydjk.org.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ajo.uphjek.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jeo.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dof.9152youxi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ana.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pxe.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gdi.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ifo.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ybt.ydjk.org.cn

================================================================================
来源：http://qiw.yvedp.cn

O. 并发与异步
来源：http://qiv.ydzc1.top

================================================================================
来源：http://prj.yuxming.cn

[O01] 启动一个线程
来源：http://wnb.jqgufenzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://klo.uphjek.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xnd.jinghuilouyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bih.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://oyj.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://jeq.smart0.xyz

Go:   go f()
来源：http://lly.gaohongyu789.top

Ruby: Thread.new { f }
来源：http://grj.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://ado.nwbrower.top

[O02] 使用线程池
来源：http://rba.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://shh.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ehd.fzhhl.top

JS:   // worker_threads 线程池
来源：http://ncx.iojbl.cn

TS:   // worker_threads 线程池
来源：http://crw.xylfe.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pqr.jinqigufen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zuy.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dtw.haohaochexian.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://emx.daria6918.cn

[O03] 加锁保护共享数据
来源：http://jvc.cdnleiting.top

Py:   with lock: shared += 1
来源：http://dbh.fanxiaobao.xyz

PHP:  // 用 flock() 做文件锁
来源：http://twa.havefunace.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sgk.zhiwuduotai.top

TS:   // 同 JS
来源：http://vcz.jqgfzy.top

Java: synchronized (this) { shared++; }
来源：http://bef.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xqy.zhijiandao.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uej.uphjek.com

C#:   lock (gate) { shared++; }
来源：http://olf.iojbl.cn

[O04] 定义异步函数并等待
来源：http://jtf.xuanzx.com

Py:   async def f():⏎    await g()
来源：http://yuo.sufxvd.cn


<!-- 参考信息 -->