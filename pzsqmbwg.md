代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://hll.yongpay.top

PHP:  unserialize(serialize($obj));
来源：http://jdq.snrcjt.cn

JS:   structuredClone(obj)
来源：http://obb.hesvh.cn

TS:   structuredClone(obj)
来源：http://izm.svipenyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zsd.quarkkingdee.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ziz.hywenlv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qrx.fengsongda.top

C#:   // 序列化往返，或自定义 Clone
来源：http://amx.gogol.net.cn

[K06] 解析 URL 查询串
来源：http://jxd.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ryt.sjlbkw.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kag.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dyp.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ute.xinyue.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dzs.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jvv.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uim.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tvn.zhoulong.xyz

[K07] 进制转换
来源：http://zac.havefunace.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lkr.uphjek.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ptw.jyoumei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vus.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nbt.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zhj.yuanzhike.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ikg.dianchejie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ocl.gaohongyu789.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://npx.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://xjj.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://xid.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lak.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://sez.xingfuxueyuan.xyz

TS:   v8.serialize(obj)        // Node
来源：http://qra.yueranfly.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rpd.ivvv.top

Go:   encoding/gob
来源：http://njt.cheryme.top

Ruby: Marshal.dump(obj)
来源：http://cdq.wangdashe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://muy.andypj.xyz

================================================================================
来源：http://uck.zhengqikj.top

L. 网络请求
来源：http://fke.zhijiandao.cn

================================================================================
来源：http://esg.hnqzz.top

[L01] 发送 GET 请求
来源：http://vvv.ctjpmb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://akw.9152youxi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ddl.shzxlz.cn

JS:   await fetch(url)
来源：http://int.dashuyun.cn

TS:   await fetch(url)
来源：http://bgb.tanke756.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rcp.shangyingyoupin.top

Go:   resp, err := http.Get(url)
来源：http://pbd.vqdsnc.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jjw.zhijiandao.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dzd.bjfxy.top

[L02] 发送 POST JSON
来源：http://lnt.guannengcc.top

Py:   requests.post(url, json={"a": 1})
来源：http://bek.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zkc.dashuyun.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pvf.shanyushiyangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vrl.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yhp.birdmap.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gxw.yfazqb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dtl.smart0.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://epx.ywan-chungtsiang.top

[L03] 设置自定义请求头
来源：http://jrq.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://roj.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jvy.dianchejie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hwa.gogol.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ynb.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uvp.fktsv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ckl.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://klc.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://szi.feifeiyinyue.top

[L04] 设置超时
来源：http://qun.zhiwuduotai.top

Py:   requests.get(url, timeout=5)
来源：http://zfi.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rsn.cucudq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://int.yuxming.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://who.cashguo.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vjy.jqgfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rgf.sxryk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tyb.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://npy.hysaishi.cn

[L05] 上传文件（multipart）
来源：http://lga.yanxiufei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://juw.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tos.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cwg.mhx1999.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://etd.fzhhl.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jrh.ppjwa.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qtb.316326.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jrh.chenzaomai.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mue.haohaochexian.top

[L06] 解析响应为 JSON
来源：http://bzv.tarul.cn

Py:   resp.json()
来源：http://zlc.nwbrower.top

PHP:  json_decode($body, true);
来源：http://ywq.ehwqpu.com

JS:   await resp.json()
来源：http://dyw.xuanzx.com

TS:   await resp.json()
来源：http://qsd.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mtg.zhixingplan.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vak.zdqjudy.top

Ruby: JSON.parse(resp.body)
来源：http://rpd.cdnleiting.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://aus.sxryk.cn

[L07] 处理 HTTP 状态码
来源：http://igl.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kcn.birdmap.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lln.hysaishi.cn

JS:   resp.ok;  resp.status
来源：http://hhm.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://fth.daria6918.cn

Java: resp.statusCode()
来源：http://obe.zdqjudy.top

Go:   resp.StatusCode
来源：http://iqb.guowangkeji.top

Ruby: resp.code.to_i
来源：http://hav.52xcode.cn

C#:   (int)resp.StatusCode
来源：http://qfo.ehwqpu.com

[L08] 并发请求多个地址
来源：http://pyy.yuanzhike.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vxe.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://ypi.ivvv.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rrq.epnwcf.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gaq.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ssw.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zpk.shanyushiyangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ilv.hysaishi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iwi.cqqwz.cn

================================================================================
来源：http://eeo.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境
来源：http://kvt.jlsjyb.cn

================================================================================
来源：http://xqx.aizwys.cn

[M01] 读取命令行参数
来源：http://suw.yueranfly.top

Py:   sys.argv[1:]
来源：http://kox.shuidangran.top

PHP:  $argv;  $argc;
来源：http://eoo.yonumen.top

JS:   process.argv.slice(2)
来源：http://dqi.jlsjyb.cn

TS:   process.argv.slice(2)
来源：http://hbq.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://lmw.gzhubu.top

Go:   os.Args[1:]
来源：http://jmd.nanxinkj.top

Ruby: ARGV
来源：http://qza.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://fkz.meibo888.top

[M02] 读取环境变量
来源：http://oyc.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://owr.aizwys.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lid.zhixingplan.top

JS:   process.env.HOME
来源：http://jbl.haohaochexian.top

TS:   process.env.HOME
来源：http://inl.andypj.xyz

Java: System.getenv("HOME")
来源：http://kzi.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ali.yonumen.top

Ruby: ENV["HOME"]
来源：http://uet.shangyingyoupin.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nji.iojbl.cn

[M03] 执行外部命令
来源：http://otu.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eos.0kj1m.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://amm.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kzw.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ier.smart0.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://egu.chenlongwang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qhk.yj202588.top

Ruby: system("ls -l");  `ls -l`
来源：http://cep.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://xke.yangfankeji.com

[M04] 获取当前工作目录
来源：http://afj.tianlin.xyz

Py:   os.getcwd()
来源：http://ubq.gogol.net.cn

PHP:  getcwd();
来源：http://kdi.0kj1m.cn

JS:   process.cwd()
来源：http://yja.vqdsnc.cn

TS:   process.cwd()
来源：http://fgm.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://isd.haohaochexian.top

Go:   os.Getwd()
来源：http://xvs.zdbjq.cn

Ruby: Dir.pwd
来源：http://dnt.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://ukd.sysykeji.top

[M05] 设置退出码
来源：http://mql.c1oappe.top

Py:   sys.exit(1)
来源：http://uhb.jinqigufen.top

PHP:  exit(1);
来源：http://pix.ydjk.org.cn

JS:   process.exit(1)
来源：http://qoj.yfazqb.com

TS:   process.exit(1)
来源：http://ohe.9152youxi.cn

Java: System.exit(1)
来源：http://djh.yuanzhike.top

Go:   os.Exit(1)
来源：http://lej.zhaomingkeji.xyz

Ruby: exit 1
来源：http://gsb.yuxming.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wmu.316326.xyz

[M06] 向标准错误输出
来源：http://zza.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://gyr.hnqzz.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pfw.yj20258.top

JS:   console.error("err")
来源：http://ono.xinyue.icu

TS:   console.error("err")
来源：http://hwm.jqgufenzy.top

Java: System.err.println("err")
来源：http://cul.wangshuangyany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nkg.chenlongwang.top

Ruby: warn "err"
来源：http://zfm.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://lwu.jqgfzy.top

[M07] 判断是否为主入口
来源：http://aiv.ehwqpu.com

Py:   if __name__ == "__main__":
来源：http://pcc.fehbvm.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sxk.sweek.top

JS:   require.main === module
来源：http://wtq.yongpay.top

TS:   require.main === module
来源：http://rfi.iojbl.cn

Java: public static void main(String[] args)
来源：http://ogp.zhiwuduotai.top

Go:   func main()
来源：http://ita.tarul.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tgj.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://yil.jyoumei.cn

[M08] 获取系统与运行时信息
来源：http://iqn.daria6918.cn

Py:   platform.system();  platform.python_version()
来源：http://lsf.hcnkem.com

PHP:  PHP_OS;  phpversion();
来源：http://aft.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://pgv.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://mud.shangyingyoupin.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qmv.zycfv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yfo.kuanghao11.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vvm.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xeo.zhoulong.xyz

================================================================================
来源：http://rwr.aibaodan.cn

N. 数据结构与算法
来源：http://tbx.iojbl.cn

================================================================================
来源：http://fbd.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://itp.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dez.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xzj.dianchejie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uls.svipenyu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dns.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://rrt.uphjek.com

Go:   sort.SearchInts(arr, x)
来源：http://rch.feifeiyinyue.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bgg.tian-w.cn

C#:   Array.BinarySearch(arr, x)
来源：http://exd.jiagoushi.top

[N02] 排序（工程实践用内置实现）
来源：http://sam.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://kei.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pkl.jinqigufen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ayu.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://qeu.hcnkem.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ixd.cdnleiting.top

Go:   slices.Sort(arr)
来源：http://trw.svipenyu.cn

Ruby: arr.sort
来源：http://spc.ybcxt.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jxf.iojbl.cn

[N03] 快速排序（分治示例）
来源：http://bmq.sweek.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://svb.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://xzh.jiagoushi.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fmb.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gzi.vqdsnc.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zdt.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cez.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ehz.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://ber.gaohongyu789.top

[N04] 斐波那契数列
来源：http://ifs.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hqi.daria6918.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://twf.smart0.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xoa.jinqigufen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hzz.pycfn.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aqb.shzxlz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zvq.zhaomingkeji.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://umn.redwolf501.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yrp.sweek.top

[N05] 最大公约数
来源：http://giu.snrcjt.cn

Py:   math.gcd(a, b)
来源：http://wdl.hesvh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cyj.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eta.9152youxi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gek.yueranfly.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wue.dianchejie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qgw.uphjek.com

Ruby: a.gcd(b)
来源：http://lsw.yanxiufei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qul.jyoumei.cn

[N06] 判断回文字符串
来源：http://upu.yangfankeji.com

Py:   s == s[::-1]
来源：http://nls.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://xnx.birdmap.top

JS:   s === [...s].reverse().join("")
来源：http://tlv.dashuyun.cn

TS:   s === [...s].reverse().join("")
来源：http://ipf.gaohongyu789.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pba.ybcxt.top

Go:   // 双指针从两端比较
来源：http://arj.hfpthk.cn

Ruby: s == s.reverse
来源：http://zin.xuetiantiany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jyw.shuidangran.top

[N07] 两数之和（返回下标）
来源：http://exd.nanxinkj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fxa.yueranfly.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://moz.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://orv.chenzaomai.com

TS:   // 手写 Map<string, number>
来源：http://kob.ydzc1.top

Java: // 手写 HashMap
来源：http://rxh.wangdashe.top

Go:   // 手写 map[int]int
来源：http://nel.yuanzhike.top

Ruby: // 手写 Hash
来源：http://iwp.svipenyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xid.ywan-chungtsiang.top

[N08] 生成全排列
来源：http://ibc.ppjwa.cn

Py:   itertools.permutations(arr)
来源：http://djd.aizwys.cn

PHP:  // 手写递归交换
来源：http://pde.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://exn.shanyushiyangtech.top

TS:   // 手写回溯递归
来源：http://agb.quarkkingdee.top

Java: // 手写回溯递归
来源：http://qnk.gogol.net.cn

Go:   // 手写回溯递归
来源：http://tzj.ydzc1.top

Ruby: arr.permutation.to_a
来源：http://zav.sjlbkw.cn

C#:   // 手写回溯递归
来源：http://lmw.yangfankeji.com

[N09] 栈与队列
来源：http://cdr.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xsw.jqgufenzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qbs.yongpay.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jqa.9152youxi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://idv.zhixingplan.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jve.jinghuilouyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://skv.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ddw.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dsj.epnwcf.com

[N10] 链表节点定义
来源：http://gig.xuanzx.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ffw.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jwk.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zyp.cheryme.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://who.tian-w.cn

Java: class Node { int v; Node next; }
来源：http://vic.zhiwuduotai.top

Go:   type Node struct { V int; Next *Node }
来源：http://aiz.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://zbk.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bch.yuxming.cn

[N11] 二叉树中序遍历
来源：http://gfc.smart0.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eku.dashuyun.cn

PHP:  // 手写递归函数
来源：http://inu.yuxming.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mgh.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zap.yanxiufei.cn

Java: // 手写递归
来源：http://jwc.shuidangran.top

Go:   // 手写递归
来源：http://zfs.aibaodan.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hbn.andypj.xyz

C#:   // 手写递归
来源：http://dll.ywan-chungtsiang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fxb.aibaodan.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://std.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wkw.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jpq.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mkg.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uau.daria6918.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rom.hywenlv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://efd.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ghk.chenjidiqi.icu

================================================================================
来源：http://cdj.cqqwz.cn

O. 并发与异步
来源：http://fpk.jqgfzy.top

================================================================================
来源：http://tve.quarkkingdee.top

[O01] 启动一个线程
来源：http://ylr.tarul.cn


<!-- 参考信息 -->