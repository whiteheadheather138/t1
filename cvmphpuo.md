代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://pqy.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://peb.hongshengwenyu.top

TS:   v8.serialize(obj)        // Node
来源：http://yxh.havefunace.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qih.fktsv.cn

Go:   encoding/gob
来源：http://adb.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://jso.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ayi.chenjidiqi.icu

================================================================================
来源：http://ixb.nanxinkj.top

L. 网络请求
来源：http://pbu.havefunace.top

================================================================================
来源：http://frq.dashuyun.cn

[L01] 发送 GET 请求
来源：http://ieq.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jji.yuanzhike.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bgd.jqgfzy.top

JS:   await fetch(url)
来源：http://xli.hnqzz.top

TS:   await fetch(url)
来源：http://gsh.gzhubu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jig.hongshengwenyu.top

Go:   resp, err := http.Get(url)
来源：http://yrf.jqgfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://off.xinyue.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://brr.0kj1m.cn

[L02] 发送 POST JSON
来源：http://lwv.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://bcn.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://low.jinqigfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gfl.hesvh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hsy.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kbj.zycfv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xbu.xuanzx.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sil.fehbvm.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://swv.wangshuangyany.cn

[L03] 设置自定义请求头
来源：http://cjr.yanxiufei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rxd.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yjk.chenlongwang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uli.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vcn.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wzz.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fxf.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://goc.uphjek.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mqb.gaohongyu789.top

[L04] 设置超时
来源：http://rie.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://ehi.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hdt.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uay.cashguo.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fnj.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rfe.svipenyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wgz.redwolf501.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pxv.cheryme.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zkb.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://bwg.zhengqikj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kac.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ulj.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tph.mhx1999.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wqw.ivvv.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://okl.zycfv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ldq.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lvu.xingfuxueyuan.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jnx.sysykeji.top

[L06] 解析响应为 JSON
来源：http://hbn.xinyue.icu

Py:   resp.json()
来源：http://geh.c1oappe.top

PHP:  json_decode($body, true);
来源：http://nsg.zhengqikj.top

JS:   await resp.json()
来源：http://ijs.quarkkingdee.top

TS:   await resp.json()
来源：http://jeh.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bnx.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vay.yvedp.cn

Ruby: JSON.parse(resp.body)
来源：http://erw.sjlbkw.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qdw.ctjpmb.com

[L07] 处理 HTTP 状态码
来源：http://hcr.ctjpmb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dbp.ehwqpu.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xmr.sxryk.cn

JS:   resp.ok;  resp.status
来源：http://bmz.ivvv.top

TS:   resp.ok;  resp.status
来源：http://vft.iojbl.cn

Java: resp.statusCode()
来源：http://nqk.tarul.cn

Go:   resp.StatusCode
来源：http://ccr.jinqigfzy.top

Ruby: resp.code.to_i
来源：http://xin.yfazqb.com

C#:   (int)resp.StatusCode
来源：http://qtv.aibaodan.cn

[L08] 并发请求多个地址
来源：http://ild.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://apj.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://obk.sweek.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://clx.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wbl.mhx1999.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://epu.ybcxt.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oep.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ioa.meibo888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cye.chenzaomai.com

================================================================================
来源：http://tna.zhoulong.xyz

M. 命令行 / 进程 / 环境
来源：http://zfb.hcnkem.com

================================================================================
来源：http://ifn.cheryme.top

[M01] 读取命令行参数
来源：http://mqx.aizwys.cn

Py:   sys.argv[1:]
来源：http://epq.havefunace.top

PHP:  $argv;  $argc;
来源：http://whu.xuetiantiany.cn

JS:   process.argv.slice(2)
来源：http://zgz.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://ubn.ppjwa.cn

Java: args 数组（main 方法参数）
来源：http://lpq.birdmap.top

Go:   os.Args[1:]
来源：http://hax.jinqigufen.top

Ruby: ARGV
来源：http://ztk.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://rwz.daria6918.cn

[M02] 读取环境变量
来源：http://tgc.yj20258888.top

Py:   os.environ.get("HOME")
来源：http://ncg.shanyushiyangtech.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://evr.ivvv.top

JS:   process.env.HOME
来源：http://vkm.hywenlv.cn

TS:   process.env.HOME
来源：http://tfw.havefunace.top

Java: System.getenv("HOME")
来源：http://mjg.cdnleiting.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://glu.fktsv.cn

Ruby: ENV["HOME"]
来源：http://bif.fzhhl.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ikw.feifeiyinyue.top

[M03] 执行外部命令
来源：http://czk.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ros.0kj1m.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lbi.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ijo.cdnleiting.top

TS:   child_process.execSync("ls -l").toString()
来源：http://irr.jinghuilouyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://otq.hcnkem.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ude.cashguo.top

Ruby: system("ls -l");  `ls -l`
来源：http://qiq.jinqigfzy.top

C#:   Process.Start("ls", "-l");
来源：http://ddi.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://bud.iojbl.cn

Py:   os.getcwd()
来源：http://isf.yj20258888.top

PHP:  getcwd();
来源：http://vwb.yfazqb.com

JS:   process.cwd()
来源：http://kwk.ydjk.org.cn

TS:   process.cwd()
来源：http://tix.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://bpp.chenjidiqi.icu

Go:   os.Getwd()
来源：http://nww.cqqwz.cn

Ruby: Dir.pwd
来源：http://jwm.bjfxy.top

C#:   Directory.GetCurrentDirectory()
来源：http://bon.ydzc1.top

[M05] 设置退出码
来源：http://xmg.xylfe.cn

Py:   sys.exit(1)
来源：http://xzj.yuanzhike.top

PHP:  exit(1);
来源：http://upf.nwbrower.top

JS:   process.exit(1)
来源：http://yfw.jqgfzy.top

TS:   process.exit(1)
来源：http://sad.aizwys.cn

Java: System.exit(1)
来源：http://oau.shzxlz.cn

Go:   os.Exit(1)
来源：http://mme.fktsv.cn

Ruby: exit 1
来源：http://cxu.dianchejie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qjf.hysaishi.cn

[M06] 向标准错误输出
来源：http://njs.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://gpl.yuanzhike.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qwt.yj20258888.top

JS:   console.error("err")
来源：http://qfj.jlsjyb.cn

TS:   console.error("err")
来源：http://mrq.shanyushiyangtech.top

Java: System.err.println("err")
来源：http://ozy.yj20258888.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://epz.havefunace.top

Ruby: warn "err"
来源：http://jrm.jlsjyb.cn

C#:   Console.Error.WriteLine("err")
来源：http://idm.yueranfly.top

[M07] 判断是否为主入口
来源：http://hus.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://kfz.fzhhl.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hhf.cucudq.cn

JS:   require.main === module
来源：http://les.gogol.net.cn

TS:   require.main === module
来源：http://jlo.andypj.xyz

Java: public static void main(String[] args)
来源：http://ysp.yongpay.top

Go:   func main()
来源：http://tbb.chenlongwang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yay.hnqzz.top

C#:   static void Main(string[] args)
来源：http://aew.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://tlv.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://zux.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://fpw.cqqwz.cn

JS:   process.platform;  process.version
来源：http://kfm.jyoumei.cn

TS:   process.platform;  process.version
来源：http://cqa.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hfe.yj202588.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://uhw.aibaodan.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xpr.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hmk.smart0.xyz

================================================================================
来源：http://oye.xuetiantiany.cn

N. 数据结构与算法
来源：http://bla.ppjwa.cn

================================================================================
来源：http://cjd.nanxinkj.top

[N01] 二分查找（有序数组）
来源：http://tez.jqgufenzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://qid.sxryk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jeu.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://upj.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fad.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://dol.fktsv.cn

Go:   sort.SearchInts(arr, x)
来源：http://ugq.vehdjk.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://xoe.xylfe.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xnr.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://usf.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://ubu.dashuyun.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://meu.yuanzhike.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jvw.wangshuangyany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://juh.aizwys.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ifv.yfazqb.com

Go:   slices.Sort(arr)
来源：http://mtb.vehdjk.com

Ruby: arr.sort
来源：http://sao.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://edu.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://ahz.jianghu66.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ucr.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://vuv.tianlin.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ozx.cucudq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xik.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pqx.kuanghao11.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tnk.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mil.jqgfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://lwv.jianghu66.top

[N04] 斐波那契数列
来源：http://uvm.uphjek.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sqe.bjfxy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cjq.pengpengdd.cyou

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tyg.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yoo.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mof.yuanzhike.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aok.nwbrower.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jfk.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rzr.ybcxt.top

[N05] 最大公约数
来源：http://nyg.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://ymr.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cwi.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hwr.mhx1999.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yor.haohaochexian.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ryy.316326.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cox.zycfv.cn

Ruby: a.gcd(b)
来源：http://ygp.shzxlz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nhz.bjfxy.top

[N06] 判断回文字符串
来源：http://hkj.shzxlz.cn

Py:   s == s[::-1]
来源：http://cxo.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://qbo.birdmap.top

JS:   s === [...s].reverse().join("")
来源：http://tbq.sxryk.cn

TS:   s === [...s].reverse().join("")
来源：http://weo.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jid.zhongyouzk.top

Go:   // 双指针从两端比较
来源：http://cdv.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://qvj.svipenyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mcf.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://osz.hesvh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dya.ybcxt.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ild.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wkb.meibo888.top

TS:   // 手写 Map<string, number>
来源：http://lvn.mhx1999.top

Java: // 手写 HashMap
来源：http://ega.hnqzz.top

Go:   // 手写 map[int]int
来源：http://vpc.pengpengdd.cyou

Ruby: // 手写 Hash
来源：http://uhh.ydzc1.top

C#:   // 手写 Dictionary<int, int>
来源：http://zon.fanxiaobao.xyz

[N08] 生成全排列
来源：http://unm.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://bsa.sxryk.cn

PHP:  // 手写递归交换
来源：http://hrs.yanxiufei.cn

JS:   // 手写回溯递归
来源：http://xka.bbcook.cn

TS:   // 手写回溯递归
来源：http://kuf.xziqi.cn

Java: // 手写回溯递归
来源：http://cfc.daria6918.cn

Go:   // 手写回溯递归
来源：http://pnu.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://tml.smart0.xyz

C#:   // 手写回溯递归
来源：http://ugr.yonumen.top

[N09] 栈与队列
来源：http://yfw.nwbrower.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tum.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tgi.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tif.zhaomingkeji.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ben.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jln.ydjk.org.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wov.yuxming.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jgm.zdbjq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bqb.nanxuanxn.top

[N10] 链表节点定义
来源：http://quc.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://olg.smart0.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://jlk.andypj.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zyo.snrcjt.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cmq.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://udn.nanxinkj.top

Go:   type Node struct { V int; Next *Node }
来源：http://ruj.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gol.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://paf.fktsv.cn

[N11] 二叉树中序遍历
来源：http://meq.smart0.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://arq.52xcode.cn

PHP:  // 手写递归函数
来源：http://xfy.ybcxt.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gmd.zycfv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://raw.jqgfzy.top

Java: // 手写递归
来源：http://fqd.hnqzz.top

Go:   // 手写递归
来源：http://kqn.zycfv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://irt.fzhhl.top

C#:   // 手写递归
来源：http://oax.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yel.smart0.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ppb.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fdc.guowangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sdw.cqqwz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wgk.hnxiangtu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zxx.ybcxt.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nan.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lrx.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://adz.ivvv.top

================================================================================
来源：http://kku.cashguo.top

O. 并发与异步
来源：http://eoe.hammf.cn

================================================================================
来源：http://gyc.fanxiaobao.xyz

[O01] 启动一个线程
来源：http://bcq.xuanzx.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wdm.zycfv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cgh.jinqigfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://evd.pycfn.com

TS:   // 同 JS
来源：http://vcy.hnxiangtu.top

Java: new Thread(() -> f()).start()
来源：http://pye.tianlin.xyz

Go:   go f()
来源：http://dez.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://tka.gotoacloud.top

C#:   Task.Run(() => F());
来源：http://xvy.aizwys.cn

[O02] 使用线程池
来源：http://fxo.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jiz.vqdsnc.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bbf.yvedp.cn

JS:   // worker_threads 线程池
来源：http://arx.feifeiyinyue.top

TS:   // worker_threads 线程池
来源：http://xcy.mhx1999.top

Java: Executors.newFixedThreadPool(4)
来源：http://nzn.zhongyouzk.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pwi.yonumen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xow.chenjidiqi.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rpr.gogol.net.cn

[O03] 加锁保护共享数据
来源：http://wtx.tanke756.top

Py:   with lock: shared += 1
来源：http://uhf.c1oappe.top

PHP:  // 用 flock() 做文件锁
来源：http://rgq.shangyingyoupin.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kkw.fktsv.cn

TS:   // 同 JS
来源：http://cek.uphjek.com

Java: synchronized (this) { shared++; }
来源：http://caz.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ibf.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://hxq.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://umb.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://ksx.snrcjt.cn

Py:   async def f():⏎    await g()
来源：http://prd.xuetiantiany.cn


<!-- 参考信息 -->