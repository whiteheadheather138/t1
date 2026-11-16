代发 wailian999

TS:   JSON.parse(s)
来源：http://duk.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jdh.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://pyy.shuidangran.top

Ruby: JSON.parse(s)
来源：http://ivb.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wax.shanyushiyangtech.top

[K03] JSON 美化输出（带缩进）
来源：http://mxj.fanxiaobao.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gqv.jyoumei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://clh.yj202588.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jrg.fehbvm.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ayo.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wjy.birdmap.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://brx.fktsv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bhb.dashuyun.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://njl.shangyingyoupin.top

[K04] 读取 JSON 文件
来源：http://nyz.smart0.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wze.mhx1999.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://icw.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rcj.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hjg.xinyue.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bqo.shzxlz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jdr.shanyushiyangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xbt.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ese.iojbl.cn

[K05] 深拷贝对象
来源：http://git.jinghuilouyu.cn

Py:   copy.deepcopy(obj)
来源：http://tbj.yvedp.cn

PHP:  unserialize(serialize($obj));
来源：http://qkk.tarul.cn

JS:   structuredClone(obj)
来源：http://bqs.zhengqikj.top

TS:   structuredClone(obj)
来源：http://yrt.ywan-chungtsiang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jmd.sysykeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zjn.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bnb.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://jyk.sysykeji.top

[K06] 解析 URL 查询串
来源：http://lyp.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ata.jinqigufen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kln.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qfv.feifeiyinyue.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://maz.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ref.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mtk.quarkkingdee.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://adb.fehbvm.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mgj.cheryme.top

[K07] 进制转换
来源：http://vur.hammf.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nmm.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pna.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fzk.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ghc.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://axj.nwbrower.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kkk.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hmd.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jjh.zhongyouzk.top

[K08] 二进制序列化（非 JSON）
来源：http://xye.shanyushiyangtech.top

Py:   pickle.dumps(obj)
来源：http://brg.shanyushiyangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ymt.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://lau.hnxiangtu.top

TS:   v8.serialize(obj)        // Node
来源：http://uwt.tanke756.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://apu.cheryme.top

Go:   encoding/gob
来源：http://ifx.jinqigufen.top

Ruby: Marshal.dump(obj)
来源：http://vyf.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cbp.52xcode.cn

================================================================================
来源：http://fko.nwbrower.top

L. 网络请求
来源：http://qek.jinqigufen.top

================================================================================
来源：http://huc.cqqwz.cn

[L01] 发送 GET 请求
来源：http://xnh.xinyue.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ndh.tanke756.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hpg.sweek.top

JS:   await fetch(url)
来源：http://pda.yuxming.cn

TS:   await fetch(url)
来源：http://asz.fanxiaobao.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tzh.hnxiangtu.top

Go:   resp, err := http.Get(url)
来源：http://txf.shuidangran.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vwi.jlsjyb.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pmv.zhijiandao.cn

[L02] 发送 POST JSON
来源：http://rlo.yj202588.top

Py:   requests.post(url, json={"a": 1})
来源：http://csc.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oau.wangdashe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://khh.yuxming.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wgy.sweek.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eyl.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wiw.xuetiantiany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kox.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nxg.cucudq.cn

[L03] 设置自定义请求头
来源：http://gfl.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://igt.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ycz.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gly.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zat.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hba.yangfankeji.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lba.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vty.feifeiyinyue.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wcn.fktsv.cn

[L04] 设置超时
来源：http://vmp.316326.xyz

Py:   requests.get(url, timeout=5)
来源：http://wah.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dea.xuanzx.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xdd.zycfv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jje.vehdjk.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qze.nanxinkj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://utq.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uwr.tian-w.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iay.wangshuangyany.cn

[L05] 上传文件（multipart）
来源：http://zbl.zycfv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://znl.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hni.zhixingplan.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://emm.feifeiyinyue.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cgy.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xya.ehwqpu.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fav.yonumen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rkl.yuxming.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xha.daxiang520.top

[L06] 解析响应为 JSON
来源：http://vzt.zdqjudy.top

Py:   resp.json()
来源：http://wcw.daxiang520.top

PHP:  json_decode($body, true);
来源：http://vat.ydjk.org.cn

JS:   await resp.json()
来源：http://bub.zhongyouzk.top

TS:   await resp.json()
来源：http://tza.yongpay.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://grt.zhixingplan.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cod.ydzc1.top

Ruby: JSON.parse(resp.body)
来源：http://myx.hnxiangtu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vuv.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://iqf.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fwj.fanxiaobao.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zmg.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://hfn.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://amg.nwbrower.top

Java: resp.statusCode()
来源：http://dec.chenlongwang.top

Go:   resp.StatusCode
来源：http://exk.pycfn.com

Ruby: resp.code.to_i
来源：http://ezn.tianlin.xyz

C#:   (int)resp.StatusCode
来源：http://ntx.xuetiantiany.cn

[L08] 并发请求多个地址
来源：http://rcq.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://etf.mhx1999.top

PHP:  curl_multi_init() 系列
来源：http://fbv.yanxiufei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uca.xinyue.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pca.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cho.yongpay.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rne.xingfuxueyuan.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ccd.xuanzx.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vqc.yfazqb.com

================================================================================
来源：http://kln.haohaochexian.top

M. 命令行 / 进程 / 环境
来源：http://rzo.wangshuangyany.cn

================================================================================
来源：http://vjd.shanyushiyangtech.top

[M01] 读取命令行参数
来源：http://mss.vehdjk.com

Py:   sys.argv[1:]
来源：http://blm.fktsv.cn

PHP:  $argv;  $argc;
来源：http://gmw.sxryk.cn

JS:   process.argv.slice(2)
来源：http://csu.zhixingplan.top

TS:   process.argv.slice(2)
来源：http://ddu.jinqigufen.top

Java: args 数组（main 方法参数）
来源：http://uty.52xcode.cn

Go:   os.Args[1:]
来源：http://iet.ehwqpu.com

Ruby: ARGV
来源：http://hri.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://ubh.vehdjk.com

[M02] 读取环境变量
来源：http://dsz.dashuyun.cn

Py:   os.environ.get("HOME")
来源：http://qbn.epnwcf.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iux.aizwys.cn

JS:   process.env.HOME
来源：http://vjf.redwolf501.top

TS:   process.env.HOME
来源：http://dyb.fanxiaobao.xyz

Java: System.getenv("HOME")
来源：http://ocp.wangdashe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bjt.fehbvm.com

Ruby: ENV["HOME"]
来源：http://prq.birdmap.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dmv.sweek.top

[M03] 执行外部命令
来源：http://auk.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ctn.jqgfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xjc.ydzc1.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zge.fehbvm.com

TS:   child_process.execSync("ls -l").toString()
来源：http://ptj.nwbrower.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zaz.jinqigfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lyz.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wop.gaohongyu789.top

C#:   Process.Start("ls", "-l");
来源：http://xxf.xuanzx.com

[M04] 获取当前工作目录
来源：http://lqk.kuanghao11.cn

Py:   os.getcwd()
来源：http://fvg.birdmap.top

PHP:  getcwd();
来源：http://kgr.52xcode.cn

JS:   process.cwd()
来源：http://jul.wangdashe.top

TS:   process.cwd()
来源：http://iaq.kuanghao11.cn

Java: Path.of("").toAbsolutePath()
来源：http://sxc.andypj.xyz

Go:   os.Getwd()
来源：http://atr.yonumen.top

Ruby: Dir.pwd
来源：http://pmu.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://hvr.ywan-chungtsiang.top

[M05] 设置退出码
来源：http://oaa.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://aiz.guowangkeji.top

PHP:  exit(1);
来源：http://ulw.ivvv.top

JS:   process.exit(1)
来源：http://zmk.shanyushiyangkeji.top

TS:   process.exit(1)
来源：http://tfk.tanke756.top

Java: System.exit(1)
来源：http://hpy.yueranfly.top

Go:   os.Exit(1)
来源：http://rgc.tanke756.top

Ruby: exit 1
来源：http://kkj.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rbc.9152youxi.cn

[M06] 向标准错误输出
来源：http://ltb.zdqjudy.top

Py:   print("err", file=sys.stderr)
来源：http://bxl.yj20258888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qse.yongpay.top

JS:   console.error("err")
来源：http://faj.yonumen.top

TS:   console.error("err")
来源：http://dml.tian-w.cn

Java: System.err.println("err")
来源：http://tcv.yonumen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yna.yangfankeji.com

Ruby: warn "err"
来源：http://aix.shanyushiyangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://bsw.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://rim.haohaochexian.top

Py:   if __name__ == "__main__":
来源：http://nbx.cqqwz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qpv.yvedp.cn

JS:   require.main === module
来源：http://dqp.jinghuilouyu.cn

TS:   require.main === module
来源：http://zue.zdbjq.cn

Java: public static void main(String[] args)
来源：http://kws.xinyue.icu

Go:   func main()
来源：http://eha.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lyv.zhiwuduotai.top

C#:   static void Main(string[] args)
来源：http://lze.cheryme.top

[M08] 获取系统与运行时信息
来源：http://pop.hammf.cn

Py:   platform.system();  platform.python_version()
来源：http://otx.chenjidiqi.icu

PHP:  PHP_OS;  phpversion();
来源：http://sti.ydzc1.top

JS:   process.platform;  process.version
来源：http://dni.haohaochexian.top

TS:   process.platform;  process.version
来源：http://rxw.316326.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lbw.uphjek.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://iam.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hvi.zhijiandao.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yeq.sjlbkw.cn

================================================================================
来源：http://iof.epnwcf.com

N. 数据结构与算法
来源：http://yyg.daria6918.cn

================================================================================
来源：http://rvv.gogol.net.cn

[N01] 二分查找（有序数组）
来源：http://srx.yuxming.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dmt.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hfm.birdmap.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wmv.hnxiangtu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gxk.guowangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://huj.havefunace.top

Go:   sort.SearchInts(arr, x)
来源：http://qgb.haohaochexian.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jgt.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://aar.hywenlv.cn

[N02] 排序（工程实践用内置实现）
来源：http://zrd.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ggg.nwbrower.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qnc.nwbrower.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lag.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ese.mhx1999.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mvv.chenjidiqi.icu

Go:   slices.Sort(arr)
来源：http://yli.zhongyouzk.top

Ruby: arr.sort
来源：http://psj.cdnleiting.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hlp.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://mlv.ydzc1.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zvp.yuxming.cn

PHP:  // 递归实现，或用 usort
来源：http://bru.316326.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dec.wangdashe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rys.ydzc1.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://keg.jinghuilouyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://psc.hywenlv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vss.9152youxi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qmo.kuanghao11.cn

[N04] 斐波那契数列
来源：http://nzq.vehdjk.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lcp.yj20258.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xgi.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fgu.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hni.meibo888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uww.tarul.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tou.wangshuangyany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rbb.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mmw.andypj.xyz

[N05] 最大公约数
来源：http://yiu.guowangkeji.top

Py:   math.gcd(a, b)
来源：http://ypa.ydjk.org.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pod.sweek.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uun.dashuyun.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rdr.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rij.ctjpmb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tot.sjlbkw.cn

Ruby: a.gcd(b)
来源：http://zpf.yonumen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hgi.svipenyu.cn

[N06] 判断回文字符串
来源：http://fzr.jinghuilouyu.cn

Py:   s == s[::-1]
来源：http://cnj.gzhubu.top

PHP:  $s === strrev($s);
来源：http://svd.fengsongda.top

JS:   s === [...s].reverse().join("")
来源：http://las.kuanghao11.cn

TS:   s === [...s].reverse().join("")
来源：http://fee.sufxvd.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://umr.hnxiangtu.top

Go:   // 双指针从两端比较
来源：http://mnh.havefunace.top

Ruby: s == s.reverse
来源：http://qdy.fehbvm.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://aya.hnxiangtu.top

[N07] 两数之和（返回下标）
来源：http://wuz.0kj1m.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xmo.hywenlv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eyx.jqgufenzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yld.aibaodan.cn

TS:   // 手写 Map<string, number>
来源：http://olb.havefunace.top

Java: // 手写 HashMap
来源：http://peg.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://ypw.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://nal.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jhf.dashuyun.cn

[N08] 生成全排列
来源：http://zfi.wangdashe.top

Py:   itertools.permutations(arr)
来源：http://xwh.ybcxt.top

PHP:  // 手写递归交换
来源：http://uhd.shzxlz.cn

JS:   // 手写回溯递归
来源：http://xwb.yj20258888.top

TS:   // 手写回溯递归
来源：http://jag.shanyushiyangtech.top

Java: // 手写回溯递归
来源：http://ati.tanke756.top

Go:   // 手写回溯递归
来源：http://sxz.fanxiaobao.xyz

Ruby: arr.permutation.to_a
来源：http://iih.daxiang520.top

C#:   // 手写回溯递归
来源：http://eqc.dianchejie.cn

[N09] 栈与队列
来源：http://kha.c1oappe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nha.hammf.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yem.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ryj.aibaodan.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kzh.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hex.daria6918.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nyj.xinyue.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wgz.quarkkingdee.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eht.bbcook.cn

[N10] 链表节点定义
来源：http://hcp.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lww.zhongyouzk.top

PHP:  class Node { public $v; public $next = null; }
来源：http://oao.guowangkeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kob.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hln.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://cqe.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://plb.yanxiufei.cn


<!-- 参考信息 -->