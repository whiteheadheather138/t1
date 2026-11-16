代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wnn.hysaishi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dng.havefunace.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ytn.gaohongyu789.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ypr.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iqo.dianchejie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kzn.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wgt.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://wtk.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dll.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jvh.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xap.0kj1m.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dsk.chenzaomai.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tbf.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ajh.tian-w.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ntb.hnqzz.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tgq.316326.xyz

================================================================================
来源：http://ujd.shuidangran.top

K. JSON 与序列化
来源：http://hat.bjfxy.top

================================================================================
来源：http://jhv.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://epg.jianghu66.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kqv.bjfxy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lvn.tanke756.top

JS:   JSON.stringify(obj)
来源：http://dio.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://kls.sufxvd.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uwp.redwolf501.top

Go:   json.Marshal(obj)
来源：http://vdr.shanyushiyangtech.top

Ruby: obj.to_json                                     // require "json"
来源：http://hgd.yj20258888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tnn.zhiwuduotai.top

[K02] JSON 字符串转对象
来源：http://aqt.jinghuilouyu.cn

Py:   json.loads(s)
来源：http://ian.birdmap.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://icb.sysykeji.top

JS:   JSON.parse(s)
来源：http://eqa.nanxuanxn.top

TS:   JSON.parse(s)
来源：http://kwb.wangdashe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ike.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://tpc.zhoulong.xyz

Ruby: JSON.parse(s)
来源：http://tyr.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mjb.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://ejr.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://juf.yongpay.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hqk.shzxlz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sxx.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fow.hfpthk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vzi.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bqo.zhixingplan.top

Ruby: JSON.pretty_generate(obj)
来源：http://ruy.yfazqb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jda.cheryme.top

[K04] 读取 JSON 文件
来源：http://jjc.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fam.nanxinkj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xgg.andypj.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rym.sweek.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qji.andypj.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sht.yfazqb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wnn.zhiwuduotai.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rcj.316326.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lki.cdnleiting.top

[K05] 深拷贝对象
来源：http://eft.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://wqq.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://avu.chenlongwang.top

JS:   structuredClone(obj)
来源：http://ihm.guannengcc.top

TS:   structuredClone(obj)
来源：http://vnc.snrcjt.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uuc.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iug.hesvh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lrn.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qxf.yvedp.cn

[K06] 解析 URL 查询串
来源：http://kui.zhoulong.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gcx.hysaishi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pec.chenzaomai.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rku.jqgufenzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lct.yonumen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lcz.haohaochexian.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://axn.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lyo.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eae.yuanzhike.top

[K07] 进制转换
来源：http://mak.jiagoushi.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cif.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ott.gaohongyu789.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wco.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sva.snrcjt.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eze.jinghuilouyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://joy.cucudq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mlv.shangyingyoupin.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hkp.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://unz.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://oas.yanxiufei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://aej.mhx1999.top

JS:   v8.serialize(obj)        // Node
来源：http://plx.ybcxt.top

TS:   v8.serialize(obj)        // Node
来源：http://ycq.xuanzx.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nso.vehdjk.com

Go:   encoding/gob
来源：http://zbf.guannengcc.top

Ruby: Marshal.dump(obj)
来源：http://sru.zhijiandao.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jkw.yanxiufei.cn

================================================================================
来源：http://jrn.fzhhl.top

L. 网络请求
来源：http://ltf.sxryk.cn

================================================================================
来源：http://scn.hnqzz.top

[L01] 发送 GET 请求
来源：http://rcl.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hqm.zhengqikj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dry.tanke756.top

JS:   await fetch(url)
来源：http://wbx.shangyingyoupin.top

TS:   await fetch(url)
来源：http://kme.zdqjudy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gyu.cdnleiting.top

Go:   resp, err := http.Get(url)
来源：http://tyh.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cka.haohaochexian.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://plx.aizwys.cn

[L02] 发送 POST JSON
来源：http://umb.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://dye.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nfr.havefunace.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mdi.zhixingplan.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://thq.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rrr.yvedp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://anf.yfazqb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xuj.pengpengdd.cyou

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ljt.yvedp.cn

[L03] 设置自定义请求头
来源：http://fnm.shanyushiyangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rcs.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://chc.zhoulong.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cls.hesvh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gft.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ipz.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tfe.tian-w.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wty.shanyushiyangtech.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fnp.ydzc1.top

[L04] 设置超时
来源：http://aod.shzxlz.cn

Py:   requests.get(url, timeout=5)
来源：http://yuw.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mfe.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kso.vqdsnc.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yhi.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hqp.cqqwz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://krl.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ytf.yuxming.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hob.daria6918.cn

[L05] 上传文件（multipart）
来源：http://nnq.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yec.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kby.aizwys.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mip.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gjg.sxryk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sbt.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fyi.chenzaomai.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mip.andypj.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sbc.cucudq.cn

[L06] 解析响应为 JSON
来源：http://naj.guowangkeji.top

Py:   resp.json()
来源：http://zee.birdmap.top

PHP:  json_decode($body, true);
来源：http://grn.zdqjudy.top

JS:   await resp.json()
来源：http://fwj.sxryk.cn

TS:   await resp.json()
来源：http://ejc.yonumen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bhs.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dot.bbcook.cn

Ruby: JSON.parse(resp.body)
来源：http://bop.jiagoushi.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vfr.nwbrower.top

[L07] 处理 HTTP 状态码
来源：http://vgb.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://poh.yuxming.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uoi.iojbl.cn

JS:   resp.ok;  resp.status
来源：http://krv.zhaomingkeji.xyz

TS:   resp.ok;  resp.status
来源：http://oun.c1oappe.top

Java: resp.statusCode()
来源：http://txa.ybcxt.top

Go:   resp.StatusCode
来源：http://ysz.epnwcf.com

Ruby: resp.code.to_i
来源：http://oca.shanyushiyangkeji.top

C#:   (int)resp.StatusCode
来源：http://vez.316326.xyz

[L08] 并发请求多个地址
来源：http://nam.yangfankeji.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nur.zdqjudy.top

PHP:  curl_multi_init() 系列
来源：http://lct.jinghuilouyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://scp.andypj.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nou.nwbrower.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://seb.jqgufenzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://evi.hfpthk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sbb.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://evu.feifeiyinyue.top

================================================================================
来源：http://wmi.xuetiantiany.cn

M. 命令行 / 进程 / 环境
来源：http://dvr.vqdsnc.cn

================================================================================
来源：http://euv.nwbrower.top

[M01] 读取命令行参数
来源：http://asm.xziqi.cn

Py:   sys.argv[1:]
来源：http://lbn.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://gsf.birdmap.top

JS:   process.argv.slice(2)
来源：http://mxj.chenjidiqi.icu

TS:   process.argv.slice(2)
来源：http://lli.uphjek.com

Java: args 数组（main 方法参数）
来源：http://mkl.zhiwuduotai.top

Go:   os.Args[1:]
来源：http://stg.jinyuanbaomall.cn

Ruby: ARGV
来源：http://emo.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://sku.sjlbkw.cn

[M02] 读取环境变量
来源：http://rrb.zhiwuduotai.top

Py:   os.environ.get("HOME")
来源：http://fmi.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://php.yueranfly.top

JS:   process.env.HOME
来源：http://mdq.zdqjudy.top

TS:   process.env.HOME
来源：http://jtr.hesvh.cn

Java: System.getenv("HOME")
来源：http://opr.guannengcc.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qok.yj20258.top

Ruby: ENV["HOME"]
来源：http://lrl.shanyushiyangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://inq.haohaochexian.top

[M03] 执行外部命令
来源：http://olm.svipenyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jxq.gotoacloud.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xik.ehwqpu.com

JS:   child_process.execSync("ls -l").toString()
来源：http://zkt.fzhhl.top

TS:   child_process.execSync("ls -l").toString()
来源：http://eih.fengsongda.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zqg.jqgufenzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mhi.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://yqa.gotoacloud.top

C#:   Process.Start("ls", "-l");
来源：http://osq.yonumen.top

[M04] 获取当前工作目录
来源：http://kbe.yj20258.top

Py:   os.getcwd()
来源：http://vfq.shuidangran.top

PHP:  getcwd();
来源：http://nzm.dianchejie.cn

JS:   process.cwd()
来源：http://mjc.wangdashe.top

TS:   process.cwd()
来源：http://oex.nwbrower.top

Java: Path.of("").toAbsolutePath()
来源：http://dzc.shzxlz.cn

Go:   os.Getwd()
来源：http://zub.zycfv.cn

Ruby: Dir.pwd
来源：http://tmi.smart0.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://owd.smart0.xyz

[M05] 设置退出码
来源：http://gzw.mhx1999.top

Py:   sys.exit(1)
来源：http://taw.quarkkingdee.top

PHP:  exit(1);
来源：http://yvf.zhengqikj.top

JS:   process.exit(1)
来源：http://rpb.hywenlv.cn

TS:   process.exit(1)
来源：http://voe.hywenlv.cn

Java: System.exit(1)
来源：http://amo.meibo888.top

Go:   os.Exit(1)
来源：http://eqt.guowangkeji.top

Ruby: exit 1
来源：http://irr.tarul.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rhc.jiagoushi.top

[M06] 向标准错误输出
来源：http://lkx.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://bnk.vehdjk.com

PHP:  fwrite(STDERR, "err\n");
来源：http://ahl.feifeiyinyue.top

JS:   console.error("err")
来源：http://zpa.shuidangran.top

TS:   console.error("err")
来源：http://nap.hysaishi.cn

Java: System.err.println("err")
来源：http://qfv.aibaodan.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tam.ctjpmb.com

Ruby: warn "err"
来源：http://sdq.sysykeji.top

C#:   Console.Error.WriteLine("err")
来源：http://hpz.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://oll.ydzc1.top

Py:   if __name__ == "__main__":
来源：http://qyo.chenjidiqi.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zdb.shuidangran.top

JS:   require.main === module
来源：http://wdm.cucudq.cn

TS:   require.main === module
来源：http://zqk.hcnkem.com

Java: public static void main(String[] args)
来源：http://lkk.daxiang520.top

Go:   func main()
来源：http://hws.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eiv.andypj.xyz

C#:   static void Main(string[] args)
来源：http://dzw.hywenlv.cn

[M08] 获取系统与运行时信息
来源：http://qif.shzxlz.cn

Py:   platform.system();  platform.python_version()
来源：http://snm.xylfe.cn

PHP:  PHP_OS;  phpversion();
来源：http://mvb.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://ebf.fktsv.cn

TS:   process.platform;  process.version
来源：http://ply.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zrw.yj20258.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tcw.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cnj.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gcd.birdmap.top

================================================================================
来源：http://vwu.tian-w.cn

N. 数据结构与算法
来源：http://els.jlsjyb.cn

================================================================================
来源：http://ype.fanxiaobao.xyz

[N01] 二分查找（有序数组）
来源：http://vfn.meibo888.top

Py:   bisect.bisect_left(arr, x)
来源：http://sji.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rdm.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fpz.ybcxt.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://idj.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://baf.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://gpq.zhaomingkeji.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://jqu.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://wdt.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://vgk.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://hxr.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pws.chenjidiqi.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://puc.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yhh.jinghuilouyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gxr.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://fii.hywenlv.cn

Ruby: arr.sort
来源：http://oiq.xylfe.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vbz.hammf.cn

[N03] 快速排序（分治示例）
来源：http://ewn.fanxiaobao.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vtt.c1oappe.top

PHP:  // 递归实现，或用 usort
来源：http://gow.sjlbkw.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ckb.cdnleiting.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pol.sxryk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lfe.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lca.316326.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bgl.yj202588.top

C#:   // 手写递归，或 Array.Sort
来源：http://fvj.cqqwz.cn

[N04] 斐波那契数列
来源：http://cpx.zhoulong.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kak.pengpengdd.cyou

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qcr.feifeiyinyue.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qol.feifeiyinyue.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pqg.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ann.jinqigfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://flp.xinyue.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iag.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://umc.jqgufenzy.top

[N05] 最大公约数
来源：http://vta.ppjwa.cn

Py:   math.gcd(a, b)
来源：http://skx.zhongyouzk.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vgq.zhijiandao.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ycb.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xsu.nanxuanxn.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hry.birdmap.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gjg.zhixingplan.top

Ruby: a.gcd(b)
来源：http://dez.zhengqikj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jlf.tian-w.cn

[N06] 判断回文字符串
来源：http://wol.zycfv.cn

Py:   s == s[::-1]
来源：http://ehi.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://dyp.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://hww.kuanghao11.cn

TS:   s === [...s].reverse().join("")
来源：http://sni.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qag.cucudq.cn

Go:   // 双指针从两端比较
来源：http://trx.ctjpmb.com

Ruby: s == s.reverse
来源：http://xll.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hiq.fehbvm.com

[N07] 两数之和（返回下标）
来源：http://joa.shangyingyoupin.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rfj.zhaomingkeji.xyz


<!-- 参考信息 -->