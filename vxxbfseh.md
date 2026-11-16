代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://ejo.jlsjyb.cn

JS:   v8.serialize(obj)        // Node
来源：http://wxe.yj20258.top

TS:   v8.serialize(obj)        // Node
来源：http://wbh.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kvw.ppjwa.cn

Go:   encoding/gob
来源：http://wvj.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://trd.fzhhl.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://huo.yuanzhike.top

================================================================================
来源：http://qet.sxryk.cn

L. 网络请求
来源：http://cma.yfazqb.com

================================================================================
来源：http://frt.xuanzx.com

[L01] 发送 GET 请求
来源：http://bes.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cln.yj202588.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uqn.yangfankeji.com

JS:   await fetch(url)
来源：http://ouv.zdqjudy.top

TS:   await fetch(url)
来源：http://ois.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://reo.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://tvo.jyoumei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zho.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xkv.nanxinkj.top

[L02] 发送 POST JSON
来源：http://lzd.kuanghao11.cn

Py:   requests.post(url, json={"a": 1})
来源：http://noc.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mbh.wangshuangyany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rqf.haohaochexian.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pwn.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fhj.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sri.haohaochexian.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mqe.uphjek.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ivi.cdnleiting.top

[L03] 设置自定义请求头
来源：http://thq.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kyi.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://txr.9152youxi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mey.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xdz.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tfh.yj20258.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dsr.sufxvd.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mxa.cqqwz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zwc.316326.xyz

[L04] 设置超时
来源：http://ymr.quarkkingdee.top

Py:   requests.get(url, timeout=5)
来源：http://asb.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tcc.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baw.xylfe.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ume.zycfv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xpj.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xpd.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kpl.ydzc1.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ewk.yfazqb.com

[L05] 上传文件（multipart）
来源：http://jmq.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qow.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fcp.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hlk.ybcxt.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kuk.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oru.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ahg.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fhj.hammf.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xtw.yonumen.top

[L06] 解析响应为 JSON
来源：http://iwg.hammf.cn

Py:   resp.json()
来源：http://sib.yvedp.cn

PHP:  json_decode($body, true);
来源：http://wzb.uphjek.com

JS:   await resp.json()
来源：http://ylv.smart0.xyz

TS:   await resp.json()
来源：http://afn.hesvh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uuo.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xek.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://qla.jlsjyb.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://scx.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://olg.iojbl.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aab.meibo888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rch.xingfuxueyuan.xyz

JS:   resp.ok;  resp.status
来源：http://hzi.zycfv.cn

TS:   resp.ok;  resp.status
来源：http://soe.fehbvm.com

Java: resp.statusCode()
来源：http://bru.shanyushiyangkeji.top

Go:   resp.StatusCode
来源：http://uww.sysykeji.top

Ruby: resp.code.to_i
来源：http://sor.xuanzx.com

C#:   (int)resp.StatusCode
来源：http://xey.chenlongwang.top

[L08] 并发请求多个地址
来源：http://jfp.zhoulong.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ccm.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://qjy.sjlbkw.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fwd.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jiu.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zuz.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rap.daxiang520.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iip.nanxuanxn.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gxt.epnwcf.com

================================================================================
来源：http://qot.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://msc.gotoacloud.top

================================================================================
来源：http://itp.wangdashe.top

[M01] 读取命令行参数
来源：http://rss.sweek.top

Py:   sys.argv[1:]
来源：http://uuy.yangfankeji.com

PHP:  $argv;  $argc;
来源：http://cme.iojbl.cn

JS:   process.argv.slice(2)
来源：http://kqh.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://eya.uphjek.com

Java: args 数组（main 方法参数）
来源：http://hdw.hfpthk.cn

Go:   os.Args[1:]
来源：http://fsm.aibaodan.cn

Ruby: ARGV
来源：http://pnt.hnxiangtu.top

C#:   args 数组（Main 方法参数）
来源：http://uum.guowangkeji.top

[M02] 读取环境变量
来源：http://tps.jqgfzy.top

Py:   os.environ.get("HOME")
来源：http://irb.uphjek.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ttk.ydzc1.top

JS:   process.env.HOME
来源：http://kwo.chenzaomai.com

TS:   process.env.HOME
来源：http://thf.yonumen.top

Java: System.getenv("HOME")
来源：http://xdm.hnxiangtu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rzi.ivvv.top

Ruby: ENV["HOME"]
来源：http://dsa.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ybn.316326.xyz

[M03] 执行外部命令
来源：http://xfd.shanyushiyangtech.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://klv.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aey.pycfn.com

JS:   child_process.execSync("ls -l").toString()
来源：http://szy.aibaodan.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tvh.fengsongda.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jez.andypj.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://tem.fanxiaobao.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://mho.jinyuanbaomall.cn

C#:   Process.Start("ls", "-l");
来源：http://ugw.feifeiyinyue.top

[M04] 获取当前工作目录
来源：http://itl.yongpay.top

Py:   os.getcwd()
来源：http://nzs.meibo888.top

PHP:  getcwd();
来源：http://frj.ybcxt.top

JS:   process.cwd()
来源：http://mqn.iojbl.cn

TS:   process.cwd()
来源：http://thi.gogol.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://csc.zhaomingkeji.xyz

Go:   os.Getwd()
来源：http://nqo.yuxming.cn

Ruby: Dir.pwd
来源：http://tlg.xylfe.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xbf.gzhubu.top

[M05] 设置退出码
来源：http://smu.yongpay.top

Py:   sys.exit(1)
来源：http://avd.tarul.cn

PHP:  exit(1);
来源：http://qoc.tian-w.cn

JS:   process.exit(1)
来源：http://gez.andypj.xyz

TS:   process.exit(1)
来源：http://rcb.hnxiangtu.top

Java: System.exit(1)
来源：http://ygj.zycfv.cn

Go:   os.Exit(1)
来源：http://nrz.gaohongyu789.top

Ruby: exit 1
来源：http://ibz.hywenlv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tbl.9152youxi.cn

[M06] 向标准错误输出
来源：http://rvu.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://xjh.yfazqb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://cmu.shzxlz.cn

JS:   console.error("err")
来源：http://rsp.xuetiantiany.cn

TS:   console.error("err")
来源：http://tti.zdbjq.cn

Java: System.err.println("err")
来源：http://jqr.316326.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iob.chenjidiqi.icu

Ruby: warn "err"
来源：http://yyx.dianchejie.cn

C#:   Console.Error.WriteLine("err")
来源：http://mca.ivvv.top

[M07] 判断是否为主入口
来源：http://eie.yonumen.top

Py:   if __name__ == "__main__":
来源：http://fsf.chenjidiqi.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dgm.yuxming.cn

JS:   require.main === module
来源：http://jtn.daxiang520.top

TS:   require.main === module
来源：http://ddh.mhx1999.top

Java: public static void main(String[] args)
来源：http://vwg.pycfn.com

Go:   func main()
来源：http://rpy.gogol.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://krv.epnwcf.com

C#:   static void Main(string[] args)
来源：http://sjy.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://cdw.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://npw.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://qxe.sweek.top

JS:   process.platform;  process.version
来源：http://hnf.hysaishi.cn

TS:   process.platform;  process.version
来源：http://zvq.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dpy.chenjidiqi.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://isw.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jtp.jinghuilouyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gru.zhiwuduotai.top

================================================================================
来源：http://osn.316326.xyz

N. 数据结构与算法
来源：http://hhq.gogol.net.cn

================================================================================
来源：http://hyo.sysykeji.top

[N01] 二分查找（有序数组）
来源：http://aen.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://wbl.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pci.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ydi.jyoumei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://grv.zhoulong.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://awe.316326.xyz

Go:   sort.SearchInts(arr, x)
来源：http://uhd.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gir.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://plb.hfpthk.cn

[N02] 排序（工程实践用内置实现）
来源：http://pik.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://ckd.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dob.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vou.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jha.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://edg.bbcook.cn

Go:   slices.Sort(arr)
来源：http://zzj.ppjwa.cn

Ruby: arr.sort
来源：http://weu.tianlin.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://iiv.yuanzhike.top

[N03] 快速排序（分治示例）
来源：http://zsc.gzhubu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lby.9152youxi.cn

PHP:  // 递归实现，或用 usort
来源：http://sam.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uqs.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ofu.zhoulong.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yjk.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ali.xinyue.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ufs.yfazqb.com

C#:   // 手写递归，或 Array.Sort
来源：http://fnh.zhengqikj.top

[N04] 斐波那契数列
来源：http://ytn.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bwr.jyoumei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://plc.zhaomingkeji.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rtw.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hse.fanxiaobao.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kfs.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://prf.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fgk.cdnleiting.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fun.cucudq.cn

[N05] 最大公约数
来源：http://xtz.cheryme.top

Py:   math.gcd(a, b)
来源：http://tit.feifeiyinyue.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nyt.316326.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rby.uphjek.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ebm.epnwcf.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jud.nanxinkj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zjq.bjfxy.top

Ruby: a.gcd(b)
来源：http://rny.nanxinkj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ahj.fanxiaobao.xyz

[N06] 判断回文字符串
来源：http://pph.jlsjyb.cn

Py:   s == s[::-1]
来源：http://kfu.ywan-chungtsiang.top

PHP:  $s === strrev($s);
来源：http://iac.iojbl.cn

JS:   s === [...s].reverse().join("")
来源：http://khs.pycfn.com

TS:   s === [...s].reverse().join("")
来源：http://klt.9152youxi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jbt.havefunace.top

Go:   // 双指针从两端比较
来源：http://ilw.epnwcf.com

Ruby: s == s.reverse
来源：http://wuc.shuidangran.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://eia.yj20258.top

[N07] 两数之和（返回下标）
来源：http://lfu.dianchejie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fbr.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vox.zhongyouzk.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dbt.hnxiangtu.top

TS:   // 手写 Map<string, number>
来源：http://hsj.yanxiufei.cn

Java: // 手写 HashMap
来源：http://lgw.yuanzhike.top

Go:   // 手写 map[int]int
来源：http://yuv.cqqwz.cn

Ruby: // 手写 Hash
来源：http://keg.hesvh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bwb.yfazqb.com

[N08] 生成全排列
来源：http://gix.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://zjm.meibo888.top

PHP:  // 手写递归交换
来源：http://ags.shanyushiyangkeji.top

JS:   // 手写回溯递归
来源：http://dzf.jinqigfzy.top

TS:   // 手写回溯递归
来源：http://uyh.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://rgt.hnxiangtu.top

Go:   // 手写回溯递归
来源：http://qvb.hfpthk.cn

Ruby: arr.permutation.to_a
来源：http://abm.shzxlz.cn

C#:   // 手写回溯递归
来源：http://smj.andypj.xyz

[N09] 栈与队列
来源：http://iah.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://msj.redwolf501.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cmo.cashguo.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nfi.havefunace.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lyi.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://shl.jqgfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ple.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://soh.ppjwa.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pcj.chenzaomai.com

[N10] 链表节点定义
来源：http://dkq.sjlbkw.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aeo.zhoulong.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://bah.pengpengdd.cyou

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://owe.shanyushiyangtech.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ris.hammf.cn

Java: class Node { int v; Node next; }
来源：http://dia.gaohongyu789.top

Go:   type Node struct { V int; Next *Node }
来源：http://pvm.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://wnj.ydzc1.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lat.gzhubu.top

[N11] 二叉树中序遍历
来源：http://ylo.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kcj.hesvh.cn

PHP:  // 手写递归函数
来源：http://yxx.yj202588.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fod.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vsu.9152youxi.cn

Java: // 手写递归
来源：http://plc.zycfv.cn

Go:   // 手写递归
来源：http://rdo.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ypo.hywenlv.cn

C#:   // 手写递归
来源：http://jhn.fktsv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ovw.hesvh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fln.hcnkem.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://meu.gotoacloud.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uvw.yj202588.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mtw.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fxc.hesvh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qeg.chenjidiqi.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mef.redwolf501.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eon.tarul.cn

================================================================================
来源：http://iyj.yj202588.top

O. 并发与异步
来源：http://uhn.fzhhl.top

================================================================================
来源：http://dal.shangyingyoupin.top

[O01] 启动一个线程
来源：http://zrs.andypj.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://raf.vqdsnc.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rla.jinqigfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://msm.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://ubb.dianchejie.cn

Java: new Thread(() -> f()).start()
来源：http://zyw.zhijiandao.cn

Go:   go f()
来源：http://jol.tanke756.top

Ruby: Thread.new { f }
来源：http://aul.redwolf501.top

C#:   Task.Run(() => F());
来源：http://iiy.yvedp.cn

[O02] 使用线程池
来源：http://ksf.gotoacloud.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qtv.pengpengdd.cyou

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://acc.ehwqpu.com

JS:   // worker_threads 线程池
来源：http://nno.zhongyouzk.top

TS:   // worker_threads 线程池
来源：http://btu.havefunace.top

Java: Executors.newFixedThreadPool(4)
来源：http://dmz.hongshengwenyu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uus.ybcxt.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cst.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ujp.havefunace.top

[O03] 加锁保护共享数据
来源：http://ykd.havefunace.top

Py:   with lock: shared += 1
来源：http://kgs.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://wof.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cya.jlsjyb.cn

TS:   // 同 JS
来源：http://hwy.haohaochexian.top

Java: synchronized (this) { shared++; }
来源：http://suk.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dtp.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://alo.jinyuanbaomall.cn

C#:   lock (gate) { shared++; }
来源：http://psk.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://nlu.zdqjudy.top

Py:   async def f():⏎    await g()
来源：http://zje.jlsjyb.cn


<!-- 参考信息 -->