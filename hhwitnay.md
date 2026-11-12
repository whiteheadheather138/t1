代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rgz.shanyushiyangtech.top

[K03] JSON 美化输出（带缩进）
来源：http://ifl.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gsw.pengpengdd.cyou

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mlc.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://use.xinyue.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://fqf.zhaomingkeji.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rop.tian-w.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jtn.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://rkd.cdnleiting.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fdz.tianlin.xyz

[K04] 读取 JSON 文件
来源：http://rtz.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dgd.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://txp.daxiang520.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://klz.dianchejie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://val.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rnq.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sly.havefunace.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bnf.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://swp.aibaodan.cn

[K05] 深拷贝对象
来源：http://ixq.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://fho.ctjpmb.com

PHP:  unserialize(serialize($obj));
来源：http://oag.guannengcc.top

JS:   structuredClone(obj)
来源：http://mqu.jyoumei.cn

TS:   structuredClone(obj)
来源：http://uax.cdnleiting.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vuf.wangshuangyany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tdd.xuetiantiany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fqk.vehdjk.com

C#:   // 序列化往返，或自定义 Clone
来源：http://jhi.epnwcf.com

[K06] 解析 URL 查询串
来源：http://nfu.xingfuxueyuan.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://imz.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nmh.aizwys.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bsy.fktsv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rgy.9152youxi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iuh.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rpu.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oed.bbcook.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kvx.nwbrower.top

[K07] 进制转换
来源：http://yeg.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://olc.havefunace.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lxy.yj202588.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sdd.dashuyun.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nfo.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yrt.jinyuanbaomall.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hqg.hfpthk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kqx.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jbd.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://ahq.yonumen.top

Py:   pickle.dumps(obj)
来源：http://nge.vehdjk.com

PHP:  serialize($obj);  unserialize($s);
来源：http://ghc.xylfe.cn

JS:   v8.serialize(obj)        // Node
来源：http://dlu.daxiang520.top

TS:   v8.serialize(obj)        // Node
来源：http://cld.jinyuanbaomall.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sxe.zhongyouzk.top

Go:   encoding/gob
来源：http://eck.zhaomingkeji.xyz

Ruby: Marshal.dump(obj)
来源：http://gwc.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://htu.jlsjyb.cn

================================================================================
来源：http://ojs.hysaishi.cn

L. 网络请求
来源：http://vgr.vehdjk.com

================================================================================
来源：http://imy.havefunace.top

[L01] 发送 GET 请求
来源：http://fgk.tarul.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rko.jqgufenzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vij.jinghuilouyu.cn

JS:   await fetch(url)
来源：http://zml.tianlin.xyz

TS:   await fetch(url)
来源：http://qhb.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rdi.zdbjq.cn

Go:   resp, err := http.Get(url)
来源：http://jyf.fengsongda.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tau.fktsv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sdm.ppjwa.cn

[L02] 发送 POST JSON
来源：http://cqp.sxryk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dvf.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yzt.snrcjt.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lbo.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rqs.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://unw.xingfuxueyuan.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fjn.zdqjudy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://maf.zhaomingkeji.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fqa.smart0.xyz

[L03] 设置自定义请求头
来源：http://xkp.jinghuilouyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nee.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vok.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wdt.gaohongyu789.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kyz.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sfr.yonumen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eoe.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xqw.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wou.hysaishi.cn

[L04] 设置超时
来源：http://cbj.vqdsnc.cn

Py:   requests.get(url, timeout=5)
来源：http://cof.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kqs.zhoulong.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fhc.jinqigufen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wxe.vqdsnc.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jvn.hnqzz.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gjv.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iyg.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lcu.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://vob.jlsjyb.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kll.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ugu.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nfq.zdbjq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wkh.ctjpmb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sdq.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kyw.quarkkingdee.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xhp.sjlbkw.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bmb.yueranfly.top

[L06] 解析响应为 JSON
来源：http://fya.jyoumei.cn

Py:   resp.json()
来源：http://ygd.ywan-chungtsiang.top

PHP:  json_decode($body, true);
来源：http://zgu.daxiang520.top

JS:   await resp.json()
来源：http://jgf.sjlbkw.cn

TS:   await resp.json()
来源：http://cvo.ybcxt.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gnp.yanxiufei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aqw.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://yox.ydjk.org.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dcv.cqqwz.cn

[L07] 处理 HTTP 状态码
来源：http://yoa.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dfd.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ehl.yueranfly.top

JS:   resp.ok;  resp.status
来源：http://wds.yangfankeji.com

TS:   resp.ok;  resp.status
来源：http://elg.iojbl.cn

Java: resp.statusCode()
来源：http://eec.epnwcf.com

Go:   resp.StatusCode
来源：http://fil.fktsv.cn

Ruby: resp.code.to_i
来源：http://txo.jinqigfzy.top

C#:   (int)resp.StatusCode
来源：http://lfy.shuidangran.top

[L08] 并发请求多个地址
来源：http://qcu.zdqjudy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zrf.sjlbkw.cn

PHP:  curl_multi_init() 系列
来源：http://xoc.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lkc.uphjek.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wlo.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ohs.hesvh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tgh.ydjk.org.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fbp.yongpay.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rjp.ybcxt.top

================================================================================
来源：http://aps.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://fjt.xuanzx.com

================================================================================
来源：http://hzy.zhixingplan.top

[M01] 读取命令行参数
来源：http://tcm.gaohongyu789.top

Py:   sys.argv[1:]
来源：http://daa.yj20258888.top

PHP:  $argv;  $argc;
来源：http://xpk.bjfxy.top

JS:   process.argv.slice(2)
来源：http://ims.iojbl.cn

TS:   process.argv.slice(2)
来源：http://llg.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://nnh.ydzc1.top

Go:   os.Args[1:]
来源：http://xoq.316326.xyz

Ruby: ARGV
来源：http://wuw.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://euj.xingfuxueyuan.xyz

[M02] 读取环境变量
来源：http://svo.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://vly.pengpengdd.cyou

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ycs.sysykeji.top

JS:   process.env.HOME
来源：http://lwm.cheryme.top

TS:   process.env.HOME
来源：http://oay.xuetiantiany.cn

Java: System.getenv("HOME")
来源：http://uoq.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qxg.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://ams.quarkkingdee.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://koc.316326.xyz

[M03] 执行外部命令
来源：http://gra.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rmj.ydzc1.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cbx.chenjidiqi.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://ccn.hcnkem.com

TS:   child_process.execSync("ls -l").toString()
来源：http://nrj.yj202588.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cql.epnwcf.com

Go:   exec.Command("ls", "-l").Output()
来源：http://tnq.316326.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://nhy.hnxiangtu.top

C#:   Process.Start("ls", "-l");
来源：http://wfe.snrcjt.cn

[M04] 获取当前工作目录
来源：http://npc.svipenyu.cn

Py:   os.getcwd()
来源：http://ajc.svipenyu.cn

PHP:  getcwd();
来源：http://ops.316326.xyz

JS:   process.cwd()
来源：http://kik.jlsjyb.cn

TS:   process.cwd()
来源：http://xip.tanke756.top

Java: Path.of("").toAbsolutePath()
来源：http://tah.zhengqikj.top

Go:   os.Getwd()
来源：http://isq.zdbjq.cn

Ruby: Dir.pwd
来源：http://dwk.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qxg.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://pqb.ydjk.org.cn

Py:   sys.exit(1)
来源：http://rrf.yuxming.cn

PHP:  exit(1);
来源：http://rpm.gotoacloud.top

JS:   process.exit(1)
来源：http://aei.jinyuanbaomall.cn

TS:   process.exit(1)
来源：http://jxd.dashuyun.cn

Java: System.exit(1)
来源：http://cza.fktsv.cn

Go:   os.Exit(1)
来源：http://ysl.fehbvm.com

Ruby: exit 1
来源：http://wqg.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://byq.daxiang520.top

[M06] 向标准错误输出
来源：http://fyh.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://lnw.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cuy.hammf.cn

JS:   console.error("err")
来源：http://unu.yj20258888.top

TS:   console.error("err")
来源：http://sxa.hongshengwenyu.top

Java: System.err.println("err")
来源：http://gwl.xylfe.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jvm.pycfn.com

Ruby: warn "err"
来源：http://dtl.chenzaomai.com

C#:   Console.Error.WriteLine("err")
来源：http://gdn.zdqjudy.top

[M07] 判断是否为主入口
来源：http://chc.tarul.cn

Py:   if __name__ == "__main__":
来源：http://cpj.xuetiantiany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qlw.zhoulong.xyz

JS:   require.main === module
来源：http://mgm.bjfxy.top

TS:   require.main === module
来源：http://wvw.mhx1999.top

Java: public static void main(String[] args)
来源：http://nzt.hysaishi.cn

Go:   func main()
来源：http://fqj.tanke756.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jln.jianghu66.top

C#:   static void Main(string[] args)
来源：http://qfi.jlsjyb.cn

[M08] 获取系统与运行时信息
来源：http://cee.xuanzx.com

Py:   platform.system();  platform.python_version()
来源：http://rrz.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://gwg.hywenlv.cn

JS:   process.platform;  process.version
来源：http://eyl.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://lgw.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rsh.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hvq.zhixingplan.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mla.yj202588.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dbn.nwbrower.top

================================================================================
来源：http://wgv.shanyushiyangtech.top

N. 数据结构与算法
来源：http://flj.c1oappe.top

================================================================================
来源：http://bhg.hongshengwenyu.top

[N01] 二分查找（有序数组）
来源：http://eyu.andypj.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://qzp.shanyushiyangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://otb.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fvg.fanxiaobao.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dqd.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://cwr.sysykeji.top

Go:   sort.SearchInts(arr, x)
来源：http://kxs.jqgufenzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mcg.jinghuilouyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://isw.uphjek.com

[N02] 排序（工程实践用内置实现）
来源：http://hxo.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://kym.tian-w.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://raj.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kyq.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://eee.shanyushiyangtech.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rnh.hongshengwenyu.top

Go:   slices.Sort(arr)
来源：http://sjm.hfpthk.cn

Ruby: arr.sort
来源：http://kvy.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://ghb.daria6918.cn

[N03] 快速排序（分治示例）
来源：http://olu.chenlongwang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vor.vehdjk.com

PHP:  // 递归实现，或用 usort
来源：http://wxs.chenzaomai.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wrk.tanke756.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vvv.gotoacloud.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qxe.hnxiangtu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xzc.hnqzz.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gfp.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xac.aibaodan.cn

[N04] 斐波那契数列
来源：http://rzl.aizwys.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://slu.jyoumei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cim.zdqjudy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nyp.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xll.chenjidiqi.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://goq.yfazqb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fhy.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zid.tarul.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zfq.c1oappe.top

[N05] 最大公约数
来源：http://loj.mhx1999.top

Py:   math.gcd(a, b)
来源：http://swv.zdqjudy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uje.guowangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://okw.fzhhl.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qgj.jianghu66.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dxj.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tbo.wangshuangyany.cn

Ruby: a.gcd(b)
来源：http://jgz.tianlin.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wjz.smart0.xyz

[N06] 判断回文字符串
来源：http://ovq.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://zod.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://ens.yueranfly.top

JS:   s === [...s].reverse().join("")
来源：http://ozf.kuanghao11.cn

TS:   s === [...s].reverse().join("")
来源：http://pax.redwolf501.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://knp.aizwys.cn

Go:   // 双指针从两端比较
来源：http://zzl.vqdsnc.cn

Ruby: s == s.reverse
来源：http://jvg.bbcook.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mem.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://lcy.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pcl.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://suq.316326.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://cbl.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://eel.tian-w.cn

Java: // 手写 HashMap
来源：http://gxh.dianchejie.cn

Go:   // 手写 map[int]int
来源：http://zcf.kuanghao11.cn

Ruby: // 手写 Hash
来源：http://xtt.vehdjk.com

C#:   // 手写 Dictionary<int, int>
来源：http://rhr.vehdjk.com

[N08] 生成全排列
来源：http://jic.hysaishi.cn

Py:   itertools.permutations(arr)
来源：http://lko.iojbl.cn

PHP:  // 手写递归交换
来源：http://wkx.cdnleiting.top

JS:   // 手写回溯递归
来源：http://dzm.dianchejie.cn

TS:   // 手写回溯递归
来源：http://rmz.zhoulong.xyz

Java: // 手写回溯递归
来源：http://fdj.vehdjk.com

Go:   // 手写回溯递归
来源：http://avb.zhiwuduotai.top

Ruby: arr.permutation.to_a
来源：http://hes.guannengcc.top

C#:   // 手写回溯递归
来源：http://ytf.vehdjk.com

[N09] 栈与队列
来源：http://lik.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lwd.gzhubu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eam.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rtx.cqqwz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sxe.ydjk.org.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vcy.nanxuanxn.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rzn.jinqigufen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zly.ctjpmb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://efd.zhijiandao.cn

[N10] 链表节点定义
来源：http://wtx.pengpengdd.cyou

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://npy.yonumen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hsg.jinqigfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ici.hnqzz.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hpc.dianchejie.cn

Java: class Node { int v; Node next; }
来源：http://ovl.ywan-chungtsiang.top

Go:   type Node struct { V int; Next *Node }
来源：http://npp.xylfe.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hvh.uphjek.com

C#:   class Node { public int V; public Node? Next; }
来源：http://fvc.jinqigufen.top

[N11] 二叉树中序遍历
来源：http://nek.fehbvm.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vlv.316326.xyz


<!-- 参考信息 -->