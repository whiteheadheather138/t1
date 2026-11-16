代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://arq.wangshuangyany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nlb.sufxvd.cn

[J09] 时区处理
来源：http://pzz.mhx1999.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://asx.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://deg.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://isw.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tfc.dashuyun.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://szc.mhx1999.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xkl.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kbn.zhixingplan.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ybt.birdmap.top

[J10] 取今天 / 本月第一天
来源：http://boa.jlsjyb.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cie.fzhhl.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yqj.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tno.bjfxy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cvr.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ypg.gzhubu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xra.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fyd.pycfn.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qzb.epnwcf.com

================================================================================
来源：http://szv.sxryk.cn

K. JSON 与序列化
来源：http://znf.sysykeji.top

================================================================================
来源：http://cbo.gogol.net.cn

[K01] 对象转 JSON 字符串
来源：http://oaf.dianchejie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gem.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fim.zhiwuduotai.top

JS:   JSON.stringify(obj)
来源：http://pqb.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://icj.ydzc1.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zqp.hcnkem.com

Go:   json.Marshal(obj)
来源：http://upg.yj20258.top

Ruby: obj.to_json                                     // require "json"
来源：http://rfw.yvedp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wtx.guannengcc.top

[K02] JSON 字符串转对象
来源：http://dma.gzhubu.top

Py:   json.loads(s)
来源：http://hzj.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://crf.cqqwz.cn

JS:   JSON.parse(s)
来源：http://kmb.sysykeji.top

TS:   JSON.parse(s)
来源：http://izb.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jze.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://oyc.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://hyz.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zdb.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://cjv.yfazqb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bsd.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qkk.shangyingyoupin.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jwe.xylfe.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vzf.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lua.zhengqikj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hsp.zdbjq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wew.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lxx.gogol.net.cn

[K04] 读取 JSON 文件
来源：http://aan.cucudq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://obw.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hkt.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pdh.yfazqb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rjj.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://czd.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://srt.zhoulong.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://ryu.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dto.bbcook.cn

[K05] 深拷贝对象
来源：http://joe.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://owy.ywan-chungtsiang.top

PHP:  unserialize(serialize($obj));
来源：http://dll.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://lft.sufxvd.cn

TS:   structuredClone(obj)
来源：http://vhg.jyoumei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dnc.xuetiantiany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bfp.dashuyun.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dad.birdmap.top

C#:   // 序列化往返，或自定义 Clone
来源：http://epk.jiagoushi.top

[K06] 解析 URL 查询串
来源：http://bcd.52xcode.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fmv.jianghu66.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ouy.nanxinkj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rio.jinqigufen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sig.havefunace.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://azv.epnwcf.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://sfj.hfpthk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hcx.52xcode.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yqm.c1oappe.top

[K07] 进制转换
来源：http://ovo.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zss.cashguo.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rwy.yuanzhike.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://och.fzhhl.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yyw.havefunace.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hlz.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://siz.iojbl.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yca.yongpay.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cao.hongshengwenyu.top

[K08] 二进制序列化（非 JSON）
来源：http://ztm.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://ifj.yuxming.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ohb.guowangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://ftk.ehwqpu.com

TS:   v8.serialize(obj)        // Node
来源：http://xcr.gzhubu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dzd.ydzc1.top

Go:   encoding/gob
来源：http://dzt.mhx1999.top

Ruby: Marshal.dump(obj)
来源：http://xph.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yce.fktsv.cn

================================================================================
来源：http://jhz.yuanzhike.top

L. 网络请求
来源：http://uut.yj202588.top

================================================================================
来源：http://sji.ywan-chungtsiang.top

[L01] 发送 GET 请求
来源：http://fpe.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uwh.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aka.zdbjq.cn

JS:   await fetch(url)
来源：http://cnn.fengsongda.top

TS:   await fetch(url)
来源：http://efp.sjlbkw.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pvc.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://jdi.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://erh.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kkq.hywenlv.cn

[L02] 发送 POST JSON
来源：http://ugv.yj202588.top

Py:   requests.post(url, json={"a": 1})
来源：http://jrt.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kig.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://agl.xingfuxueyuan.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kjf.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pjy.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cbp.c1oappe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iwr.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rqt.shzxlz.cn

[L03] 设置自定义请求头
来源：http://icl.nanxinkj.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://suk.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nor.yuxming.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gxq.xylfe.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uwq.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zvh.jinghuilouyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://icg.svipenyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ygi.dashuyun.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kqg.ehwqpu.com

[L04] 设置超时
来源：http://xju.iojbl.cn

Py:   requests.get(url, timeout=5)
来源：http://oto.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tvh.vehdjk.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ufa.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ahl.zycfv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wag.jqgfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nkj.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yhn.xylfe.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://efz.yanxiufei.cn

[L05] 上传文件（multipart）
来源：http://jvt.shuidangran.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fwo.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://idx.gogol.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qsi.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lhf.jinghuilouyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ldb.jqgufenzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oot.hcnkem.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yrh.xuanzx.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dfi.andypj.xyz

[L06] 解析响应为 JSON
来源：http://bvw.xuetiantiany.cn

Py:   resp.json()
来源：http://nbg.dashuyun.cn

PHP:  json_decode($body, true);
来源：http://rxg.bjfxy.top

JS:   await resp.json()
来源：http://uzx.ydjk.org.cn

TS:   await resp.json()
来源：http://dpr.bbcook.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ejp.yj202588.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pxj.zhoulong.xyz

Ruby: JSON.parse(resp.body)
来源：http://rik.cashguo.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iys.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://lfv.yueranfly.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pfk.ivvv.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://duy.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://lea.wangshuangyany.cn

TS:   resp.ok;  resp.status
来源：http://pjw.yuxming.cn

Java: resp.statusCode()
来源：http://bfx.52xcode.cn

Go:   resp.StatusCode
来源：http://tqi.guannengcc.top

Ruby: resp.code.to_i
来源：http://ekg.zdqjudy.top

C#:   (int)resp.StatusCode
来源：http://sfu.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://pzs.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kvp.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://stc.chenlongwang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zse.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wia.bbcook.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://txz.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dfv.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xks.tanke756.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qlk.vehdjk.com

================================================================================
来源：http://dir.jiagoushi.top

M. 命令行 / 进程 / 环境
来源：http://bya.9152youxi.cn

================================================================================
来源：http://ivy.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://oht.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://kic.ctjpmb.com

PHP:  $argv;  $argc;
来源：http://qhf.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://dff.shuidangran.top

TS:   process.argv.slice(2)
来源：http://gyw.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://yas.jinqigfzy.top

Go:   os.Args[1:]
来源：http://dni.dashuyun.cn

Ruby: ARGV
来源：http://jaw.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://hxr.jinyuanbaomall.cn

[M02] 读取环境变量
来源：http://azs.shzxlz.cn

Py:   os.environ.get("HOME")
来源：http://xda.birdmap.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://apa.smart0.xyz

JS:   process.env.HOME
来源：http://xdb.vqdsnc.cn

TS:   process.env.HOME
来源：http://rxa.tarul.cn

Java: System.getenv("HOME")
来源：http://wsh.hammf.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cso.jinqigufen.top

Ruby: ENV["HOME"]
来源：http://ppn.zycfv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pwt.feifeiyinyue.top

[M03] 执行外部命令
来源：http://gez.jqgfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uqh.hesvh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pdj.sxryk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tsu.aibaodan.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nkt.guowangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://evt.havefunace.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lax.xziqi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wnk.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://zfe.ybcxt.top

[M04] 获取当前工作目录
来源：http://rjf.yanxiufei.cn

Py:   os.getcwd()
来源：http://bpm.gzhubu.top

PHP:  getcwd();
来源：http://ypz.cheryme.top

JS:   process.cwd()
来源：http://ikq.yvedp.cn

TS:   process.cwd()
来源：http://shz.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://xmz.redwolf501.top

Go:   os.Getwd()
来源：http://pal.xingfuxueyuan.xyz

Ruby: Dir.pwd
来源：http://edk.hesvh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qki.shanyushiyangtech.top

[M05] 设置退出码
来源：http://dwo.tanke756.top

Py:   sys.exit(1)
来源：http://fvu.fzhhl.top

PHP:  exit(1);
来源：http://njj.hammf.cn

JS:   process.exit(1)
来源：http://ose.sufxvd.cn

TS:   process.exit(1)
来源：http://fkq.yonumen.top

Java: System.exit(1)
来源：http://dab.zhijiandao.cn

Go:   os.Exit(1)
来源：http://ajp.andypj.xyz

Ruby: exit 1
来源：http://afa.jiagoushi.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mei.fzhhl.top

[M06] 向标准错误输出
来源：http://eev.feifeiyinyue.top

Py:   print("err", file=sys.stderr)
来源：http://upm.wangshuangyany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dbq.cashguo.top

JS:   console.error("err")
来源：http://vew.gotoacloud.top

TS:   console.error("err")
来源：http://chz.gzhubu.top

Java: System.err.println("err")
来源：http://exe.yongpay.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yqe.svipenyu.cn

Ruby: warn "err"
来源：http://nmm.hywenlv.cn

C#:   Console.Error.WriteLine("err")
来源：http://kjn.sjlbkw.cn

[M07] 判断是否为主入口
来源：http://mvy.zdbjq.cn

Py:   if __name__ == "__main__":
来源：http://dbj.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sqs.xingfuxueyuan.xyz

JS:   require.main === module
来源：http://uji.ybcxt.top

TS:   require.main === module
来源：http://knh.epnwcf.com

Java: public static void main(String[] args)
来源：http://ksb.epnwcf.com

Go:   func main()
来源：http://gyl.chenjidiqi.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ine.shanyushiyangkeji.top

C#:   static void Main(string[] args)
来源：http://qjj.xylfe.cn

[M08] 获取系统与运行时信息
来源：http://fqy.svipenyu.cn

Py:   platform.system();  platform.python_version()
来源：http://kel.9152youxi.cn

PHP:  PHP_OS;  phpversion();
来源：http://xld.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://fyh.shuidangran.top

TS:   process.platform;  process.version
来源：http://yni.9152youxi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kzv.yj20258888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xcb.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xcg.bjfxy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bnt.aizwys.cn

================================================================================
来源：http://hsb.cqqwz.cn

N. 数据结构与算法
来源：http://qfu.chenzaomai.com

================================================================================
来源：http://rju.zycfv.cn

[N01] 二分查找（有序数组）
来源：http://add.nanxuanxn.top

Py:   bisect.bisect_left(arr, x)
来源：http://saz.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vdn.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zsg.shangyingyoupin.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dve.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bfa.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://jif.zhaomingkeji.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://eio.yj20258888.top

C#:   Array.BinarySearch(arr, x)
来源：http://ovt.nanxuanxn.top

[N02] 排序（工程实践用内置实现）
来源：http://pcz.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://kzb.shanyushiyangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iaz.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dwp.cheryme.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lrj.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xfy.hywenlv.cn

Go:   slices.Sort(arr)
来源：http://nci.jqgfzy.top

Ruby: arr.sort
来源：http://xlt.chenzaomai.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://vfl.shangyingyoupin.top

[N03] 快速排序（分治示例）
来源：http://bkb.hnxiangtu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://htt.shanyushiyangtech.top

PHP:  // 递归实现，或用 usort
来源：http://ndq.zdbjq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xbi.yueranfly.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fqu.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://btz.tanke756.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kfo.0kj1m.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://myo.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://ebx.vehdjk.com

[N04] 斐波那契数列
来源：http://waj.ivvv.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cmj.tanke756.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bwu.hfpthk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yxr.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bxb.epnwcf.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dta.birdmap.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yki.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lmy.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ebq.yfazqb.com

[N05] 最大公约数
来源：http://tyr.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://okx.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vzl.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://waq.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qtm.zhengqikj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vze.gogol.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fpw.zhiwuduotai.top

Ruby: a.gcd(b)
来源：http://nte.tarul.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ekf.9152youxi.cn

[N06] 判断回文字符串
来源：http://boq.wangdashe.top

Py:   s == s[::-1]
来源：http://iwp.chenjidiqi.icu

PHP:  $s === strrev($s);
来源：http://cfi.feifeiyinyue.top

JS:   s === [...s].reverse().join("")
来源：http://yan.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://kur.jianghu66.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yfa.yfazqb.com

Go:   // 双指针从两端比较
来源：http://wab.cashguo.top


<!-- 参考信息 -->