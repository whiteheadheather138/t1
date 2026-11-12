代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jjo.zhiwuduotai.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dcg.fengsongda.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lod.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nmu.jqgufenzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xgm.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://auy.yanxiufei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hva.mhx1999.top

[J10] 取今天 / 本月第一天
来源：http://lau.yanxiufei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nun.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ftp.yanxiufei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ett.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dto.tarul.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vgg.shangyingyoupin.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ccn.0kj1m.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sns.yanxiufei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hwv.hesvh.cn

================================================================================
来源：http://hat.ppjwa.cn

K. JSON 与序列化
来源：http://ztx.shuidangran.top

================================================================================
来源：http://fwk.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://bvx.chenjidiqi.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gir.mhx1999.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://skd.ydjk.org.cn

JS:   JSON.stringify(obj)
来源：http://end.xingfuxueyuan.xyz

TS:   JSON.stringify(obj)
来源：http://fyu.cheryme.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baf.tianlin.xyz

Go:   json.Marshal(obj)
来源：http://awy.hongshengwenyu.top

Ruby: obj.to_json                                     // require "json"
来源：http://lab.shzxlz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cle.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://jbv.jinghuilouyu.cn

Py:   json.loads(s)
来源：http://srx.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://asp.hnqzz.top

JS:   JSON.parse(s)
来源：http://qvm.nanxuanxn.top

TS:   JSON.parse(s)
来源：http://ees.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fhf.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://iwk.ydzc1.top

Ruby: JSON.parse(s)
来源：http://hah.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rwv.haohaochexian.top

[K03] JSON 美化输出（带缩进）
来源：http://kvn.ydjk.org.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bna.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ooj.pycfn.com

JS:   JSON.stringify(obj, null, 2)
来源：http://xvn.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://tsy.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iqf.jqgfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hvi.cheryme.top

Ruby: JSON.pretty_generate(obj)
来源：http://pda.hywenlv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nun.zycfv.cn

[K04] 读取 JSON 文件
来源：http://swu.yangfankeji.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tat.chenjidiqi.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jre.c1oappe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xxo.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ezk.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hkk.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nwm.iojbl.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gpd.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nhe.mhx1999.top

[K05] 深拷贝对象
来源：http://inf.cucudq.cn

Py:   copy.deepcopy(obj)
来源：http://brm.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://cun.guowangkeji.top

JS:   structuredClone(obj)
来源：http://rly.hcnkem.com

TS:   structuredClone(obj)
来源：http://xgw.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nvt.snrcjt.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vsv.zycfv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zmo.hammf.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fwz.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://cvk.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qdj.ybcxt.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uzm.tarul.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vbh.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://prp.ehwqpu.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kts.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nww.fktsv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nnj.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uxp.mhx1999.top

[K07] 进制转换
来源：http://hfk.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kzh.sxryk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fly.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dcc.hysaishi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mgq.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nlz.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jrg.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://apl.jinqigufen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vzd.hnqzz.top

[K08] 二进制序列化（非 JSON）
来源：http://dxt.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://mxp.hywenlv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ehg.nanxuanxn.top

JS:   v8.serialize(obj)        // Node
来源：http://uoc.feifeiyinyue.top

TS:   v8.serialize(obj)        // Node
来源：http://byp.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zzt.bbcook.cn

Go:   encoding/gob
来源：http://psj.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://buu.9152youxi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yjv.haohaochexian.top

================================================================================
来源：http://csc.yuanzhike.top

L. 网络请求
来源：http://ail.cqqwz.cn

================================================================================
来源：http://awf.fzhhl.top

[L01] 发送 GET 请求
来源：http://fwf.hfpthk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rtq.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pms.jiagoushi.top

JS:   await fetch(url)
来源：http://yve.epnwcf.com

TS:   await fetch(url)
来源：http://zuu.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://flz.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://dhy.vqdsnc.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fhf.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nno.tarul.cn

[L02] 发送 POST JSON
来源：http://cjh.hongshengwenyu.top

Py:   requests.post(url, json={"a": 1})
来源：http://lgm.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lrk.ehwqpu.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://swq.redwolf501.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fqb.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bng.xuanzx.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tht.meibo888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ipu.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cfk.gaohongyu789.top

[L03] 设置自定义请求头
来源：http://wso.yueranfly.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eqv.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cww.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yfp.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fpx.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jvd.cdnleiting.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wve.aibaodan.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dnc.guowangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://snz.guannengcc.top

[L04] 设置超时
来源：http://wbx.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://fuk.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bhr.cucudq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://swz.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rrg.jyoumei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hqu.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ini.jyoumei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aba.cheryme.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lyu.redwolf501.top

[L05] 上传文件（multipart）
来源：http://hks.havefunace.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://npk.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bdk.shanyushiyangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hdg.mhx1999.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://osh.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dgc.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oru.jinghuilouyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://crf.ywan-chungtsiang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gzl.uphjek.com

[L06] 解析响应为 JSON
来源：http://cfr.fehbvm.com

Py:   resp.json()
来源：http://hzd.daria6918.cn

PHP:  json_decode($body, true);
来源：http://wgt.xingfuxueyuan.xyz

JS:   await resp.json()
来源：http://avy.pycfn.com

TS:   await resp.json()
来源：http://ueu.zhoulong.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hvu.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aqj.guannengcc.top

Ruby: JSON.parse(resp.body)
来源：http://bpm.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yif.aizwys.cn

[L07] 处理 HTTP 状态码
来源：http://rvb.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fnu.redwolf501.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sqr.yfazqb.com

JS:   resp.ok;  resp.status
来源：http://wwx.hammf.cn

TS:   resp.ok;  resp.status
来源：http://yyh.hcnkem.com

Java: resp.statusCode()
来源：http://sva.shuidangran.top

Go:   resp.StatusCode
来源：http://ush.chenjidiqi.icu

Ruby: resp.code.to_i
来源：http://toj.yongpay.top

C#:   (int)resp.StatusCode
来源：http://gwj.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://jja.iojbl.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uvz.ehwqpu.com

PHP:  curl_multi_init() 系列
来源：http://kqs.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ovg.ppjwa.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ksu.cheryme.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eas.aibaodan.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xwz.quarkkingdee.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lec.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zot.xingfuxueyuan.xyz

================================================================================
来源：http://fau.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://mfr.zhiwuduotai.top

================================================================================
来源：http://jhy.ehwqpu.com

[M01] 读取命令行参数
来源：http://pmd.zhijiandao.cn

Py:   sys.argv[1:]
来源：http://dmb.daxiang520.top

PHP:  $argv;  $argc;
来源：http://qff.zdbjq.cn

JS:   process.argv.slice(2)
来源：http://dkw.andypj.xyz

TS:   process.argv.slice(2)
来源：http://bpx.zhijiandao.cn

Java: args 数组（main 方法参数）
来源：http://dvy.shanyushiyangkeji.top

Go:   os.Args[1:]
来源：http://lxt.ppjwa.cn

Ruby: ARGV
来源：http://jav.cheryme.top

C#:   args 数组（Main 方法参数）
来源：http://dor.hysaishi.cn

[M02] 读取环境变量
来源：http://scm.wangshuangyany.cn

Py:   os.environ.get("HOME")
来源：http://xpy.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ple.hesvh.cn

JS:   process.env.HOME
来源：http://qzu.hammf.cn

TS:   process.env.HOME
来源：http://xbh.birdmap.top

Java: System.getenv("HOME")
来源：http://men.sufxvd.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ets.hysaishi.cn

Ruby: ENV["HOME"]
来源：http://jyw.fehbvm.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sap.jianghu66.top

[M03] 执行外部命令
来源：http://sjn.bbcook.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://esn.yj20258.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://duw.zdbjq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pxn.hnqzz.top

TS:   child_process.execSync("ls -l").toString()
来源：http://asd.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://idi.xingfuxueyuan.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://bmw.bjfxy.top

Ruby: system("ls -l");  `ls -l`
来源：http://cav.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://tjy.xuanzx.com

[M04] 获取当前工作目录
来源：http://rpi.yuxming.cn

Py:   os.getcwd()
来源：http://ixy.svipenyu.cn

PHP:  getcwd();
来源：http://pbu.yonumen.top

JS:   process.cwd()
来源：http://jcg.hcnkem.com

TS:   process.cwd()
来源：http://xkq.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://adx.svipenyu.cn

Go:   os.Getwd()
来源：http://nlm.hesvh.cn

Ruby: Dir.pwd
来源：http://lcr.xingfuxueyuan.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://yuq.hfpthk.cn

[M05] 设置退出码
来源：http://bjx.cqqwz.cn

Py:   sys.exit(1)
来源：http://gfq.meibo888.top

PHP:  exit(1);
来源：http://fbu.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://rbo.yj202588.top

TS:   process.exit(1)
来源：http://lng.cashguo.top

Java: System.exit(1)
来源：http://hvd.ybcxt.top

Go:   os.Exit(1)
来源：http://gix.hammf.cn

Ruby: exit 1
来源：http://ado.sweek.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bhb.zhongyouzk.top

[M06] 向标准错误输出
来源：http://lpp.yj202588.top

Py:   print("err", file=sys.stderr)
来源：http://vst.jlsjyb.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sij.xuanzx.com

JS:   console.error("err")
来源：http://mqv.shangyingyoupin.top

TS:   console.error("err")
来源：http://dkf.svipenyu.cn

Java: System.err.println("err")
来源：http://eve.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qur.dashuyun.cn

Ruby: warn "err"
来源：http://bvm.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://tgz.yj20258.top

[M07] 判断是否为主入口
来源：http://exi.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://fyh.hcnkem.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wqv.tarul.cn

JS:   require.main === module
来源：http://mlx.hywenlv.cn

TS:   require.main === module
来源：http://wrf.hammf.cn

Java: public static void main(String[] args)
来源：http://ptq.jyoumei.cn

Go:   func main()
来源：http://mke.yangfankeji.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ugi.pycfn.com

C#:   static void Main(string[] args)
来源：http://kyu.fengsongda.top

[M08] 获取系统与运行时信息
来源：http://qlh.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://pxv.pengpengdd.cyou

PHP:  PHP_OS;  phpversion();
来源：http://dij.jlsjyb.cn

JS:   process.platform;  process.version
来源：http://iwp.ehwqpu.com

TS:   process.platform;  process.version
来源：http://eml.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rga.shanyushiyangtech.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jsy.ywan-chungtsiang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://emy.yvedp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jut.wangshuangyany.cn

================================================================================
来源：http://rxf.shzxlz.cn

N. 数据结构与算法
来源：http://rjv.hammf.cn

================================================================================
来源：http://vvj.guannengcc.top

[N01] 二分查找（有序数组）
来源：http://ecd.tanke756.top

Py:   bisect.bisect_left(arr, x)
来源：http://apc.vqdsnc.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xmb.aizwys.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tfd.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zyp.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://qvn.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://bow.dianchejie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ovg.zhoulong.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://hmy.jyoumei.cn

[N02] 排序（工程实践用内置实现）
来源：http://uby.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://gdp.epnwcf.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hlu.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://xea.52xcode.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hpi.shanyushiyangtech.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fnq.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://zqa.dashuyun.cn

Ruby: arr.sort
来源：http://sld.gogol.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cgl.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://tgw.cdnleiting.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zeo.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://shf.xylfe.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hnr.316326.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gad.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qrv.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://khi.hammf.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mcz.fengsongda.top

C#:   // 手写递归，或 Array.Sort
来源：http://lda.xziqi.cn

[N04] 斐波那契数列
来源：http://srl.nanxuanxn.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gjf.yueranfly.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://awd.52xcode.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wmj.chenzaomai.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fie.sufxvd.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jov.ybcxt.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://faa.wangshuangyany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rsk.hesvh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://juw.haohaochexian.top

[N05] 最大公约数
来源：http://qsa.cdnleiting.top

Py:   math.gcd(a, b)
来源：http://dlh.dianchejie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qmi.jianghu66.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kcr.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rmf.pengpengdd.cyou

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mcb.hammf.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wwv.tarul.cn

Ruby: a.gcd(b)
来源：http://lww.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cau.chenzaomai.com

[N06] 判断回文字符串
来源：http://jih.chenlongwang.top

Py:   s == s[::-1]
来源：http://snd.cucudq.cn

PHP:  $s === strrev($s);
来源：http://log.ybcxt.top

JS:   s === [...s].reverse().join("")
来源：http://oqe.zhengqikj.top

TS:   s === [...s].reverse().join("")
来源：http://gdw.iojbl.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nbx.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://igg.pycfn.com

Ruby: s == s.reverse
来源：http://tfs.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xkp.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://hms.andypj.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pom.fengsongda.top


<!-- 参考信息 -->