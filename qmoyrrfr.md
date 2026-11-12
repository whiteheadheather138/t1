代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://tuy.yonumen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dpn.nwbrower.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://got.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gru.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://spl.yj202588.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://skq.yuxming.cn

[K04] 读取 JSON 文件
来源：http://jyq.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://utd.xuetiantiany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://joi.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ipd.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xei.chenjidiqi.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mfw.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vhp.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://tue.uphjek.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qqe.ivvv.top

[K05] 深拷贝对象
来源：http://ven.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://cub.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://yjt.bbcook.cn

JS:   structuredClone(obj)
来源：http://mcc.smart0.xyz

TS:   structuredClone(obj)
来源：http://sig.c1oappe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://seq.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oxu.yj202588.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://esw.tarul.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gra.cucudq.cn

[K06] 解析 URL 查询串
来源：http://ohd.yvedp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wig.jqgfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://slm.hywenlv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vqc.ctjpmb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ssh.yvedp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qzk.sjlbkw.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nha.cashguo.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pop.c1oappe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dio.hfpthk.cn

[K07] 进制转换
来源：http://qda.cucudq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://knc.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oct.hysaishi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jru.uphjek.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://npx.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dqc.yj20258888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zbl.cucudq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xri.yonumen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eun.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://gek.guowangkeji.top

Py:   pickle.dumps(obj)
来源：http://pvz.yvedp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gxr.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://ros.birdmap.top

TS:   v8.serialize(obj)        // Node
来源：http://zlm.yongpay.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wgd.fanxiaobao.xyz

Go:   encoding/gob
来源：http://tcc.wangshuangyany.cn

Ruby: Marshal.dump(obj)
来源：http://utr.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rgu.jinqigfzy.top

================================================================================
来源：http://lqc.daria6918.cn

L. 网络请求
来源：http://nft.mhx1999.top

================================================================================
来源：http://rsh.smart0.xyz

[L01] 发送 GET 请求
来源：http://phe.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ttr.chenlongwang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tjv.daria6918.cn

JS:   await fetch(url)
来源：http://tgr.chenlongwang.top

TS:   await fetch(url)
来源：http://urv.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xfj.tianlin.xyz

Go:   resp, err := http.Get(url)
来源：http://fno.52xcode.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hiv.jiagoushi.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oap.aibaodan.cn

[L02] 发送 POST JSON
来源：http://ozn.uphjek.com

Py:   requests.post(url, json={"a": 1})
来源：http://oox.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oro.tianlin.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wmq.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kvb.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://llu.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://day.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ish.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dxq.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://wye.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fvm.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://crg.andypj.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wge.aizwys.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uis.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nhk.fktsv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iiu.tarul.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wmw.ehwqpu.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rzy.yj20258.top

[L04] 设置超时
来源：http://ocr.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://ggm.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kxy.sufxvd.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nyk.jinqigufen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ljy.iojbl.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lgg.cashguo.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://afg.jianghu66.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ccw.hnqzz.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cfy.yuxming.cn

[L05] 上传文件（multipart）
来源：http://iti.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://txj.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bka.hfpthk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yht.jqgfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wrv.zhijiandao.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ctd.ydjk.org.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aal.ivvv.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://amd.havefunace.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://alp.cucudq.cn

[L06] 解析响应为 JSON
来源：http://jeo.hnxiangtu.top

Py:   resp.json()
来源：http://zac.haohaochexian.top

PHP:  json_decode($body, true);
来源：http://jak.aizwys.cn

JS:   await resp.json()
来源：http://dfg.birdmap.top

TS:   await resp.json()
来源：http://zxh.9152youxi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pkk.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://njf.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://zdo.hammf.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lbb.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://vwz.sxryk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cng.xinyue.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vwq.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://suc.quarkkingdee.top

TS:   resp.ok;  resp.status
来源：http://sgf.hysaishi.cn

Java: resp.statusCode()
来源：http://fbr.0kj1m.cn

Go:   resp.StatusCode
来源：http://bke.zhiwuduotai.top

Ruby: resp.code.to_i
来源：http://acu.ybcxt.top

C#:   (int)resp.StatusCode
来源：http://yfh.fzhhl.top

[L08] 并发请求多个地址
来源：http://zkp.gogol.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mha.mhx1999.top

PHP:  curl_multi_init() 系列
来源：http://wij.vqdsnc.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hkx.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hts.shuidangran.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ate.cqqwz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sfe.zhoulong.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vml.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bbv.chenlongwang.top

================================================================================
来源：http://cip.jqgfzy.top

M. 命令行 / 进程 / 环境
来源：http://mip.uphjek.com

================================================================================
来源：http://nxp.chenlongwang.top

[M01] 读取命令行参数
来源：http://iaf.shanyushiyangtech.top

Py:   sys.argv[1:]
来源：http://baj.nanxuanxn.top

PHP:  $argv;  $argc;
来源：http://qjy.wangshuangyany.cn

JS:   process.argv.slice(2)
来源：http://spe.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://tzl.zdqjudy.top

Java: args 数组（main 方法参数）
来源：http://elq.9152youxi.cn

Go:   os.Args[1:]
来源：http://zql.aizwys.cn

Ruby: ARGV
来源：http://ibu.xylfe.cn

C#:   args 数组（Main 方法参数）
来源：http://rnf.bjfxy.top

[M02] 读取环境变量
来源：http://fxk.yuxming.cn

Py:   os.environ.get("HOME")
来源：http://rfe.dashuyun.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mlg.cdnleiting.top

JS:   process.env.HOME
来源：http://lbp.havefunace.top

TS:   process.env.HOME
来源：http://sjl.yuxming.cn

Java: System.getenv("HOME")
来源：http://ais.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vyx.ydjk.org.cn

Ruby: ENV["HOME"]
来源：http://hdr.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rox.zhongyouzk.top

[M03] 执行外部命令
来源：http://vur.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hip.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ttv.sufxvd.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vrm.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yek.jinqigufen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gao.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lbv.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://cjv.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://wbl.yangfankeji.com

[M04] 获取当前工作目录
来源：http://aeg.zycfv.cn

Py:   os.getcwd()
来源：http://bjb.svipenyu.cn

PHP:  getcwd();
来源：http://uhp.ybcxt.top

JS:   process.cwd()
来源：http://xrq.zdbjq.cn

TS:   process.cwd()
来源：http://bia.ybcxt.top

Java: Path.of("").toAbsolutePath()
来源：http://rvg.ydzc1.top

Go:   os.Getwd()
来源：http://nqg.316326.xyz

Ruby: Dir.pwd
来源：http://izy.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://mgx.jianghu66.top

[M05] 设置退出码
来源：http://unr.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://ddh.nanxuanxn.top

PHP:  exit(1);
来源：http://fad.yanxiufei.cn

JS:   process.exit(1)
来源：http://qeq.sysykeji.top

TS:   process.exit(1)
来源：http://yol.nanxuanxn.top

Java: System.exit(1)
来源：http://bif.9152youxi.cn

Go:   os.Exit(1)
来源：http://gil.yj20258888.top

Ruby: exit 1
来源：http://tcm.vehdjk.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://buq.yonumen.top

[M06] 向标准错误输出
来源：http://wjg.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://wdp.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://znz.dashuyun.cn

JS:   console.error("err")
来源：http://jmw.ywan-chungtsiang.top

TS:   console.error("err")
来源：http://emb.feifeiyinyue.top

Java: System.err.println("err")
来源：http://dob.cucudq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nsk.tarul.cn

Ruby: warn "err"
来源：http://izn.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://jur.yonumen.top

[M07] 判断是否为主入口
来源：http://cwj.cdnleiting.top

Py:   if __name__ == "__main__":
来源：http://bpe.tarul.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uuo.c1oappe.top

JS:   require.main === module
来源：http://zff.yangfankeji.com

TS:   require.main === module
来源：http://fge.dashuyun.cn

Java: public static void main(String[] args)
来源：http://kpj.meibo888.top

Go:   func main()
来源：http://omd.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fse.hcnkem.com

C#:   static void Main(string[] args)
来源：http://qkf.jinqigufen.top

[M08] 获取系统与运行时信息
来源：http://mcz.jinqigufen.top

Py:   platform.system();  platform.python_version()
来源：http://sri.xingfuxueyuan.xyz

PHP:  PHP_OS;  phpversion();
来源：http://rrm.pycfn.com

JS:   process.platform;  process.version
来源：http://onf.fanxiaobao.xyz

TS:   process.platform;  process.version
来源：http://dof.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ghq.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lnx.redwolf501.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ygv.andypj.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://hmr.sufxvd.cn

================================================================================
来源：http://ekm.sjlbkw.cn

N. 数据结构与算法
来源：http://oem.xylfe.cn

================================================================================
来源：http://blf.sjlbkw.cn

[N01] 二分查找（有序数组）
来源：http://pcm.jiagoushi.top

Py:   bisect.bisect_left(arr, x)
来源：http://wmy.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pzc.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://voi.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pbw.fengsongda.top

Java: Arrays.binarySearch(arr, x)
来源：http://emc.jinqigfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://gcj.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://iql.haohaochexian.top

C#:   Array.BinarySearch(arr, x)
来源：http://mww.tarul.cn

[N02] 排序（工程实践用内置实现）
来源：http://frx.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://xju.zhengqikj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yux.shuidangran.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lip.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vrr.cheryme.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mwd.316326.xyz

Go:   slices.Sort(arr)
来源：http://qda.xuanzx.com

Ruby: arr.sort
来源：http://zas.jqgufenzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hme.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://pfy.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tql.kuanghao11.cn

PHP:  // 递归实现，或用 usort
来源：http://lob.shanyushiyangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aqi.fanxiaobao.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ztg.jinyuanbaomall.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mor.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yrx.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://osv.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xvc.yangfankeji.com

[N04] 斐波那契数列
来源：http://zlf.zhixingplan.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://srg.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kdx.jinghuilouyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nit.gaohongyu789.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pva.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gzo.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jfw.dianchejie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kkb.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://riq.gaohongyu789.top

[N05] 最大公约数
来源：http://jta.c1oappe.top

Py:   math.gcd(a, b)
来源：http://rgd.chenjidiqi.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ouy.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ggy.wangshuangyany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nqc.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ywq.mhx1999.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://edw.hongshengwenyu.top

Ruby: a.gcd(b)
来源：http://yvr.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fly.cucudq.cn

[N06] 判断回文字符串
来源：http://oln.yangfankeji.com

Py:   s == s[::-1]
来源：http://seg.pycfn.com

PHP:  $s === strrev($s);
来源：http://dgg.haohaochexian.top

JS:   s === [...s].reverse().join("")
来源：http://hcn.sxryk.cn

TS:   s === [...s].reverse().join("")
来源：http://zpq.c1oappe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uzo.fzhhl.top

Go:   // 双指针从两端比较
来源：http://egk.hnqzz.top

Ruby: s == s.reverse
来源：http://kym.cqqwz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ibe.jqgfzy.top

[N07] 两数之和（返回下标）
来源：http://dsv.xuanzx.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cre.sufxvd.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vdl.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rvt.zhijiandao.cn

TS:   // 手写 Map<string, number>
来源：http://tsy.sweek.top

Java: // 手写 HashMap
来源：http://xml.shzxlz.cn

Go:   // 手写 map[int]int
来源：http://pro.yanxiufei.cn

Ruby: // 手写 Hash
来源：http://wrc.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ccw.yueranfly.top

[N08] 生成全排列
来源：http://xpi.hnxiangtu.top

Py:   itertools.permutations(arr)
来源：http://ihj.chenlongwang.top

PHP:  // 手写递归交换
来源：http://otl.jinqigfzy.top

JS:   // 手写回溯递归
来源：http://ooo.zhixingplan.top

TS:   // 手写回溯递归
来源：http://mfq.chenlongwang.top

Java: // 手写回溯递归
来源：http://qsz.sxryk.cn

Go:   // 手写回溯递归
来源：http://xaf.kuanghao11.cn

Ruby: arr.permutation.to_a
来源：http://zrl.xingfuxueyuan.xyz

C#:   // 手写回溯递归
来源：http://qiz.zhiwuduotai.top

[N09] 栈与队列
来源：http://ssw.gotoacloud.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wqq.hywenlv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zlv.redwolf501.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gjo.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cia.yfazqb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wlj.xuetiantiany.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://inq.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wrn.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mhx.smart0.xyz

[N10] 链表节点定义
来源：http://brb.gotoacloud.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fib.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://rgu.ppjwa.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xni.jianghu66.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xdo.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://bkr.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://wvv.haohaochexian.top

Ruby: Node = Struct.new(:v, :next)
来源：http://fff.pengpengdd.cyou

C#:   class Node { public int V; public Node? Next; }
来源：http://ajq.sweek.top

[N11] 二叉树中序遍历
来源：http://nmf.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ctu.yj20258888.top

PHP:  // 手写递归函数
来源：http://mbn.yvedp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rhi.nanxuanxn.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ets.zhongyouzk.top

Java: // 手写递归
来源：http://jak.zhiwuduotai.top


<!-- 参考信息 -->