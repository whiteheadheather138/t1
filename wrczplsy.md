代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://izl.epnwcf.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wnd.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ocb.kuanghao11.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xyb.sysykeji.top

[K06] 解析 URL 查询串
来源：http://akc.hongshengwenyu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rwf.zhiwuduotai.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://okh.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nif.chenzaomai.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ftr.snrcjt.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ukj.daria6918.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hwl.zdqjudy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nqq.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ima.ydzc1.top

[K07] 进制转换
来源：http://fyt.sufxvd.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bpr.bjfxy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xbh.pycfn.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dso.hesvh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jdc.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qzw.tian-w.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oim.epnwcf.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ont.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vms.hnxiangtu.top

[K08] 二进制序列化（非 JSON）
来源：http://eqd.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://vcc.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://anc.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://gdo.cucudq.cn

TS:   v8.serialize(obj)        // Node
来源：http://xjy.zdbjq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ncv.yj20258888.top

Go:   encoding/gob
来源：http://xad.guowangkeji.top

Ruby: Marshal.dump(obj)
来源：http://nmq.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jld.gzhubu.top

================================================================================
来源：http://nkt.cashguo.top

L. 网络请求
来源：http://dnk.chenlongwang.top

================================================================================
来源：http://ong.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://ysl.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fdq.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mrx.gaohongyu789.top

JS:   await fetch(url)
来源：http://neg.yfazqb.com

TS:   await fetch(url)
来源：http://ngr.jqgufenzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nmp.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://wzw.bbcook.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yyo.fanxiaobao.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cmh.svipenyu.cn

[L02] 发送 POST JSON
来源：http://htb.birdmap.top

Py:   requests.post(url, json={"a": 1})
来源：http://hne.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yez.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://daf.shangyingyoupin.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fhp.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zrg.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ybx.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qvp.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jlm.gogol.net.cn

[L03] 设置自定义请求头
来源：http://fca.zhixingplan.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://abp.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pgo.xuanzx.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cwc.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ozg.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uax.zhaomingkeji.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dzw.wangdashe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hvx.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bee.birdmap.top

[L04] 设置超时
来源：http://mgj.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://cbs.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zop.svipenyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wur.tarul.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jeq.gotoacloud.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hpp.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hsk.zhaomingkeji.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tgh.9152youxi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nzd.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://nhc.cashguo.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bpw.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xfq.pycfn.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eav.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tva.xuanzx.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ugr.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sfx.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cju.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qlt.daria6918.cn

[L06] 解析响应为 JSON
来源：http://iny.ybcxt.top

Py:   resp.json()
来源：http://dyg.daria6918.cn

PHP:  json_decode($body, true);
来源：http://ymv.jinyuanbaomall.cn

JS:   await resp.json()
来源：http://xyg.yonumen.top

TS:   await resp.json()
来源：http://oeb.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bqr.nwbrower.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lbd.ppjwa.cn

Ruby: JSON.parse(resp.body)
来源：http://zma.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://diu.sxryk.cn

[L07] 处理 HTTP 状态码
来源：http://cmo.fengsongda.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://las.shanyushiyangtech.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qij.ywan-chungtsiang.top

JS:   resp.ok;  resp.status
来源：http://ihi.zhaomingkeji.xyz

TS:   resp.ok;  resp.status
来源：http://jhb.tianlin.xyz

Java: resp.statusCode()
来源：http://ojp.ybcxt.top

Go:   resp.StatusCode
来源：http://sql.yj20258.top

Ruby: resp.code.to_i
来源：http://xwq.nanxuanxn.top

C#:   (int)resp.StatusCode
来源：http://tel.hongshengwenyu.top

[L08] 并发请求多个地址
来源：http://iyu.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fqc.jiagoushi.top

PHP:  curl_multi_init() 系列
来源：http://nxw.svipenyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wla.wangdashe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zee.ppjwa.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uux.iojbl.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uqc.jlsjyb.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tpm.hnqzz.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pnx.aibaodan.cn

================================================================================
来源：http://tmh.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://qbp.hywenlv.cn

================================================================================
来源：http://vzu.nanxinkj.top

[M01] 读取命令行参数
来源：http://zpq.aizwys.cn

Py:   sys.argv[1:]
来源：http://plf.xuanzx.com

PHP:  $argv;  $argc;
来源：http://iqf.jqgufenzy.top

JS:   process.argv.slice(2)
来源：http://pgo.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://wcu.nanxuanxn.top

Java: args 数组（main 方法参数）
来源：http://mqa.zhixingplan.top

Go:   os.Args[1:]
来源：http://xde.hfpthk.cn

Ruby: ARGV
来源：http://bna.zhoulong.xyz

C#:   args 数组（Main 方法参数）
来源：http://kqs.fehbvm.com

[M02] 读取环境变量
来源：http://bdb.cqqwz.cn

Py:   os.environ.get("HOME")
来源：http://rju.zdbjq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gib.hcnkem.com

JS:   process.env.HOME
来源：http://scj.nanxuanxn.top

TS:   process.env.HOME
来源：http://xym.shangyingyoupin.top

Java: System.getenv("HOME")
来源：http://ovd.epnwcf.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bdp.wangdashe.top

Ruby: ENV["HOME"]
来源：http://mhf.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://njc.wangshuangyany.cn

[M03] 执行外部命令
来源：http://zmr.pycfn.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xih.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ipg.52xcode.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ops.cheryme.top

TS:   child_process.execSync("ls -l").toString()
来源：http://oxw.shanyushiyangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rey.sjlbkw.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yrh.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://syh.yfazqb.com

C#:   Process.Start("ls", "-l");
来源：http://tzg.fzhhl.top

[M04] 获取当前工作目录
来源：http://jnd.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://wat.ehwqpu.com

PHP:  getcwd();
来源：http://jno.kuanghao11.cn

JS:   process.cwd()
来源：http://khe.ctjpmb.com

TS:   process.cwd()
来源：http://ycu.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://ehw.sxryk.cn

Go:   os.Getwd()
来源：http://fjr.kuanghao11.cn

Ruby: Dir.pwd
来源：http://gtl.zhijiandao.cn

C#:   Directory.GetCurrentDirectory()
来源：http://exz.hesvh.cn

[M05] 设置退出码
来源：http://lur.sweek.top

Py:   sys.exit(1)
来源：http://qxk.andypj.xyz

PHP:  exit(1);
来源：http://bnw.yvedp.cn

JS:   process.exit(1)
来源：http://ssw.xziqi.cn

TS:   process.exit(1)
来源：http://dbz.yonumen.top

Java: System.exit(1)
来源：http://ips.sweek.top

Go:   os.Exit(1)
来源：http://vye.zdbjq.cn

Ruby: exit 1
来源：http://kjz.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iab.fehbvm.com

[M06] 向标准错误输出
来源：http://gpx.pengpengdd.cyou

Py:   print("err", file=sys.stderr)
来源：http://mnj.gzhubu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pqo.yvedp.cn

JS:   console.error("err")
来源：http://zil.fanxiaobao.xyz

TS:   console.error("err")
来源：http://pfm.cucudq.cn

Java: System.err.println("err")
来源：http://cnh.tarul.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://chd.tarul.cn

Ruby: warn "err"
来源：http://ycj.gotoacloud.top

C#:   Console.Error.WriteLine("err")
来源：http://iys.ywan-chungtsiang.top

[M07] 判断是否为主入口
来源：http://nms.uphjek.com

Py:   if __name__ == "__main__":
来源：http://lqi.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kgn.tian-w.cn

JS:   require.main === module
来源：http://pbg.cashguo.top

TS:   require.main === module
来源：http://cdn.quarkkingdee.top

Java: public static void main(String[] args)
来源：http://fdl.jinyuanbaomall.cn

Go:   func main()
来源：http://ucr.yfazqb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kcx.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://ckq.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://wnv.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://sgc.zhijiandao.cn

PHP:  PHP_OS;  phpversion();
来源：http://ves.cucudq.cn

JS:   process.platform;  process.version
来源：http://xkx.havefunace.top

TS:   process.platform;  process.version
来源：http://ryv.9152youxi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://esv.sysykeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ngw.uphjek.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://unq.chenlongwang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vcs.guannengcc.top

================================================================================
来源：http://mmr.bjfxy.top

N. 数据结构与算法
来源：http://ckn.tian-w.cn

================================================================================
来源：http://dqj.andypj.xyz

[N01] 二分查找（有序数组）
来源：http://mdn.yj20258888.top

Py:   bisect.bisect_left(arr, x)
来源：http://lyd.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mxz.jqgufenzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://via.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xfu.tianlin.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://yht.c1oappe.top

Go:   sort.SearchInts(arr, x)
来源：http://xum.dianchejie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dpy.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tfc.zhaomingkeji.xyz

[N02] 排序（工程实践用内置实现）
来源：http://efq.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://qop.quarkkingdee.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lgn.hongshengwenyu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://cle.tianlin.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://ovb.aibaodan.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://znc.hnqzz.top

Go:   slices.Sort(arr)
来源：http://xxt.jyoumei.cn

Ruby: arr.sort
来源：http://hoc.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://tqp.jianghu66.top

[N03] 快速排序（分治示例）
来源：http://moc.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ssz.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://hoy.havefunace.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bpm.jiagoushi.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cbk.dashuyun.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cqp.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fjm.jianghu66.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bsj.tanke756.top

C#:   // 手写递归，或 Array.Sort
来源：http://tga.nwbrower.top

[N04] 斐波那契数列
来源：http://mxf.yj20258.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gsh.pengpengdd.cyou

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lrf.feifeiyinyue.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://njq.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tqd.jqgufenzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://obc.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wqk.cheryme.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cbs.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://suv.zhengqikj.top

[N05] 最大公约数
来源：http://ouv.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://tmz.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wgt.haohaochexian.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xmh.meibo888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mgv.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://poi.gotoacloud.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vgj.fehbvm.com

Ruby: a.gcd(b)
来源：http://xlt.daxiang520.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hyl.shzxlz.cn

[N06] 判断回文字符串
来源：http://uqt.quarkkingdee.top

Py:   s == s[::-1]
来源：http://ysr.haohaochexian.top

PHP:  $s === strrev($s);
来源：http://mns.xinyue.icu

JS:   s === [...s].reverse().join("")
来源：http://nez.haohaochexian.top

TS:   s === [...s].reverse().join("")
来源：http://dle.zycfv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ufj.shangyingyoupin.top

Go:   // 双指针从两端比较
来源：http://jlv.daxiang520.top

Ruby: s == s.reverse
来源：http://mje.sysykeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tkr.smart0.xyz

[N07] 两数之和（返回下标）
来源：http://zbt.zdbjq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mhj.cdnleiting.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tqr.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://azt.jianghu66.top

TS:   // 手写 Map<string, number>
来源：http://jax.sysykeji.top

Java: // 手写 HashMap
来源：http://frj.smart0.xyz

Go:   // 手写 map[int]int
来源：http://pce.hywenlv.cn

Ruby: // 手写 Hash
来源：http://jim.jinghuilouyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://svg.tian-w.cn

[N08] 生成全排列
来源：http://ibu.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://nlk.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://iwf.epnwcf.com

JS:   // 手写回溯递归
来源：http://yjs.fanxiaobao.xyz

TS:   // 手写回溯递归
来源：http://qyf.shangyingyoupin.top

Java: // 手写回溯递归
来源：http://cme.wangshuangyany.cn

Go:   // 手写回溯递归
来源：http://ugm.yj20258.top

Ruby: arr.permutation.to_a
来源：http://nmz.fktsv.cn

C#:   // 手写回溯递归
来源：http://auy.tian-w.cn

[N09] 栈与队列
来源：http://zzf.52xcode.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mgv.ppjwa.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kry.aibaodan.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://esb.yj20258888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zln.pycfn.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fnt.gogol.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gpj.yangfankeji.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nsd.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wyj.chenzaomai.com

[N10] 链表节点定义
来源：http://rbe.daxiang520.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uja.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ufq.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vqr.dashuyun.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xmd.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://fih.tianlin.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://pyl.xylfe.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yzr.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://boz.feifeiyinyue.top

[N11] 二叉树中序遍历
来源：http://fpf.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nji.yueranfly.top

PHP:  // 手写递归函数
来源：http://jez.jyoumei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mnd.yongpay.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zsi.zhengqikj.top

Java: // 手写递归
来源：http://etq.pycfn.com

Go:   // 手写递归
来源：http://lti.nwbrower.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jex.chenjidiqi.icu

C#:   // 手写递归
来源：http://ilh.ybcxt.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fue.zhaomingkeji.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ywk.cqqwz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wuf.yfazqb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iis.jinyuanbaomall.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ywm.svipenyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bjl.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wgc.dashuyun.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wsi.ppjwa.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bvl.yfazqb.com

================================================================================
来源：http://pyb.sxryk.cn

O. 并发与异步
来源：http://nxf.guannengcc.top

================================================================================
来源：http://wfl.xinyue.icu

[O01] 启动一个线程
来源：http://pga.uphjek.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rdo.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xon.uphjek.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rfm.yanxiufei.cn

TS:   // 同 JS
来源：http://bcm.cheryme.top


<!-- 参考信息 -->