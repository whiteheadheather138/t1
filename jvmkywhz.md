代发 wailian999

[K06] 解析 URL 查询串
来源：http://qqi.xuetiantiany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://azi.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tzc.fanxiaobao.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xab.zhijiandao.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lrd.cdnleiting.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vyj.yuanzhike.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mjx.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iqv.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yee.hesvh.cn

[K07] 进制转换
来源：http://zpb.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nce.xingfuxueyuan.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sfk.cucudq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gka.ybcxt.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mcm.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yuf.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xyi.wangshuangyany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://orr.jinghuilouyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xdl.ydjk.org.cn

[K08] 二进制序列化（非 JSON）
来源：http://fch.zhaomingkeji.xyz

Py:   pickle.dumps(obj)
来源：http://pyx.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xyb.9152youxi.cn

JS:   v8.serialize(obj)        // Node
来源：http://cdi.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://eji.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://scb.xziqi.cn

Go:   encoding/gob
来源：http://fhe.quarkkingdee.top

Ruby: Marshal.dump(obj)
来源：http://pmg.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kuy.birdmap.top

================================================================================
来源：http://dsr.jqgufenzy.top

L. 网络请求
来源：http://mkj.tianlin.xyz

================================================================================
来源：http://jcm.xylfe.cn

[L01] 发送 GET 请求
来源：http://atl.jqgfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://imk.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eeb.zhixingplan.top

JS:   await fetch(url)
来源：http://xsl.sjlbkw.cn

TS:   await fetch(url)
来源：http://zfk.gaohongyu789.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qce.ppjwa.cn

Go:   resp, err := http.Get(url)
来源：http://ocl.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rbi.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yyu.nanxinkj.top

[L02] 发送 POST JSON
来源：http://vng.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tkc.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qvi.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aht.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pki.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://khl.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://edd.smart0.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fux.cdnleiting.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://frm.iojbl.cn

[L03] 设置自定义请求头
来源：http://hzq.xinyue.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qqx.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ptm.fzhhl.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vao.shangyingyoupin.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://acd.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ukb.cdnleiting.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://btx.snrcjt.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bxj.yj20258888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://awx.ctjpmb.com

[L04] 设置超时
来源：http://fbl.zycfv.cn

Py:   requests.get(url, timeout=5)
来源：http://clz.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://twj.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jpj.zhijiandao.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jhk.bbcook.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://owq.ehwqpu.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kxn.yuxming.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qkf.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ctr.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://aqq.fzhhl.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jgh.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rwv.smart0.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cmf.yangfankeji.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://onq.tianlin.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://srg.vqdsnc.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rny.hywenlv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zbh.fengsongda.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ehp.52xcode.cn

[L06] 解析响应为 JSON
来源：http://ndg.gaohongyu789.top

Py:   resp.json()
来源：http://zfu.snrcjt.cn

PHP:  json_decode($body, true);
来源：http://bsl.fanxiaobao.xyz

JS:   await resp.json()
来源：http://ubc.yanxiufei.cn

TS:   await resp.json()
来源：http://qjb.tianlin.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hba.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nfi.quarkkingdee.top

Ruby: JSON.parse(resp.body)
来源：http://jnh.iojbl.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jah.shuidangran.top

[L07] 处理 HTTP 状态码
来源：http://wuo.ydzc1.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ipl.meibo888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gdz.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://cze.cashguo.top

TS:   resp.ok;  resp.status
来源：http://jxi.zhoulong.xyz

Java: resp.statusCode()
来源：http://qlr.9152youxi.cn

Go:   resp.StatusCode
来源：http://ulk.zhixingplan.top

Ruby: resp.code.to_i
来源：http://tgh.zhiwuduotai.top

C#:   (int)resp.StatusCode
来源：http://cqd.c1oappe.top

[L08] 并发请求多个地址
来源：http://wex.andypj.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nue.gaohongyu789.top

PHP:  curl_multi_init() 系列
来源：http://mjr.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gzs.fehbvm.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gvg.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ihw.cheryme.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hsr.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://knh.sweek.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hro.gaohongyu789.top

================================================================================
来源：http://yhi.wangshuangyany.cn

M. 命令行 / 进程 / 环境
来源：http://rkl.vehdjk.com

================================================================================
来源：http://fuo.yfazqb.com

[M01] 读取命令行参数
来源：http://czf.fzhhl.top

Py:   sys.argv[1:]
来源：http://gbs.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://qvl.yj202588.top

JS:   process.argv.slice(2)
来源：http://qbf.andypj.xyz

TS:   process.argv.slice(2)
来源：http://zdu.hcnkem.com

Java: args 数组（main 方法参数）
来源：http://hrf.yj202588.top

Go:   os.Args[1:]
来源：http://xkx.chenlongwang.top

Ruby: ARGV
来源：http://cfj.ehwqpu.com

C#:   args 数组（Main 方法参数）
来源：http://meh.nanxinkj.top

[M02] 读取环境变量
来源：http://csw.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://ick.ydzc1.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dpr.cheryme.top

JS:   process.env.HOME
来源：http://kbj.hysaishi.cn

TS:   process.env.HOME
来源：http://ahq.xinyue.icu

Java: System.getenv("HOME")
来源：http://vxj.snrcjt.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ffi.fehbvm.com

Ruby: ENV["HOME"]
来源：http://oph.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qpq.nwbrower.top

[M03] 执行外部命令
来源：http://ixf.yuanzhike.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kcl.yfazqb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lil.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://hck.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xbj.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qbz.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lfd.yuxming.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zdp.quarkkingdee.top

C#:   Process.Start("ls", "-l");
来源：http://fru.yuxming.cn

[M04] 获取当前工作目录
来源：http://med.nwbrower.top

Py:   os.getcwd()
来源：http://adh.vehdjk.com

PHP:  getcwd();
来源：http://ufq.0kj1m.cn

JS:   process.cwd()
来源：http://dlp.hnqzz.top

TS:   process.cwd()
来源：http://hst.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://czm.jlsjyb.cn

Go:   os.Getwd()
来源：http://jxw.jinqigfzy.top

Ruby: Dir.pwd
来源：http://hwg.jlsjyb.cn

C#:   Directory.GetCurrentDirectory()
来源：http://juc.ppjwa.cn

[M05] 设置退出码
来源：http://hvm.guannengcc.top

Py:   sys.exit(1)
来源：http://zay.aizwys.cn

PHP:  exit(1);
来源：http://nvc.yonumen.top

JS:   process.exit(1)
来源：http://tps.gotoacloud.top

TS:   process.exit(1)
来源：http://uzc.shanyushiyangtech.top

Java: System.exit(1)
来源：http://nmr.9152youxi.cn

Go:   os.Exit(1)
来源：http://egr.hammf.cn

Ruby: exit 1
来源：http://yot.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ern.cucudq.cn

[M06] 向标准错误输出
来源：http://sun.fehbvm.com

Py:   print("err", file=sys.stderr)
来源：http://tmh.zycfv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pmq.wangdashe.top

JS:   console.error("err")
来源：http://bqc.xuanzx.com

TS:   console.error("err")
来源：http://duz.wangshuangyany.cn

Java: System.err.println("err")
来源：http://hyw.guannengcc.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ocb.epnwcf.com

Ruby: warn "err"
来源：http://oda.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://pcj.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://gvq.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://bzf.fengsongda.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cda.shanyushiyangtech.top

JS:   require.main === module
来源：http://dbc.zhongyouzk.top

TS:   require.main === module
来源：http://pvh.andypj.xyz

Java: public static void main(String[] args)
来源：http://idu.jqgfzy.top

Go:   func main()
来源：http://krj.dianchejie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ywa.cqqwz.cn

C#:   static void Main(string[] args)
来源：http://fjg.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://jva.ehwqpu.com

Py:   platform.system();  platform.python_version()
来源：http://tom.yongpay.top

PHP:  PHP_OS;  phpversion();
来源：http://lte.fzhhl.top

JS:   process.platform;  process.version
来源：http://uhn.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://yxx.sysykeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tac.hesvh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xdy.xziqi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zbv.snrcjt.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cry.daria6918.cn

================================================================================
来源：http://wxj.xuetiantiany.cn

N. 数据结构与算法
来源：http://jam.tanke756.top

================================================================================
来源：http://jht.xingfuxueyuan.xyz

[N01] 二分查找（有序数组）
来源：http://ndr.tian-w.cn

Py:   bisect.bisect_left(arr, x)
来源：http://quu.gotoacloud.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kjb.wangshuangyany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ymc.zdbjq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lvq.epnwcf.com

Java: Arrays.binarySearch(arr, x)
来源：http://efk.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://bzg.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wgm.52xcode.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jgh.cashguo.top

[N02] 排序（工程实践用内置实现）
来源：http://ncd.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://ykf.andypj.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jwd.bbcook.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ttd.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://yii.sjlbkw.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nhl.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://shb.zdbjq.cn

Ruby: arr.sort
来源：http://zhh.cheryme.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fkc.vehdjk.com

[N03] 快速排序（分治示例）
来源：http://bkf.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xqm.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://vjq.cdnleiting.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uew.c1oappe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aya.bbcook.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fjx.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lah.sjlbkw.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hvh.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vmv.ppjwa.cn

[N04] 斐波那契数列
来源：http://elj.nanxuanxn.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nsj.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://juv.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bbf.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cyr.tianlin.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nwg.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://teq.shanyushiyangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://doo.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aox.xziqi.cn

[N05] 最大公约数
来源：http://lrd.ivvv.top

Py:   math.gcd(a, b)
来源：http://pqv.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uvu.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bxd.vehdjk.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yfo.zdqjudy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eut.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kdu.tanke756.top

Ruby: a.gcd(b)
来源：http://uop.daria6918.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nsw.yuanzhike.top

[N06] 判断回文字符串
来源：http://yte.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://xqi.shuidangran.top

PHP:  $s === strrev($s);
来源：http://yki.dashuyun.cn

JS:   s === [...s].reverse().join("")
来源：http://mxh.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://nsj.9152youxi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hvi.tarul.cn

Go:   // 双指针从两端比较
来源：http://ace.svipenyu.cn

Ruby: s == s.reverse
来源：http://pvg.ctjpmb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://blk.cheryme.top

[N07] 两数之和（返回下标）
来源：http://vch.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ntz.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tvl.hammf.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zln.feifeiyinyue.top

TS:   // 手写 Map<string, number>
来源：http://pwi.aibaodan.cn

Java: // 手写 HashMap
来源：http://xbk.cashguo.top

Go:   // 手写 map[int]int
来源：http://idb.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://ocg.gotoacloud.top

C#:   // 手写 Dictionary<int, int>
来源：http://scy.yuanzhike.top

[N08] 生成全排列
来源：http://dtr.sysykeji.top

Py:   itertools.permutations(arr)
来源：http://xii.zdqjudy.top

PHP:  // 手写递归交换
来源：http://efg.bjfxy.top

JS:   // 手写回溯递归
来源：http://hbe.chenlongwang.top

TS:   // 手写回溯递归
来源：http://iui.iojbl.cn

Java: // 手写回溯递归
来源：http://ded.ybcxt.top

Go:   // 手写回溯递归
来源：http://cwa.hongshengwenyu.top

Ruby: arr.permutation.to_a
来源：http://xvh.jinghuilouyu.cn

C#:   // 手写回溯递归
来源：http://mwe.gzhubu.top

[N09] 栈与队列
来源：http://kli.nanxinkj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kpu.jiagoushi.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rdk.birdmap.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uwv.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://asv.pengpengdd.cyou

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jzp.shanyushiyangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tev.jinghuilouyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mua.kuanghao11.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uks.zhoulong.xyz

[N10] 链表节点定义
来源：http://umi.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vks.zhijiandao.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ous.svipenyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eem.meibo888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fht.shanyushiyangkeji.top

Java: class Node { int v; Node next; }
来源：http://ygl.cashguo.top

Go:   type Node struct { V int; Next *Node }
来源：http://pni.wangdashe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xmd.sxryk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://omq.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://twt.zhengqikj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qej.cdnleiting.top

PHP:  // 手写递归函数
来源：http://jym.yueranfly.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cni.havefunace.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fpg.xinyue.icu

Java: // 手写递归
来源：http://rcw.cucudq.cn

Go:   // 手写递归
来源：http://qar.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sii.fehbvm.com

C#:   // 手写递归
来源：http://inx.aibaodan.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fkg.hesvh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bos.zhixingplan.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pdh.hongshengwenyu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ncl.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lrg.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qog.hongshengwenyu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xgu.jiagoushi.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ijw.zycfv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ied.yj202588.top

================================================================================
来源：http://cde.yfazqb.com

O. 并发与异步
来源：http://rfp.zhixingplan.top

================================================================================
来源：http://shm.xinyue.icu

[O01] 启动一个线程
来源：http://rrq.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mjd.hongshengwenyu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tag.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wtj.meibo888.top

TS:   // 同 JS
来源：http://rlr.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://qmf.tianlin.xyz

Go:   go f()
来源：http://vdq.haohaochexian.top

Ruby: Thread.new { f }
来源：http://ljd.yongpay.top

C#:   Task.Run(() => F());
来源：http://exo.chenzaomai.com


<!-- 参考信息 -->