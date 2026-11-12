代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://ttp.shuidangran.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aza.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ksu.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://awx.hammf.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pby.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sej.xuetiantiany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yra.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oil.jianghu66.top

================================================================================
来源：http://gqr.shuidangran.top

K. JSON 与序列化
来源：http://klm.jinqigufen.top

================================================================================
来源：http://wht.gzhubu.top

[K01] 对象转 JSON 字符串
来源：http://dsw.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oqw.52xcode.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hxu.zhengqikj.top

JS:   JSON.stringify(obj)
来源：http://bam.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://bzp.redwolf501.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tgi.shangyingyoupin.top

Go:   json.Marshal(obj)
来源：http://mqu.nanxuanxn.top

Ruby: obj.to_json                                     // require "json"
来源：http://wjo.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ncm.0kj1m.cn

[K02] JSON 字符串转对象
来源：http://dum.ehwqpu.com

Py:   json.loads(s)
来源：http://noq.316326.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uvv.gotoacloud.top

JS:   JSON.parse(s)
来源：http://asp.shanyushiyangtech.top

TS:   JSON.parse(s)
来源：http://wfy.yfazqb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ydx.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://een.zdbjq.cn

Ruby: JSON.parse(s)
来源：http://epe.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lif.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://qed.jinyuanbaomall.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://osq.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hbm.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ngn.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mlf.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cwj.yj202588.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://agu.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://zew.tanke756.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mvb.havefunace.top

[K04] 读取 JSON 文件
来源：http://fvy.hammf.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tmt.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pbk.sxryk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ega.nanxuanxn.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tyh.xinyue.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jsl.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yzv.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gzz.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://onn.sysykeji.top

[K05] 深拷贝对象
来源：http://dbr.ybcxt.top

Py:   copy.deepcopy(obj)
来源：http://jed.yanxiufei.cn

PHP:  unserialize(serialize($obj));
来源：http://ebh.wangdashe.top

JS:   structuredClone(obj)
来源：http://ypo.ybcxt.top

TS:   structuredClone(obj)
来源：http://yrr.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kzq.hammf.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ihj.tianlin.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gwx.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://zjt.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://vpe.pycfn.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fby.yongpay.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jxc.epnwcf.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xca.9152youxi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qha.yangfankeji.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lup.yuanzhike.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jwu.zhixingplan.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zug.iojbl.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ilk.chenzaomai.com

[K07] 进制转换
来源：http://qxh.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dix.chenjidiqi.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fnw.ywan-chungtsiang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dyn.guannengcc.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cmf.yj20258888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vtv.dashuyun.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ibb.vehdjk.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cvj.gzhubu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cra.daxiang520.top

[K08] 二进制序列化（非 JSON）
来源：http://rbv.yj20258.top

Py:   pickle.dumps(obj)
来源：http://khg.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jvr.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://krm.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://xyc.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jrc.jianghu66.top

Go:   encoding/gob
来源：http://nqp.snrcjt.cn

Ruby: Marshal.dump(obj)
来源：http://vne.ivvv.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ful.xuanzx.com

================================================================================
来源：http://jtl.cashguo.top

L. 网络请求
来源：http://zcd.chenzaomai.com

================================================================================
来源：http://iby.havefunace.top

[L01] 发送 GET 请求
来源：http://awr.hywenlv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dqo.ctjpmb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ucv.gzhubu.top

JS:   await fetch(url)
来源：http://fjs.vqdsnc.cn

TS:   await fetch(url)
来源：http://nxc.sysykeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ulf.yangfankeji.com

Go:   resp, err := http.Get(url)
来源：http://flr.zhijiandao.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lqs.pengpengdd.cyou

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zyx.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://yni.ppjwa.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ito.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ivy.yfazqb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://swi.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jrb.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rqw.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://laz.9152youxi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fue.yfazqb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gld.zycfv.cn

[L03] 设置自定义请求头
来源：http://itg.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://coz.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jci.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://veq.birdmap.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cip.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fmr.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nyz.c1oappe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iej.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://unf.jlsjyb.cn

[L04] 设置超时
来源：http://uuw.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://lzb.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vmb.aibaodan.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mcq.kuanghao11.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vjj.jlsjyb.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pos.yongpay.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uze.dashuyun.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://unu.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://plb.dashuyun.cn

[L05] 上传文件（multipart）
来源：http://cho.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yze.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bux.tanke756.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ihr.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lwr.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://inj.mhx1999.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wmj.shanyushiyangtech.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://taf.sweek.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vco.dianchejie.cn

[L06] 解析响应为 JSON
来源：http://reh.cqqwz.cn

Py:   resp.json()
来源：http://kau.yvedp.cn

PHP:  json_decode($body, true);
来源：http://knv.hcnkem.com

JS:   await resp.json()
来源：http://rvu.bbcook.cn

TS:   await resp.json()
来源：http://aww.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jsb.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tbv.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://zmw.ydzc1.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tfv.vqdsnc.cn

[L07] 处理 HTTP 状态码
来源：http://fjq.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sji.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://edw.zhijiandao.cn

JS:   resp.ok;  resp.status
来源：http://ufs.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://ynk.9152youxi.cn

Java: resp.statusCode()
来源：http://ibe.daria6918.cn

Go:   resp.StatusCode
来源：http://ibq.9152youxi.cn

Ruby: resp.code.to_i
来源：http://nhr.vqdsnc.cn

C#:   (int)resp.StatusCode
来源：http://igb.nwbrower.top

[L08] 并发请求多个地址
来源：http://ihv.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pkd.sxryk.cn

PHP:  curl_multi_init() 系列
来源：http://jib.ivvv.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eyx.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hhm.jinyuanbaomall.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wpy.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rgw.wangshuangyany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://crq.shuidangran.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hvx.sweek.top

================================================================================
来源：http://akx.daxiang520.top

M. 命令行 / 进程 / 环境
来源：http://jce.wangshuangyany.cn

================================================================================
来源：http://rdy.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://nan.uphjek.com

Py:   sys.argv[1:]
来源：http://jwr.gzhubu.top

PHP:  $argv;  $argc;
来源：http://wvf.mhx1999.top

JS:   process.argv.slice(2)
来源：http://vls.cdnleiting.top

TS:   process.argv.slice(2)
来源：http://enc.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://iyl.chenlongwang.top

Go:   os.Args[1:]
来源：http://ble.jinqigufen.top

Ruby: ARGV
来源：http://zae.chenjidiqi.icu

C#:   args 数组（Main 方法参数）
来源：http://xkh.dashuyun.cn

[M02] 读取环境变量
来源：http://bsu.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://bhn.fengsongda.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uwz.ivvv.top

JS:   process.env.HOME
来源：http://srj.shuidangran.top

TS:   process.env.HOME
来源：http://bpc.shzxlz.cn

Java: System.getenv("HOME")
来源：http://apb.shanyushiyangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aey.xuanzx.com

Ruby: ENV["HOME"]
来源：http://vhf.cheryme.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kei.chenzaomai.com

[M03] 执行外部命令
来源：http://kbz.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nhv.ivvv.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zwy.guannengcc.top

JS:   child_process.execSync("ls -l").toString()
来源：http://adb.shzxlz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fwx.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://esu.yuanzhike.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xtk.yueranfly.top

Ruby: system("ls -l");  `ls -l`
来源：http://qkg.wangshuangyany.cn

C#:   Process.Start("ls", "-l");
来源：http://dyi.nwbrower.top

[M04] 获取当前工作目录
来源：http://ecy.nanxinkj.top

Py:   os.getcwd()
来源：http://dpv.chenzaomai.com

PHP:  getcwd();
来源：http://zpy.wangdashe.top

JS:   process.cwd()
来源：http://ojg.andypj.xyz

TS:   process.cwd()
来源：http://tyr.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://urv.hysaishi.cn

Go:   os.Getwd()
来源：http://awj.316326.xyz

Ruby: Dir.pwd
来源：http://aaa.xingfuxueyuan.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://nes.shuidangran.top

[M05] 设置退出码
来源：http://ikb.tian-w.cn

Py:   sys.exit(1)
来源：http://msp.zdqjudy.top

PHP:  exit(1);
来源：http://mpz.andypj.xyz

JS:   process.exit(1)
来源：http://zkk.hammf.cn

TS:   process.exit(1)
来源：http://yux.zhiwuduotai.top

Java: System.exit(1)
来源：http://wtf.zdbjq.cn

Go:   os.Exit(1)
来源：http://nqn.dashuyun.cn

Ruby: exit 1
来源：http://hle.shanyushiyangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nzf.tarul.cn

[M06] 向标准错误输出
来源：http://neg.zhongyouzk.top

Py:   print("err", file=sys.stderr)
来源：http://uyb.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://uwb.ydjk.org.cn

JS:   console.error("err")
来源：http://xag.tianlin.xyz

TS:   console.error("err")
来源：http://lna.dianchejie.cn

Java: System.err.println("err")
来源：http://ise.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lrc.cqqwz.cn

Ruby: warn "err"
来源：http://dqu.316326.xyz

C#:   Console.Error.WriteLine("err")
来源：http://tev.jlsjyb.cn

[M07] 判断是否为主入口
来源：http://luj.shanyushiyangkeji.top

Py:   if __name__ == "__main__":
来源：http://xib.snrcjt.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zvm.snrcjt.cn

JS:   require.main === module
来源：http://ttp.sjlbkw.cn

TS:   require.main === module
来源：http://pih.yuanzhike.top

Java: public static void main(String[] args)
来源：http://spe.vqdsnc.cn

Go:   func main()
来源：http://ioz.redwolf501.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://onr.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://ntq.chenlongwang.top

[M08] 获取系统与运行时信息
来源：http://ihx.dashuyun.cn

Py:   platform.system();  platform.python_version()
来源：http://evf.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://gpi.vehdjk.com

JS:   process.platform;  process.version
来源：http://fhy.vehdjk.com

TS:   process.platform;  process.version
来源：http://mwu.shanyushiyangtech.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cde.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cvq.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gqy.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://njf.dashuyun.cn

================================================================================
来源：http://wbt.ydzc1.top

N. 数据结构与算法
来源：http://xds.dashuyun.cn

================================================================================
来源：http://yyo.ehwqpu.com

[N01] 二分查找（有序数组）
来源：http://drk.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://qwg.c1oappe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://npy.9152youxi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vtr.sufxvd.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sds.pengpengdd.cyou

Java: Arrays.binarySearch(arr, x)
来源：http://vol.vqdsnc.cn

Go:   sort.SearchInts(arr, x)
来源：http://kmt.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dvl.jinyuanbaomall.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jqg.jqgfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://xsx.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://fku.sweek.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eaj.ctjpmb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://bra.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gpe.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fat.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://pgj.vqdsnc.cn

Ruby: arr.sort
来源：http://cun.c1oappe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xne.uphjek.com

[N03] 快速排序（分治示例）
来源：http://zjj.jinqigfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lnz.gaohongyu789.top

PHP:  // 递归实现，或用 usort
来源：http://xvq.zdbjq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zib.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ngb.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tdc.iojbl.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://war.0kj1m.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zkl.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://kxb.jianghu66.top

[N04] 斐波那契数列
来源：http://rfn.yuanzhike.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://grz.quarkkingdee.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tgm.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iju.pengpengdd.cyou

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://omd.cucudq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vyp.gzhubu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pan.yuanzhike.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qim.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://acz.yueranfly.top

[N05] 最大公约数
来源：http://dkv.nwbrower.top

Py:   math.gcd(a, b)
来源：http://nvy.birdmap.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fjq.hesvh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vbd.zdbjq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gll.yangfankeji.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://owd.jyoumei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uav.ybcxt.top

Ruby: a.gcd(b)
来源：http://ahs.yongpay.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://epj.xuanzx.com

[N06] 判断回文字符串
来源：http://zcf.daxiang520.top

Py:   s == s[::-1]
来源：http://jqd.xziqi.cn

PHP:  $s === strrev($s);
来源：http://gjo.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://saw.jinyuanbaomall.cn

TS:   s === [...s].reverse().join("")
来源：http://ijn.shzxlz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://shn.aizwys.cn

Go:   // 双指针从两端比较
来源：http://lza.shanyushiyangkeji.top

Ruby: s == s.reverse
来源：http://lrk.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://usx.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://ulj.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jzm.yj20258.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sfx.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://gpj.jqgufenzy.top

TS:   // 手写 Map<string, number>
来源：http://gyv.xuetiantiany.cn

Java: // 手写 HashMap
来源：http://gqb.shangyingyoupin.top

Go:   // 手写 map[int]int
来源：http://lwc.havefunace.top

Ruby: // 手写 Hash
来源：http://fiy.hnxiangtu.top

C#:   // 手写 Dictionary<int, int>
来源：http://bht.zhixingplan.top

[N08] 生成全排列
来源：http://btn.bbcook.cn


<!-- 参考信息 -->