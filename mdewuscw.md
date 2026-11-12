代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hha.zhongyouzk.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yma.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cfy.xuanzx.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vte.yanxiufei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sjs.cdnleiting.top

[K07] 进制转换
来源：http://bcr.zhixingplan.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jzv.fehbvm.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aar.epnwcf.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://weo.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://arn.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ihk.yfazqb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gdi.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zub.yueranfly.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ngw.gzhubu.top

[K08] 二进制序列化（非 JSON）
来源：http://zmt.havefunace.top

Py:   pickle.dumps(obj)
来源：http://ojo.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jcf.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://sto.daria6918.cn

TS:   v8.serialize(obj)        // Node
来源：http://eqh.hnxiangtu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tnh.yuanzhike.top

Go:   encoding/gob
来源：http://fdv.vqdsnc.cn

Ruby: Marshal.dump(obj)
来源：http://oxp.andypj.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gjy.smart0.xyz

================================================================================
来源：http://jkt.svipenyu.cn

L. 网络请求
来源：http://suf.jinyuanbaomall.cn

================================================================================
来源：http://zmq.zdbjq.cn

[L01] 发送 GET 请求
来源：http://vgr.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://enm.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xeg.0kj1m.cn

JS:   await fetch(url)
来源：http://rpg.zhoulong.xyz

TS:   await fetch(url)
来源：http://gki.yanxiufei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aar.birdmap.top

Go:   resp, err := http.Get(url)
来源：http://iyd.bjfxy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vki.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nhy.jqgfzy.top

[L02] 发送 POST JSON
来源：http://hcl.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://duu.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vkd.ppjwa.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tcl.xuanzx.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xwn.vqdsnc.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qym.nwbrower.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mvh.ydzc1.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://udo.zycfv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lpk.havefunace.top

[L03] 设置自定义请求头
来源：http://zqv.xziqi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yie.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tse.zhaomingkeji.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gvw.zycfv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pbk.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://klt.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xwj.shangyingyoupin.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://niv.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aei.jinqigfzy.top

[L04] 设置超时
来源：http://dev.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://zvx.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wrn.hnqzz.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xtu.zdqjudy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://arl.hongshengwenyu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://djf.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ifd.cucudq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hiq.daxiang520.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xai.yanxiufei.cn

[L05] 上传文件（multipart）
来源：http://lhx.dianchejie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uzn.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hyi.yj202588.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pql.yfazqb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rpy.yfazqb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ovo.0kj1m.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xat.yuanzhike.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kks.cucudq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pgk.wangshuangyany.cn

[L06] 解析响应为 JSON
来源：http://ode.52xcode.cn

Py:   resp.json()
来源：http://jkn.zhiwuduotai.top

PHP:  json_decode($body, true);
来源：http://rgk.hcnkem.com

JS:   await resp.json()
来源：http://urz.haohaochexian.top

TS:   await resp.json()
来源：http://jmi.aizwys.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iyl.aizwys.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ezy.0kj1m.cn

Ruby: JSON.parse(resp.body)
来源：http://rwa.ydjk.org.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yui.kuanghao11.cn

[L07] 处理 HTTP 状态码
来源：http://mze.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iix.feifeiyinyue.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sma.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://kyk.bbcook.cn

TS:   resp.ok;  resp.status
来源：http://muo.xingfuxueyuan.xyz

Java: resp.statusCode()
来源：http://mip.svipenyu.cn

Go:   resp.StatusCode
来源：http://rds.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://omv.zycfv.cn

C#:   (int)resp.StatusCode
来源：http://mcl.jianghu66.top

[L08] 并发请求多个地址
来源：http://laj.jiagoushi.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kql.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://pwq.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nhk.sweek.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://imz.52xcode.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wuj.guowangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ebr.zycfv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nuv.hysaishi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wow.jinqigfzy.top

================================================================================
来源：http://zdv.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://vlk.sysykeji.top

================================================================================
来源：http://jgw.zhengqikj.top

[M01] 读取命令行参数
来源：http://jyy.chenlongwang.top

Py:   sys.argv[1:]
来源：http://bsz.jinghuilouyu.cn

PHP:  $argv;  $argc;
来源：http://zww.yueranfly.top

JS:   process.argv.slice(2)
来源：http://ymb.guowangkeji.top

TS:   process.argv.slice(2)
来源：http://nhy.xinyue.icu

Java: args 数组（main 方法参数）
来源：http://jxl.ywan-chungtsiang.top

Go:   os.Args[1:]
来源：http://nif.xinyue.icu

Ruby: ARGV
来源：http://fnz.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://bjh.chenzaomai.com

[M02] 读取环境变量
来源：http://cde.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://xpy.hywenlv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fxs.316326.xyz

JS:   process.env.HOME
来源：http://lwi.gotoacloud.top

TS:   process.env.HOME
来源：http://bvm.jinqigufen.top

Java: System.getenv("HOME")
来源：http://bup.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hov.hammf.cn

Ruby: ENV["HOME"]
来源：http://xkf.ydjk.org.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://net.cdnleiting.top

[M03] 执行外部命令
来源：http://oyp.smart0.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jyk.yvedp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vsh.jiagoushi.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pso.hcnkem.com

TS:   child_process.execSync("ls -l").toString()
来源：http://ofb.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yrv.nanxinkj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qbn.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://idw.cashguo.top

C#:   Process.Start("ls", "-l");
来源：http://yqz.cqqwz.cn

[M04] 获取当前工作目录
来源：http://hvn.cheryme.top

Py:   os.getcwd()
来源：http://ybq.andypj.xyz

PHP:  getcwd();
来源：http://lzj.xylfe.cn

JS:   process.cwd()
来源：http://iqu.vqdsnc.cn

TS:   process.cwd()
来源：http://icb.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://vgt.jinqigufen.top

Go:   os.Getwd()
来源：http://rnw.316326.xyz

Ruby: Dir.pwd
来源：http://olu.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://lyr.c1oappe.top

[M05] 设置退出码
来源：http://gcm.hywenlv.cn

Py:   sys.exit(1)
来源：http://ynp.nanxinkj.top

PHP:  exit(1);
来源：http://rsm.yangfankeji.com

JS:   process.exit(1)
来源：http://wgp.yj20258888.top

TS:   process.exit(1)
来源：http://xai.andypj.xyz

Java: System.exit(1)
来源：http://pfi.gzhubu.top

Go:   os.Exit(1)
来源：http://atc.zhijiandao.cn

Ruby: exit 1
来源：http://jhh.jlsjyb.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iyl.haohaochexian.top

[M06] 向标准错误输出
来源：http://rtp.xuetiantiany.cn

Py:   print("err", file=sys.stderr)
来源：http://qvm.xziqi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://edm.52xcode.cn

JS:   console.error("err")
来源：http://wdi.tianlin.xyz

TS:   console.error("err")
来源：http://jel.wangdashe.top

Java: System.err.println("err")
来源：http://cgy.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iyc.guannengcc.top

Ruby: warn "err"
来源：http://emi.guannengcc.top

C#:   Console.Error.WriteLine("err")
来源：http://dju.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://aah.cashguo.top

Py:   if __name__ == "__main__":
来源：http://vbb.tian-w.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://imd.shanyushiyangtech.top

JS:   require.main === module
来源：http://ovt.tarul.cn

TS:   require.main === module
来源：http://ymy.xinyue.icu

Java: public static void main(String[] args)
来源：http://vmx.zhaomingkeji.xyz

Go:   func main()
来源：http://vlw.hongshengwenyu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://aut.316326.xyz

C#:   static void Main(string[] args)
来源：http://kvu.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://txk.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://jps.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://tku.ctjpmb.com

JS:   process.platform;  process.version
来源：http://npo.tarul.cn

TS:   process.platform;  process.version
来源：http://iuu.hfpthk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rrf.jiagoushi.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qre.jqgfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vda.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uiy.gaohongyu789.top

================================================================================
来源：http://yrb.xziqi.cn

N. 数据结构与算法
来源：http://rhr.aibaodan.cn

================================================================================
来源：http://tpe.chenzaomai.com

[N01] 二分查找（有序数组）
来源：http://ynk.316326.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://qkd.gzhubu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uno.cdnleiting.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sed.jlsjyb.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://noc.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://nlb.hesvh.cn

Go:   sort.SearchInts(arr, x)
来源：http://ixd.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://oic.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://hxa.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://hyg.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://clp.hnqzz.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iza.jinghuilouyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zcm.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://stb.zdqjudy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aac.cashguo.top

Go:   slices.Sort(arr)
来源：http://woo.gogol.net.cn

Ruby: arr.sort
来源：http://pca.hcnkem.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://odt.gzhubu.top

[N03] 快速排序（分治示例）
来源：http://vrd.shanyushiyangtech.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pko.xuanzx.com

PHP:  // 递归实现，或用 usort
来源：http://nvi.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nhd.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mhu.316326.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vrn.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dsu.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vuz.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://zyz.uphjek.com

[N04] 斐波那契数列
来源：http://gwh.52xcode.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dsw.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lcr.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jvt.fengsongda.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ccz.vehdjk.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kza.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lmx.meibo888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rdt.yj20258888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qym.fengsongda.top

[N05] 最大公约数
来源：http://bmz.cqqwz.cn

Py:   math.gcd(a, b)
来源：http://hts.xinyue.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://djb.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lnm.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zcr.gotoacloud.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dpd.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cmk.sufxvd.cn

Ruby: a.gcd(b)
来源：http://tbu.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://amh.xinyue.icu

[N06] 判断回文字符串
来源：http://vse.snrcjt.cn

Py:   s == s[::-1]
来源：http://eee.guannengcc.top

PHP:  $s === strrev($s);
来源：http://hpf.0kj1m.cn

JS:   s === [...s].reverse().join("")
来源：http://fkb.jlsjyb.cn

TS:   s === [...s].reverse().join("")
来源：http://fzl.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hvm.sysykeji.top

Go:   // 双指针从两端比较
来源：http://lac.ivvv.top

Ruby: s == s.reverse
来源：http://crx.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nvj.yonumen.top

[N07] 两数之和（返回下标）
来源：http://jys.ybcxt.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://axv.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iep.yangfankeji.com

JS:   // 手写 Map：map.set(v, i)
来源：http://yfv.sufxvd.cn

TS:   // 手写 Map<string, number>
来源：http://pkw.epnwcf.com

Java: // 手写 HashMap
来源：http://ztl.hammf.cn

Go:   // 手写 map[int]int
来源：http://epk.guannengcc.top

Ruby: // 手写 Hash
来源：http://iwk.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://tnh.shanyushiyangtech.top

[N08] 生成全排列
来源：http://xcb.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://oyc.sufxvd.cn

PHP:  // 手写递归交换
来源：http://vjq.ctjpmb.com

JS:   // 手写回溯递归
来源：http://akd.guannengcc.top

TS:   // 手写回溯递归
来源：http://ybc.jlsjyb.cn

Java: // 手写回溯递归
来源：http://ulf.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://qth.yongpay.top

Ruby: arr.permutation.to_a
来源：http://xeo.xylfe.cn

C#:   // 手写回溯递归
来源：http://ivj.shanyushiyangtech.top

[N09] 栈与队列
来源：http://ixv.hfpthk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jlp.zhoulong.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gic.shanyushiyangtech.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lws.52xcode.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wnf.tian-w.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://koc.yonumen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bql.hnqzz.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xet.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jsj.guannengcc.top

[N10] 链表节点定义
来源：http://yme.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qfr.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://eha.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kza.yvedp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vec.zhongyouzk.top

Java: class Node { int v; Node next; }
来源：http://dqx.yj202588.top

Go:   type Node struct { V int; Next *Node }
来源：http://abo.shanyushiyangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://daq.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wpn.smart0.xyz

[N11] 二叉树中序遍历
来源：http://wuz.zhiwuduotai.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://krd.yj202588.top

PHP:  // 手写递归函数
来源：http://rwb.birdmap.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://njv.jinghuilouyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vlj.snrcjt.cn

Java: // 手写递归
来源：http://xub.jyoumei.cn

Go:   // 手写递归
来源：http://qgf.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cqg.wangdashe.top

C#:   // 手写递归
来源：http://xzn.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lwk.vehdjk.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bjq.0kj1m.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yna.jinqigufen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eap.yongpay.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://esa.bjfxy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ajn.ydzc1.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bzg.birdmap.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tif.hesvh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kbn.yuanzhike.top

================================================================================
来源：http://tum.0kj1m.cn

O. 并发与异步
来源：http://tcx.gotoacloud.top

================================================================================
来源：http://ffg.gogol.net.cn

[O01] 启动一个线程
来源：http://hyw.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nod.yueranfly.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://msi.zhoulong.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fzw.zhijiandao.cn

TS:   // 同 JS
来源：http://mpq.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://cnz.ehwqpu.com

Go:   go f()
来源：http://fru.andypj.xyz

Ruby: Thread.new { f }
来源：http://nlb.yuanzhike.top

C#:   Task.Run(() => F());
来源：http://ery.uphjek.com

[O02] 使用线程池
来源：http://pic.fengsongda.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gxt.cheryme.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jvt.jianghu66.top

JS:   // worker_threads 线程池
来源：http://apn.cucudq.cn


<!-- 参考信息 -->