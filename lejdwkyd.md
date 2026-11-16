代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iol.fengsongda.top

Go:   json.Marshal(obj)
来源：http://bzl.shangyingyoupin.top

Ruby: obj.to_json                                     // require "json"
来源：http://nup.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://lda.kuanghao11.cn

[K02] JSON 字符串转对象
来源：http://dtq.tanke756.top

Py:   json.loads(s)
来源：http://zeb.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ida.hysaishi.cn

JS:   JSON.parse(s)
来源：http://qdg.jinghuilouyu.cn

TS:   JSON.parse(s)
来源：http://xsi.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rhs.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://whj.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://oyz.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://poj.jlsjyb.cn

[K03] JSON 美化输出（带缩进）
来源：http://fip.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ugm.ctjpmb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://emh.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lhk.zhixingplan.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cjk.jqgufenzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lhq.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://aew.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://rhy.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xdy.sxryk.cn

[K04] 读取 JSON 文件
来源：http://lhq.aizwys.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ahk.zdbjq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xoi.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ygq.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uhf.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lpu.aizwys.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cwz.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ntj.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yrh.shuidangran.top

[K05] 深拷贝对象
来源：http://yqg.dianchejie.cn

Py:   copy.deepcopy(obj)
来源：http://hsg.gzhubu.top

PHP:  unserialize(serialize($obj));
来源：http://wil.shuidangran.top

JS:   structuredClone(obj)
来源：http://maa.hywenlv.cn

TS:   structuredClone(obj)
来源：http://wnj.zhengqikj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mnn.jinqigfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aqi.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nbt.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dpr.zdbjq.cn

[K06] 解析 URL 查询串
来源：http://xwg.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://huz.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://umw.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bkm.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mvs.yonumen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ipp.tianlin.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://obo.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ojp.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hmn.jinqigufen.top

[K07] 进制转换
来源：http://uyr.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oaf.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fow.ehwqpu.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rxb.quarkkingdee.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jtc.chenlongwang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://umz.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zhn.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lkh.snrcjt.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jde.havefunace.top

[K08] 二进制序列化（非 JSON）
来源：http://unt.zdqjudy.top

Py:   pickle.dumps(obj)
来源：http://jjb.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://qgc.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://bhi.cqqwz.cn

TS:   v8.serialize(obj)        // Node
来源：http://egz.shzxlz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mog.meibo888.top

Go:   encoding/gob
来源：http://tyy.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://jdp.nanxuanxn.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ger.jinyuanbaomall.cn

================================================================================
来源：http://udy.zhoulong.xyz

L. 网络请求
来源：http://pzd.nanxinkj.top

================================================================================
来源：http://ker.nanxuanxn.top

[L01] 发送 GET 请求
来源：http://cyc.xinyue.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kis.ydzc1.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aju.jqgfzy.top

JS:   await fetch(url)
来源：http://xvp.yangfankeji.com

TS:   await fetch(url)
来源：http://dhg.jqgufenzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sey.yongpay.top

Go:   resp, err := http.Get(url)
来源：http://tqp.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qax.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gdz.fengsongda.top

[L02] 发送 POST JSON
来源：http://ole.aizwys.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vob.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zca.ctjpmb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://okb.fzhhl.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xdx.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rjh.havefunace.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://clm.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://amj.yonumen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hma.feifeiyinyue.top

[L03] 设置自定义请求头
来源：http://ecp.cdnleiting.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mtn.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ete.fzhhl.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://edd.yangfankeji.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dbu.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://piz.hammf.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vli.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://djx.xingfuxueyuan.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ebu.wangdashe.top

[L04] 设置超时
来源：http://jsq.hywenlv.cn

Py:   requests.get(url, timeout=5)
来源：http://ptn.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wwq.xylfe.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nme.yangfankeji.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xgn.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zpx.jianghu66.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://csg.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zrp.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://prb.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://uro.epnwcf.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bul.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wvz.bbcook.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://imi.fanxiaobao.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rhr.ctjpmb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hrb.316326.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yvo.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ywr.redwolf501.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://myn.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://rbn.sufxvd.cn

Py:   resp.json()
来源：http://six.yuanzhike.top

PHP:  json_decode($body, true);
来源：http://hdk.smart0.xyz

JS:   await resp.json()
来源：http://jie.redwolf501.top

TS:   await resp.json()
来源：http://bjr.jinqigfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uix.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kai.ctjpmb.com

Ruby: JSON.parse(resp.body)
来源：http://stt.yangfankeji.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oxn.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://hyt.zhongyouzk.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qbq.tianlin.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xvd.316326.xyz

JS:   resp.ok;  resp.status
来源：http://dok.shuidangran.top

TS:   resp.ok;  resp.status
来源：http://nwl.bjfxy.top

Java: resp.statusCode()
来源：http://wng.shzxlz.cn

Go:   resp.StatusCode
来源：http://rqz.gogol.net.cn

Ruby: resp.code.to_i
来源：http://agx.9152youxi.cn

C#:   (int)resp.StatusCode
来源：http://bhq.c1oappe.top

[L08] 并发请求多个地址
来源：http://kac.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vkw.havefunace.top

PHP:  curl_multi_init() 系列
来源：http://jew.gaohongyu789.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yor.andypj.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hrz.0kj1m.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gpd.xylfe.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://chk.yueranfly.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://smz.yj20258888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fwm.sxryk.cn

================================================================================
来源：http://lmo.yangfankeji.com

M. 命令行 / 进程 / 环境
来源：http://brg.tanke756.top

================================================================================
来源：http://wxb.quarkkingdee.top

[M01] 读取命令行参数
来源：http://brz.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://eiw.yanxiufei.cn

PHP:  $argv;  $argc;
来源：http://gwj.hcnkem.com

JS:   process.argv.slice(2)
来源：http://jrf.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://ygu.guannengcc.top

Java: args 数组（main 方法参数）
来源：http://yar.meibo888.top

Go:   os.Args[1:]
来源：http://mgb.jinqigfzy.top

Ruby: ARGV
来源：http://wqf.wangdashe.top

C#:   args 数组（Main 方法参数）
来源：http://bgs.pycfn.com

[M02] 读取环境变量
来源：http://uql.yonumen.top

Py:   os.environ.get("HOME")
来源：http://ppd.daxiang520.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vrs.gzhubu.top

JS:   process.env.HOME
来源：http://wjx.chenjidiqi.icu

TS:   process.env.HOME
来源：http://jyz.jinqigfzy.top

Java: System.getenv("HOME")
来源：http://aip.9152youxi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://agf.svipenyu.cn

Ruby: ENV["HOME"]
来源：http://mil.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gvu.zhijiandao.cn

[M03] 执行外部命令
来源：http://xag.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://utt.shanyushiyangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jke.hnxiangtu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ozi.iojbl.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zqw.fanxiaobao.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gji.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jsl.jinyuanbaomall.cn

Ruby: system("ls -l");  `ls -l`
来源：http://unb.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://mof.52xcode.cn

[M04] 获取当前工作目录
来源：http://fyq.aibaodan.cn

Py:   os.getcwd()
来源：http://vax.xylfe.cn

PHP:  getcwd();
来源：http://glf.hesvh.cn

JS:   process.cwd()
来源：http://dkt.zycfv.cn

TS:   process.cwd()
来源：http://wmk.andypj.xyz

Java: Path.of("").toAbsolutePath()
来源：http://joe.jinqigufen.top

Go:   os.Getwd()
来源：http://yxs.snrcjt.cn

Ruby: Dir.pwd
来源：http://mzd.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://ffw.yongpay.top

[M05] 设置退出码
来源：http://zkd.ppjwa.cn

Py:   sys.exit(1)
来源：http://yhn.yanxiufei.cn

PHP:  exit(1);
来源：http://okx.zhijiandao.cn

JS:   process.exit(1)
来源：http://ftw.hcnkem.com

TS:   process.exit(1)
来源：http://xbm.yj202588.top

Java: System.exit(1)
来源：http://tyi.zhongyouzk.top

Go:   os.Exit(1)
来源：http://evr.yj20258.top

Ruby: exit 1
来源：http://sie.cucudq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gne.nanxuanxn.top

[M06] 向标准错误输出
来源：http://pko.jiagoushi.top

Py:   print("err", file=sys.stderr)
来源：http://arv.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oex.aizwys.cn

JS:   console.error("err")
来源：http://xjn.daxiang520.top

TS:   console.error("err")
来源：http://keq.andypj.xyz

Java: System.err.println("err")
来源：http://eoi.sxryk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gxk.fanxiaobao.xyz

Ruby: warn "err"
来源：http://xez.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://cka.andypj.xyz

[M07] 判断是否为主入口
来源：http://xre.9152youxi.cn

Py:   if __name__ == "__main__":
来源：http://tqf.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wdg.zhijiandao.cn

JS:   require.main === module
来源：http://nim.sufxvd.cn

TS:   require.main === module
来源：http://zbe.jiagoushi.top

Java: public static void main(String[] args)
来源：http://jbl.9152youxi.cn

Go:   func main()
来源：http://rwu.meibo888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mpq.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://ijl.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://epg.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://xvg.wangshuangyany.cn

PHP:  PHP_OS;  phpversion();
来源：http://bqy.jiagoushi.top

JS:   process.platform;  process.version
来源：http://znx.sxryk.cn

TS:   process.platform;  process.version
来源：http://sfg.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://grm.andypj.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://zdi.yongpay.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mug.zhiwuduotai.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ark.jqgfzy.top

================================================================================
来源：http://xnr.hesvh.cn

N. 数据结构与算法
来源：http://ifz.gotoacloud.top

================================================================================
来源：http://pic.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://fxf.havefunace.top

Py:   bisect.bisect_left(arr, x)
来源：http://kch.birdmap.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zxp.dianchejie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ckx.shzxlz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lhl.fehbvm.com

Java: Arrays.binarySearch(arr, x)
来源：http://imh.jlsjyb.cn

Go:   sort.SearchInts(arr, x)
来源：http://xgv.tianlin.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://syx.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://qaj.sufxvd.cn

[N02] 排序（工程实践用内置实现）
来源：http://cbf.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://tvg.xylfe.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xei.vqdsnc.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://edx.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://izh.nanxinkj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zco.fktsv.cn

Go:   slices.Sort(arr)
来源：http://rnk.52xcode.cn

Ruby: arr.sort
来源：http://sfz.tian-w.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pmn.mhx1999.top

[N03] 快速排序（分治示例）
来源：http://rtm.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hoe.cqqwz.cn

PHP:  // 递归实现，或用 usort
来源：http://nzd.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://azi.zhiwuduotai.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://isa.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ooo.hysaishi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zcy.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://khq.yfazqb.com

C#:   // 手写递归，或 Array.Sort
来源：http://qys.aibaodan.cn

[N04] 斐波那契数列
来源：http://byc.sweek.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cvk.hysaishi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wko.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qio.hcnkem.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://smw.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lkd.jqgufenzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wrs.bbcook.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iym.tian-w.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yne.jiagoushi.top

[N05] 最大公约数
来源：http://vpg.yonumen.top

Py:   math.gcd(a, b)
来源：http://dug.ivvv.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vwl.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tjx.yvedp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iyw.wangdashe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wfs.yuxming.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tuu.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://awh.mhx1999.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ozf.gogol.net.cn

[N06] 判断回文字符串
来源：http://wvw.9152youxi.cn

Py:   s == s[::-1]
来源：http://eaz.jiagoushi.top

PHP:  $s === strrev($s);
来源：http://lsf.xylfe.cn

JS:   s === [...s].reverse().join("")
来源：http://ggp.shanyushiyangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://cgq.xylfe.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gai.guowangkeji.top

Go:   // 双指针从两端比较
来源：http://owt.gaohongyu789.top

Ruby: s == s.reverse
来源：http://hdh.bjfxy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hzb.sufxvd.cn

[N07] 两数之和（返回下标）
来源：http://pzu.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://unz.nanxinkj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://quv.ydzc1.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xpm.shanyushiyangkeji.top

TS:   // 手写 Map<string, number>
来源：http://klu.ehwqpu.com

Java: // 手写 HashMap
来源：http://gnu.zycfv.cn

Go:   // 手写 map[int]int
来源：http://una.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://mvw.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://wma.xinyue.icu

[N08] 生成全排列
来源：http://qzm.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://iyw.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://cud.zycfv.cn

JS:   // 手写回溯递归
来源：http://xfd.tian-w.cn

TS:   // 手写回溯递归
来源：http://pwv.ybcxt.top

Java: // 手写回溯递归
来源：http://egy.zdqjudy.top

Go:   // 手写回溯递归
来源：http://lpg.xingfuxueyuan.xyz

Ruby: arr.permutation.to_a
来源：http://dhq.daria6918.cn

C#:   // 手写回溯递归
来源：http://tdk.sweek.top

[N09] 栈与队列
来源：http://qhc.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://boz.ppjwa.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rln.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eqg.guannengcc.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vju.sweek.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nwd.jqgfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ozl.xuanzx.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zvl.dashuyun.cn


<!-- 参考信息 -->