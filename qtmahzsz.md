代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://szb.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jrc.wangshuangyany.cn

JS:   JSON.stringify(obj)
来源：http://fey.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://kqi.hnxiangtu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://etf.sjlbkw.cn

Go:   json.Marshal(obj)
来源：http://epr.dashuyun.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rmw.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tjr.yj20258888.top

[K02] JSON 字符串转对象
来源：http://aob.zdqjudy.top

Py:   json.loads(s)
来源：http://qwc.jianghu66.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hbb.cucudq.cn

JS:   JSON.parse(s)
来源：http://vji.chenzaomai.com

TS:   JSON.parse(s)
来源：http://uut.tianlin.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ngy.ctjpmb.com

Go:   json.Unmarshal(data, &v)
来源：http://hmw.hongshengwenyu.top

Ruby: JSON.parse(s)
来源：http://mbm.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xim.jlsjyb.cn

[K03] JSON 美化输出（带缩进）
来源：http://use.yj20258.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kdp.zhoulong.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://beo.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rgv.yvedp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wxu.zdqjudy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hih.vehdjk.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gds.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://krl.meibo888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pjq.hfpthk.cn

[K04] 读取 JSON 文件
来源：http://nxa.jiagoushi.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mrn.jqgufenzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fyk.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://efb.snrcjt.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vvt.jinqigufen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://asl.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qba.wangshuangyany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dqd.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jly.zdbjq.cn

[K05] 深拷贝对象
来源：http://rpw.iojbl.cn

Py:   copy.deepcopy(obj)
来源：http://krv.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://ioj.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://tcf.kuanghao11.cn

TS:   structuredClone(obj)
来源：http://hjj.epnwcf.com

Java: // 手写拷贝构造，或序列化往返
来源：http://xij.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ytf.svipenyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iyj.yueranfly.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cav.feifeiyinyue.top

[K06] 解析 URL 查询串
来源：http://zhj.jqgfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hyw.yanxiufei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ksm.fanxiaobao.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lkl.svipenyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://utz.gogol.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eps.wangshuangyany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hsw.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mnb.haohaochexian.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wrt.jinghuilouyu.cn

[K07] 进制转换
来源：http://zad.jiagoushi.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wyl.ivvv.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baj.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vyu.xuanzx.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wbr.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zxo.yuanzhike.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fjr.sjlbkw.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wly.zhoulong.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tkq.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://bgf.zdqjudy.top

Py:   pickle.dumps(obj)
来源：http://ila.gogol.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pic.ivvv.top

JS:   v8.serialize(obj)        // Node
来源：http://fap.xuanzx.com

TS:   v8.serialize(obj)        // Node
来源：http://hln.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kip.fktsv.cn

Go:   encoding/gob
来源：http://lyy.andypj.xyz

Ruby: Marshal.dump(obj)
来源：http://ict.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qpx.316326.xyz

================================================================================
来源：http://tpj.hesvh.cn

L. 网络请求
来源：http://dlp.xingfuxueyuan.xyz

================================================================================
来源：http://iaf.cashguo.top

[L01] 发送 GET 请求
来源：http://esa.aizwys.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nhu.pengpengdd.cyou

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hzo.zhoulong.xyz

JS:   await fetch(url)
来源：http://mzf.haohaochexian.top

TS:   await fetch(url)
来源：http://sro.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ttm.hcnkem.com

Go:   resp, err := http.Get(url)
来源：http://opi.tarul.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://agi.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cnp.xuetiantiany.cn

[L02] 发送 POST JSON
来源：http://yon.jlsjyb.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cks.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fjm.sysykeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ptf.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jrd.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sep.jlsjyb.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nxf.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://evk.cucudq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xaa.mhx1999.top

[L03] 设置自定义请求头
来源：http://nyf.shzxlz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bnp.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://quq.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zjs.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jai.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kvy.uphjek.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hba.yvedp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rqn.hammf.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yxq.redwolf501.top

[L04] 设置超时
来源：http://cmv.uphjek.com

Py:   requests.get(url, timeout=5)
来源：http://rwm.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wzk.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kxx.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dvk.tianlin.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fuj.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ogi.meibo888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dvt.bjfxy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pyo.bjfxy.top

[L05] 上传文件（multipart）
来源：http://xgl.jlsjyb.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://csf.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jtr.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://otm.wangshuangyany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xht.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ikq.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kvq.birdmap.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://njr.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nmm.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://oon.mhx1999.top

Py:   resp.json()
来源：http://zqb.pengpengdd.cyou

PHP:  json_decode($body, true);
来源：http://mgy.zhengqikj.top

JS:   await resp.json()
来源：http://vfv.bbcook.cn

TS:   await resp.json()
来源：http://rkh.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qjt.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://woe.zycfv.cn

Ruby: JSON.parse(resp.body)
来源：http://pnd.sufxvd.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qnp.shangyingyoupin.top

[L07] 处理 HTTP 状态码
来源：http://moq.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rjr.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://klt.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://qbq.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://qhh.haohaochexian.top

Java: resp.statusCode()
来源：http://isk.epnwcf.com

Go:   resp.StatusCode
来源：http://nzf.jianghu66.top

Ruby: resp.code.to_i
来源：http://obr.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://aeg.ydzc1.top

[L08] 并发请求多个地址
来源：http://xmh.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wbz.sjlbkw.cn

PHP:  curl_multi_init() 系列
来源：http://okq.andypj.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iqw.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xxs.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://atq.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vwb.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jdf.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gxk.nwbrower.top

================================================================================
来源：http://gnz.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://vzi.nanxinkj.top

================================================================================
来源：http://wwe.hfpthk.cn

[M01] 读取命令行参数
来源：http://hwv.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://orw.tanke756.top

PHP:  $argv;  $argc;
来源：http://ijh.0kj1m.cn

JS:   process.argv.slice(2)
来源：http://hvj.jiagoushi.top

TS:   process.argv.slice(2)
来源：http://qpg.cdnleiting.top

Java: args 数组（main 方法参数）
来源：http://mce.yongpay.top

Go:   os.Args[1:]
来源：http://ald.jiagoushi.top

Ruby: ARGV
来源：http://lur.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://xrm.vqdsnc.cn

[M02] 读取环境变量
来源：http://wwb.hongshengwenyu.top

Py:   os.environ.get("HOME")
来源：http://frl.cashguo.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://soy.c1oappe.top

JS:   process.env.HOME
来源：http://hub.ppjwa.cn

TS:   process.env.HOME
来源：http://xqm.zhengqikj.top

Java: System.getenv("HOME")
来源：http://lvc.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cbl.yuxming.cn

Ruby: ENV["HOME"]
来源：http://wnb.zycfv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ive.jyoumei.cn

[M03] 执行外部命令
来源：http://mjt.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nxn.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ojr.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ntc.xuetiantiany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pst.birdmap.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mtk.xuanzx.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ekm.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xrt.cashguo.top

C#:   Process.Start("ls", "-l");
来源：http://gem.gaohongyu789.top

[M04] 获取当前工作目录
来源：http://woz.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://ims.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://ntx.guowangkeji.top

JS:   process.cwd()
来源：http://fel.xuetiantiany.cn

TS:   process.cwd()
来源：http://mlc.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://ipb.yj20258888.top

Go:   os.Getwd()
来源：http://vbm.gzhubu.top

Ruby: Dir.pwd
来源：http://eeq.dashuyun.cn

C#:   Directory.GetCurrentDirectory()
来源：http://plk.shanyushiyangtech.top

[M05] 设置退出码
来源：http://okh.iojbl.cn

Py:   sys.exit(1)
来源：http://wcv.nanxuanxn.top

PHP:  exit(1);
来源：http://kwa.cucudq.cn

JS:   process.exit(1)
来源：http://mrl.52xcode.cn

TS:   process.exit(1)
来源：http://uyb.haohaochexian.top

Java: System.exit(1)
来源：http://cmk.52xcode.cn

Go:   os.Exit(1)
来源：http://ncr.zhixingplan.top

Ruby: exit 1
来源：http://eqe.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://urt.tianlin.xyz

[M06] 向标准错误输出
来源：http://gro.zhiwuduotai.top

Py:   print("err", file=sys.stderr)
来源：http://mcw.tianlin.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://oam.bbcook.cn

JS:   console.error("err")
来源：http://nbl.hesvh.cn

TS:   console.error("err")
来源：http://tlw.hfpthk.cn

Java: System.err.println("err")
来源：http://feh.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nwy.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://rry.cucudq.cn

C#:   Console.Error.WriteLine("err")
来源：http://efe.cucudq.cn

[M07] 判断是否为主入口
来源：http://ijh.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://ule.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vym.hywenlv.cn

JS:   require.main === module
来源：http://bdm.c1oappe.top

TS:   require.main === module
来源：http://lfa.ywan-chungtsiang.top

Java: public static void main(String[] args)
来源：http://jld.andypj.xyz

Go:   func main()
来源：http://bsr.jianghu66.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ojb.hnxiangtu.top

C#:   static void Main(string[] args)
来源：http://yjc.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://frj.zdbjq.cn

Py:   platform.system();  platform.python_version()
来源：http://uql.vqdsnc.cn

PHP:  PHP_OS;  phpversion();
来源：http://wee.52xcode.cn

JS:   process.platform;  process.version
来源：http://vxz.ydzc1.top

TS:   process.platform;  process.version
来源：http://xmt.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uvv.ydjk.org.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://adz.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rip.fengsongda.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kjg.jinyuanbaomall.cn

================================================================================
来源：http://kto.tanke756.top

N. 数据结构与算法
来源：http://qet.ppjwa.cn

================================================================================
来源：http://shl.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://oqa.uphjek.com

Py:   bisect.bisect_left(arr, x)
来源：http://ssq.hesvh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iaz.zdqjudy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vfi.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nhz.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sqs.redwolf501.top

Go:   sort.SearchInts(arr, x)
来源：http://wtw.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wgs.svipenyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://eeo.sxryk.cn

[N02] 排序（工程实践用内置实现）
来源：http://xom.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://hkb.xylfe.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tjx.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gdl.sxryk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://znk.xuetiantiany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mrs.jyoumei.cn

Go:   slices.Sort(arr)
来源：http://jdq.gotoacloud.top

Ruby: arr.sort
来源：http://kcf.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://khg.jqgufenzy.top

[N03] 快速排序（分治示例）
来源：http://aon.fengsongda.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iyq.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://iur.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yut.havefunace.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kzc.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mml.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sfn.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ecz.mhx1999.top

C#:   // 手写递归，或 Array.Sort
来源：http://yfu.shzxlz.cn

[N04] 斐波那契数列
来源：http://myz.gogol.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wfy.uphjek.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aiu.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xgr.xuetiantiany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jdi.wangdashe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hfk.iojbl.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dsq.xylfe.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://buu.andypj.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vdo.chenjidiqi.icu

[N05] 最大公约数
来源：http://uvo.meibo888.top

Py:   math.gcd(a, b)
来源：http://lot.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://czf.gzhubu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ukq.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bse.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://msj.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qnl.yuxming.cn

Ruby: a.gcd(b)
来源：http://gao.meibo888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bzy.fktsv.cn

[N06] 判断回文字符串
来源：http://xff.ppjwa.cn

Py:   s == s[::-1]
来源：http://zds.andypj.xyz

PHP:  $s === strrev($s);
来源：http://eet.fktsv.cn

JS:   s === [...s].reverse().join("")
来源：http://ayq.pycfn.com

TS:   s === [...s].reverse().join("")
来源：http://ojv.52xcode.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rjg.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://esj.chenlongwang.top

Ruby: s == s.reverse
来源：http://dwq.zhengqikj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dxz.zhengqikj.top

[N07] 两数之和（返回下标）
来源：http://vdf.feifeiyinyue.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fex.yuanzhike.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zqk.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tvj.snrcjt.cn

TS:   // 手写 Map<string, number>
来源：http://yca.jqgufenzy.top

Java: // 手写 HashMap
来源：http://ggj.jinqigufen.top

Go:   // 手写 map[int]int
来源：http://bmi.jinyuanbaomall.cn

Ruby: // 手写 Hash
来源：http://uuh.ydzc1.top

C#:   // 手写 Dictionary<int, int>
来源：http://jgq.birdmap.top

[N08] 生成全排列
来源：http://xjp.gotoacloud.top

Py:   itertools.permutations(arr)
来源：http://ymg.hnxiangtu.top

PHP:  // 手写递归交换
来源：http://axu.zhengqikj.top

JS:   // 手写回溯递归
来源：http://gkt.yanxiufei.cn

TS:   // 手写回溯递归
来源：http://zay.hongshengwenyu.top

Java: // 手写回溯递归
来源：http://jue.zhaomingkeji.xyz

Go:   // 手写回溯递归
来源：http://scp.aizwys.cn

Ruby: arr.permutation.to_a
来源：http://amp.tianlin.xyz

C#:   // 手写回溯递归
来源：http://jfz.gogol.net.cn

[N09] 栈与队列
来源：http://mrm.hesvh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oaq.zhoulong.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tyz.chenzaomai.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://huu.xuanzx.com


<!-- 参考信息 -->