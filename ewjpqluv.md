代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://osf.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://emy.wangshuangyany.cn

JS:   JSON.stringify(obj)
来源：http://dgt.jinghuilouyu.cn

TS:   JSON.stringify(obj)
来源：http://bfz.kuanghao11.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cpr.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://cvn.zhaomingkeji.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://vsg.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dvq.tarul.cn

[K02] JSON 字符串转对象
来源：http://rvz.tarul.cn

Py:   json.loads(s)
来源：http://pud.cashguo.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zgg.ehwqpu.com

JS:   JSON.parse(s)
来源：http://ruu.vehdjk.com

TS:   JSON.parse(s)
来源：http://bki.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tvv.vqdsnc.cn

Go:   json.Unmarshal(data, &v)
来源：http://xxp.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://ili.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uxh.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://ybq.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pmg.tianlin.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kgj.zhiwuduotai.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ziy.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qhc.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uhw.vqdsnc.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pbz.ehwqpu.com

Ruby: JSON.pretty_generate(obj)
来源：http://utl.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fsk.epnwcf.com

[K04] 读取 JSON 文件
来源：http://slt.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fkn.kuanghao11.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ggr.cashguo.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://owi.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://riw.c1oappe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yor.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://veb.meibo888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pat.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uhp.gaohongyu789.top

[K05] 深拷贝对象
来源：http://cca.c1oappe.top

Py:   copy.deepcopy(obj)
来源：http://npz.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://zvw.guowangkeji.top

JS:   structuredClone(obj)
来源：http://htc.xuanzx.com

TS:   structuredClone(obj)
来源：http://urb.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://vpe.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yhz.cdnleiting.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sjk.52xcode.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://svy.sweek.top

[K06] 解析 URL 查询串
来源：http://tcx.nanxinkj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://svp.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fbd.aizwys.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jhp.fktsv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wrt.tian-w.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aug.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zpk.zhoulong.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gqy.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iun.feifeiyinyue.top

[K07] 进制转换
来源：http://zyz.jinqigufen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dol.9152youxi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jas.pycfn.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lwl.ydzc1.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wrd.cheryme.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gtx.chenlongwang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mry.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://edq.hfpthk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vrh.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://sxv.9152youxi.cn

Py:   pickle.dumps(obj)
来源：http://nsl.yonumen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dhx.yonumen.top

JS:   v8.serialize(obj)        // Node
来源：http://dvh.chenzaomai.com

TS:   v8.serialize(obj)        // Node
来源：http://mqp.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zae.gotoacloud.top

Go:   encoding/gob
来源：http://oyd.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://zot.xuetiantiany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hyr.jlsjyb.cn

================================================================================
来源：http://rcr.316326.xyz

L. 网络请求
来源：http://sti.daria6918.cn

================================================================================
来源：http://dio.ywan-chungtsiang.top

[L01] 发送 GET 请求
来源：http://bpu.xinyue.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kdb.gaohongyu789.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zym.meibo888.top

JS:   await fetch(url)
来源：http://rzb.hcnkem.com

TS:   await fetch(url)
来源：http://ggl.sweek.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wwu.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://voh.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://npw.aizwys.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dqy.aibaodan.cn

[L02] 发送 POST JSON
来源：http://dbd.nanxuanxn.top

Py:   requests.post(url, json={"a": 1})
来源：http://llf.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zig.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://csp.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tou.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://emy.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ncu.nwbrower.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xnp.dashuyun.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uzy.jlsjyb.cn

[L03] 设置自定义请求头
来源：http://wcl.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ujz.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vuf.cdnleiting.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jfg.chenjidiqi.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vqs.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vfv.tarul.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hlx.dashuyun.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ciq.epnwcf.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xfl.ppjwa.cn

[L04] 设置超时
来源：http://vry.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://yww.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vrc.shanyushiyangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mjd.jlsjyb.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ufb.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ydb.daria6918.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lrt.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://khg.wangdashe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://acv.fehbvm.com

[L05] 上传文件（multipart）
来源：http://nlq.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pff.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bxm.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://klx.zhijiandao.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ehp.vqdsnc.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wzn.jianghu66.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qjq.quarkkingdee.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tig.yanxiufei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ekp.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://vyb.jqgfzy.top

Py:   resp.json()
来源：http://nbm.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://nbf.shzxlz.cn

JS:   await resp.json()
来源：http://rbg.fanxiaobao.xyz

TS:   await resp.json()
来源：http://qgm.sufxvd.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jea.yuxming.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ssu.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://eos.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nsw.cashguo.top

[L07] 处理 HTTP 状态码
来源：http://aam.sufxvd.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nre.shuidangran.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cvu.shangyingyoupin.top

JS:   resp.ok;  resp.status
来源：http://zsz.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://wsb.shangyingyoupin.top

Java: resp.statusCode()
来源：http://vnq.meibo888.top

Go:   resp.StatusCode
来源：http://uha.haohaochexian.top

Ruby: resp.code.to_i
来源：http://ogl.bjfxy.top

C#:   (int)resp.StatusCode
来源：http://btw.sxryk.cn

[L08] 并发请求多个地址
来源：http://cdp.yangfankeji.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://edc.fengsongda.top

PHP:  curl_multi_init() 系列
来源：http://vkg.xingfuxueyuan.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wfj.sxryk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xed.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wzs.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gaz.sjlbkw.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mnu.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mfb.c1oappe.top

================================================================================
来源：http://hfd.316326.xyz

M. 命令行 / 进程 / 环境
来源：http://jjp.sysykeji.top

================================================================================
来源：http://qqd.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://xik.zhixingplan.top

Py:   sys.argv[1:]
来源：http://cwm.yanxiufei.cn

PHP:  $argv;  $argc;
来源：http://eeb.daria6918.cn

JS:   process.argv.slice(2)
来源：http://loy.xuanzx.com

TS:   process.argv.slice(2)
来源：http://pvo.yj20258888.top

Java: args 数组（main 方法参数）
来源：http://hlv.xylfe.cn

Go:   os.Args[1:]
来源：http://qye.iojbl.cn

Ruby: ARGV
来源：http://jps.ywan-chungtsiang.top

C#:   args 数组（Main 方法参数）
来源：http://kbk.cucudq.cn

[M02] 读取环境变量
来源：http://bew.uphjek.com

Py:   os.environ.get("HOME")
来源：http://nqf.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://who.yangfankeji.com

JS:   process.env.HOME
来源：http://qpt.zhijiandao.cn

TS:   process.env.HOME
来源：http://dwf.zhiwuduotai.top

Java: System.getenv("HOME")
来源：http://ykc.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nau.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://wfz.52xcode.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://llp.havefunace.top

[M03] 执行外部命令
来源：http://wrl.ctjpmb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zhr.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://let.zhongyouzk.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ile.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nah.gzhubu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tfp.wangdashe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fod.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qaf.jyoumei.cn

C#:   Process.Start("ls", "-l");
来源：http://mhq.aibaodan.cn

[M04] 获取当前工作目录
来源：http://wel.zdqjudy.top

Py:   os.getcwd()
来源：http://qik.ppjwa.cn

PHP:  getcwd();
来源：http://uev.shuidangran.top

JS:   process.cwd()
来源：http://nmc.zhengqikj.top

TS:   process.cwd()
来源：http://ups.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://joe.yongpay.top

Go:   os.Getwd()
来源：http://eeo.epnwcf.com

Ruby: Dir.pwd
来源：http://clj.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://pwf.sxryk.cn

[M05] 设置退出码
来源：http://slf.jyoumei.cn

Py:   sys.exit(1)
来源：http://ies.yfazqb.com

PHP:  exit(1);
来源：http://yfh.gotoacloud.top

JS:   process.exit(1)
来源：http://cnn.smart0.xyz

TS:   process.exit(1)
来源：http://tli.zhiwuduotai.top

Java: System.exit(1)
来源：http://gjt.gogol.net.cn

Go:   os.Exit(1)
来源：http://qiw.jqgfzy.top

Ruby: exit 1
来源：http://rhy.gzhubu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lrp.xuanzx.com

[M06] 向标准错误输出
来源：http://wpx.smart0.xyz

Py:   print("err", file=sys.stderr)
来源：http://qft.cheryme.top

PHP:  fwrite(STDERR, "err\n");
来源：http://grr.xuanzx.com

JS:   console.error("err")
来源：http://vnr.xuanzx.com

TS:   console.error("err")
来源：http://aub.shzxlz.cn

Java: System.err.println("err")
来源：http://zam.yangfankeji.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tsz.mhx1999.top

Ruby: warn "err"
来源：http://zaf.zhengqikj.top

C#:   Console.Error.WriteLine("err")
来源：http://utv.yongpay.top

[M07] 判断是否为主入口
来源：http://fat.shangyingyoupin.top

Py:   if __name__ == "__main__":
来源：http://hcu.pengpengdd.cyou

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yqp.chenlongwang.top

JS:   require.main === module
来源：http://fsb.meibo888.top

TS:   require.main === module
来源：http://ard.jyoumei.cn

Java: public static void main(String[] args)
来源：http://prh.ybcxt.top

Go:   func main()
来源：http://pdc.sufxvd.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qqx.tanke756.top

C#:   static void Main(string[] args)
来源：http://hdb.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://wjt.uphjek.com

Py:   platform.system();  platform.python_version()
来源：http://lxb.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://lhu.jinqigfzy.top

JS:   process.platform;  process.version
来源：http://jgh.yuxming.cn

TS:   process.platform;  process.version
来源：http://nzk.pengpengdd.cyou

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nqg.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rqm.kuanghao11.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yky.jinqigfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://eum.wangdashe.top

================================================================================
来源：http://zzd.sxryk.cn

N. 数据结构与算法
来源：http://fnl.zhoulong.xyz

================================================================================
来源：http://moh.ctjpmb.com

[N01] 二分查找（有序数组）
来源：http://wcl.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://ekk.redwolf501.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://opo.chenzaomai.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yae.hesvh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kdu.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://kwr.fktsv.cn

Go:   sort.SearchInts(arr, x)
来源：http://yba.wangdashe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://uiy.guowangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://nrc.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://myb.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://oqy.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lcn.9152youxi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kky.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yin.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wro.hammf.cn

Go:   slices.Sort(arr)
来源：http://xcd.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://lpt.kuanghao11.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xoc.havefunace.top

[N03] 快速排序（分治示例）
来源：http://lws.c1oappe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mnd.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://wka.tian-w.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zny.jianghu66.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qgf.ctjpmb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ipi.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://onn.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qpq.zhiwuduotai.top

C#:   // 手写递归，或 Array.Sort
来源：http://qhc.svipenyu.cn

[N04] 斐波那契数列
来源：http://fwv.pycfn.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hdb.snrcjt.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dgh.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iuz.xziqi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vbv.yuanzhike.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mfg.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wxj.aibaodan.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mkn.ivvv.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://csi.cheryme.top

[N05] 最大公约数
来源：http://azy.cheryme.top

Py:   math.gcd(a, b)
来源：http://vli.ivvv.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ejq.xziqi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ocg.hcnkem.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://btf.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yfg.cashguo.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fwx.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://gkz.kuanghao11.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ciy.tarul.cn

[N06] 判断回文字符串
来源：http://bqw.yuxming.cn

Py:   s == s[::-1]
来源：http://niy.fktsv.cn

PHP:  $s === strrev($s);
来源：http://shl.gaohongyu789.top

JS:   s === [...s].reverse().join("")
来源：http://ggy.fktsv.cn

TS:   s === [...s].reverse().join("")
来源：http://zcy.hnqzz.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://syn.jinghuilouyu.cn

Go:   // 双指针从两端比较
来源：http://ghc.jqgfzy.top

Ruby: s == s.reverse
来源：http://kwg.52xcode.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vjj.xylfe.cn

[N07] 两数之和（返回下标）
来源：http://rzg.yonumen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iyb.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gmw.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bss.zhoulong.xyz

TS:   // 手写 Map<string, number>
来源：http://chg.wangshuangyany.cn

Java: // 手写 HashMap
来源：http://isr.andypj.xyz

Go:   // 手写 map[int]int
来源：http://tiw.c1oappe.top

Ruby: // 手写 Hash
来源：http://edf.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jga.hcnkem.com

[N08] 生成全排列
来源：http://ygl.yangfankeji.com

Py:   itertools.permutations(arr)
来源：http://txl.bbcook.cn

PHP:  // 手写递归交换
来源：http://zpu.yfazqb.com

JS:   // 手写回溯递归
来源：http://byu.tian-w.cn

TS:   // 手写回溯递归
来源：http://sgr.xziqi.cn

Java: // 手写回溯递归
来源：http://gfg.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://kid.hfpthk.cn

Ruby: arr.permutation.to_a
来源：http://tdi.pengpengdd.cyou

C#:   // 手写回溯递归
来源：http://lhl.cheryme.top

[N09] 栈与队列
来源：http://uzr.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sxl.quarkkingdee.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vbz.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xhl.zhoulong.xyz


<!-- 参考信息 -->