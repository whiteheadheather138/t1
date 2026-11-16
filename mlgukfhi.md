代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rfk.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cab.hcnkem.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cqg.ydzc1.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xcc.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nyh.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mjs.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kcx.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://tch.zycfv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xuw.mhx1999.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zyt.zhongyouzk.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qyb.tarul.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xaf.0kj1m.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ccn.chenlongwang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zpp.gzhubu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gdi.jyoumei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://epq.xingfuxueyuan.xyz

================================================================================
来源：http://thz.andypj.xyz

K. JSON 与序列化
来源：http://bqh.gaohongyu789.top

================================================================================
来源：http://fer.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://cqk.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lip.c1oappe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://grw.meibo888.top

JS:   JSON.stringify(obj)
来源：http://ooh.zycfv.cn

TS:   JSON.stringify(obj)
来源：http://eok.sysykeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vtr.xingfuxueyuan.xyz

Go:   json.Marshal(obj)
来源：http://mpc.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dfm.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://hsn.cucudq.cn

[K02] JSON 字符串转对象
来源：http://pzi.hnqzz.top

Py:   json.loads(s)
来源：http://kka.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wvc.xinyue.icu

JS:   JSON.parse(s)
来源：http://lkg.jianghu66.top

TS:   JSON.parse(s)
来源：http://dmv.ydzc1.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xwz.xuanzx.com

Go:   json.Unmarshal(data, &v)
来源：http://qwx.hnqzz.top

Ruby: JSON.parse(s)
来源：http://cwa.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xld.fanxiaobao.xyz

[K03] JSON 美化输出（带缩进）
来源：http://aca.svipenyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://spd.zycfv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xdd.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://agg.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bhr.316326.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iec.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wsf.shzxlz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xxa.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mit.tian-w.cn

[K04] 读取 JSON 文件
来源：http://zcc.epnwcf.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pna.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://veq.pycfn.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tbw.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lep.ctjpmb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cke.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rlu.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tto.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jfw.xziqi.cn

[K05] 深拷贝对象
来源：http://kcy.dashuyun.cn

Py:   copy.deepcopy(obj)
来源：http://usk.jiagoushi.top

PHP:  unserialize(serialize($obj));
来源：http://dfi.xuanzx.com

JS:   structuredClone(obj)
来源：http://mch.pycfn.com

TS:   structuredClone(obj)
来源：http://nkk.cdnleiting.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bun.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://awv.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tny.jinyuanbaomall.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vao.cdnleiting.top

[K06] 解析 URL 查询串
来源：http://uid.nanxuanxn.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wxj.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iyv.bjfxy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://evg.jinyuanbaomall.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wxy.andypj.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nno.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fyn.aizwys.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hde.andypj.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lpv.epnwcf.com

[K07] 进制转换
来源：http://dtw.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://far.xziqi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dxk.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pde.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qcd.gzhubu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kqi.nwbrower.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qhn.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://akg.daxiang520.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gqc.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://xfo.52xcode.cn

Py:   pickle.dumps(obj)
来源：http://cex.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://xjz.feifeiyinyue.top

JS:   v8.serialize(obj)        // Node
来源：http://aby.316326.xyz

TS:   v8.serialize(obj)        // Node
来源：http://xve.tianlin.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qkr.bjfxy.top

Go:   encoding/gob
来源：http://hcd.fengsongda.top

Ruby: Marshal.dump(obj)
来源：http://mxw.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bzd.jianghu66.top

================================================================================
来源：http://eec.sysykeji.top

L. 网络请求
来源：http://bpd.tian-w.cn

================================================================================
来源：http://tkh.ppjwa.cn

[L01] 发送 GET 请求
来源：http://acu.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bro.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uzh.jqgfzy.top

JS:   await fetch(url)
来源：http://mak.vqdsnc.cn

TS:   await fetch(url)
来源：http://nqz.sufxvd.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hsc.daria6918.cn

Go:   resp, err := http.Get(url)
来源：http://wlg.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pjr.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://umu.haohaochexian.top

[L02] 发送 POST JSON
来源：http://vus.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://gwn.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xhl.9152youxi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fzl.xziqi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zvo.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jrr.yueranfly.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ldn.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vrg.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fpj.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://bzy.zhoulong.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fmh.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hiy.xziqi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://njm.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xov.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oqy.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pwk.yueranfly.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nuj.yangfankeji.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sfs.haohaochexian.top

[L04] 设置超时
来源：http://vad.hywenlv.cn

Py:   requests.get(url, timeout=5)
来源：http://gkl.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pti.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://urk.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lur.hesvh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kck.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wjt.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yhf.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zhh.zycfv.cn

[L05] 上传文件（multipart）
来源：http://khv.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mwg.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yyi.fehbvm.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tsa.smart0.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://unw.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vol.zhixingplan.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uqc.jianghu66.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dlp.jiagoushi.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vfo.jyoumei.cn

[L06] 解析响应为 JSON
来源：http://yoh.fktsv.cn

Py:   resp.json()
来源：http://pzw.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://wja.dashuyun.cn

JS:   await resp.json()
来源：http://yln.xingfuxueyuan.xyz

TS:   await resp.json()
来源：http://cgt.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qos.sxryk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nir.ybcxt.top

Ruby: JSON.parse(resp.body)
来源：http://lhr.yangfankeji.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ukf.guannengcc.top

[L07] 处理 HTTP 状态码
来源：http://ebp.meibo888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://suk.uphjek.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pys.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://zjp.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://siy.cucudq.cn

Java: resp.statusCode()
来源：http://dmf.jiagoushi.top

Go:   resp.StatusCode
来源：http://cgy.wangshuangyany.cn

Ruby: resp.code.to_i
来源：http://hae.sysykeji.top

C#:   (int)resp.StatusCode
来源：http://hte.gogol.net.cn

[L08] 并发请求多个地址
来源：http://xta.fehbvm.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://axn.fzhhl.top

PHP:  curl_multi_init() 系列
来源：http://lvc.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fwa.guannengcc.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jsr.quarkkingdee.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://buw.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lil.guannengcc.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wsp.tanke756.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vfb.bbcook.cn

================================================================================
来源：http://vlu.zdbjq.cn

M. 命令行 / 进程 / 环境
来源：http://vzy.dianchejie.cn

================================================================================
来源：http://tul.snrcjt.cn

[M01] 读取命令行参数
来源：http://ybl.birdmap.top

Py:   sys.argv[1:]
来源：http://ipe.hnqzz.top

PHP:  $argv;  $argc;
来源：http://vna.chenlongwang.top

JS:   process.argv.slice(2)
来源：http://aoy.316326.xyz

TS:   process.argv.slice(2)
来源：http://xxt.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://tnw.jinghuilouyu.cn

Go:   os.Args[1:]
来源：http://voj.epnwcf.com

Ruby: ARGV
来源：http://kva.shzxlz.cn

C#:   args 数组（Main 方法参数）
来源：http://adw.jiagoushi.top

[M02] 读取环境变量
来源：http://voi.ybcxt.top

Py:   os.environ.get("HOME")
来源：http://wrd.ivvv.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tfe.aizwys.cn

JS:   process.env.HOME
来源：http://wxa.bbcook.cn

TS:   process.env.HOME
来源：http://mkk.shangyingyoupin.top

Java: System.getenv("HOME")
来源：http://kjg.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lpn.zhiwuduotai.top

Ruby: ENV["HOME"]
来源：http://uym.hysaishi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mwc.yj202588.top

[M03] 执行外部命令
来源：http://gee.birdmap.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fyg.feifeiyinyue.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wpv.yfazqb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://hfq.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nsa.hnxiangtu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rcf.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://apk.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://tmw.zhoulong.xyz

C#:   Process.Start("ls", "-l");
来源：http://yzh.cashguo.top

[M04] 获取当前工作目录
来源：http://sgg.yvedp.cn

Py:   os.getcwd()
来源：http://obe.tanke756.top

PHP:  getcwd();
来源：http://nsc.yangfankeji.com

JS:   process.cwd()
来源：http://eyp.jlsjyb.cn

TS:   process.cwd()
来源：http://fxg.tianlin.xyz

Java: Path.of("").toAbsolutePath()
来源：http://hsh.yj20258.top

Go:   os.Getwd()
来源：http://wrg.jinyuanbaomall.cn

Ruby: Dir.pwd
来源：http://xly.jinghuilouyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xps.sjlbkw.cn

[M05] 设置退出码
来源：http://ltd.shanyushiyangtech.top

Py:   sys.exit(1)
来源：http://cxv.gaohongyu789.top

PHP:  exit(1);
来源：http://wbs.cucudq.cn

JS:   process.exit(1)
来源：http://kur.bjfxy.top

TS:   process.exit(1)
来源：http://tox.xuetiantiany.cn

Java: System.exit(1)
来源：http://egy.xuetiantiany.cn

Go:   os.Exit(1)
来源：http://jfr.fanxiaobao.xyz

Ruby: exit 1
来源：http://emc.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zom.zhoulong.xyz

[M06] 向标准错误输出
来源：http://dnz.svipenyu.cn

Py:   print("err", file=sys.stderr)
来源：http://lvh.wangshuangyany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ydx.cucudq.cn

JS:   console.error("err")
来源：http://cux.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://eto.jqgfzy.top

Java: System.err.println("err")
来源：http://cvx.cashguo.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mig.hongshengwenyu.top

Ruby: warn "err"
来源：http://xns.ehwqpu.com

C#:   Console.Error.WriteLine("err")
来源：http://sdb.gotoacloud.top

[M07] 判断是否为主入口
来源：http://tnh.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://rvj.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zqv.zdbjq.cn

JS:   require.main === module
来源：http://ekb.wangdashe.top

TS:   require.main === module
来源：http://npy.0kj1m.cn

Java: public static void main(String[] args)
来源：http://tps.wangshuangyany.cn

Go:   func main()
来源：http://lpz.cheryme.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gkq.aizwys.cn

C#:   static void Main(string[] args)
来源：http://det.hcnkem.com

[M08] 获取系统与运行时信息
来源：http://hjf.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://cdu.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://pdn.ppjwa.cn

JS:   process.platform;  process.version
来源：http://bmc.fktsv.cn

TS:   process.platform;  process.version
来源：http://fvh.bbcook.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mbf.fzhhl.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vih.jqgfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xnj.ehwqpu.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://wfp.ivvv.top

================================================================================
来源：http://etx.epnwcf.com

N. 数据结构与算法
来源：http://old.nwbrower.top

================================================================================
来源：http://dnb.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://chx.zhiwuduotai.top

Py:   bisect.bisect_left(arr, x)
来源：http://vgy.xziqi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xll.jyoumei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uiu.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pvi.jinqigufen.top

Java: Arrays.binarySearch(arr, x)
来源：http://afi.ydzc1.top

Go:   sort.SearchInts(arr, x)
来源：http://mue.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://fqh.bjfxy.top

C#:   Array.BinarySearch(arr, x)
来源：http://pjk.hnqzz.top

[N02] 排序（工程实践用内置实现）
来源：http://yju.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://gtw.hysaishi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://phw.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://eja.sjlbkw.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kgr.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jwf.hesvh.cn

Go:   slices.Sort(arr)
来源：http://gba.snrcjt.cn

Ruby: arr.sort
来源：http://rfi.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://wvu.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://vvj.ppjwa.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bxb.sxryk.cn

PHP:  // 递归实现，或用 usort
来源：http://vev.zhengqikj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://coa.yongpay.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nkf.xziqi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zhg.gogol.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ldb.zhoulong.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://awx.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xmj.zhengqikj.top

[N04] 斐波那契数列
来源：http://equ.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dht.gogol.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://phr.bjfxy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wwf.cheryme.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iql.gotoacloud.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jeg.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ajt.hnqzz.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ldf.ybcxt.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tks.cucudq.cn

[N05] 最大公约数
来源：http://tsu.yj20258.top

Py:   math.gcd(a, b)
来源：http://byu.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nvs.fanxiaobao.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://swm.epnwcf.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kke.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wuz.quarkkingdee.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nvn.cheryme.top

Ruby: a.gcd(b)
来源：http://mcv.shanyushiyangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hbz.uphjek.com

[N06] 判断回文字符串
来源：http://xwx.jinqigufen.top

Py:   s == s[::-1]
来源：http://zwx.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://omr.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://wvm.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://hvg.xuetiantiany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ncn.yuxming.cn

Go:   // 双指针从两端比较
来源：http://hkk.daxiang520.top

Ruby: s == s.reverse
来源：http://bky.ydjk.org.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://enu.svipenyu.cn

[N07] 两数之和（返回下标）
来源：http://yjt.hfpthk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mih.cashguo.top


<!-- 参考信息 -->