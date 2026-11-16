代发 wailian999

Py:   (end - start).total_seconds()
来源：http://xfw.aibaodan.cn

PHP:  $end->diff($start)->days;
来源：http://kxp.dianchejie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zwy.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://igv.jinghuilouyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vxv.jqgufenzy.top

Go:   end.Sub(start).Hours()
来源：http://peo.yuanzhike.top

Ruby: end - start                 # 返回秒数
来源：http://uiv.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://flo.zdqjudy.top

[J07] 比较两个日期
来源：http://sbp.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://uqw.cashguo.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sta.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gjx.snrcjt.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iib.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cyy.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ick.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://srp.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://wea.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://qzo.zhijiandao.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yam.sjlbkw.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gbc.zdbjq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://luj.chenlongwang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lpu.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vli.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gox.chenjidiqi.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ayl.sjlbkw.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vsl.zhixingplan.top

[J09] 时区处理
来源：http://ann.yuanzhike.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://crd.yanxiufei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vgk.cucudq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pls.jinghuilouyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qbw.pycfn.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blv.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hwo.chenlongwang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zpt.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zif.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://pmk.ehwqpu.com

Py:   date.today();  date.today().replace(day=1)
来源：http://pmm.jinqigufen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vyr.zhengqikj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ksk.shzxlz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vds.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sqm.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hre.tian-w.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://koh.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zhc.xziqi.cn

================================================================================
来源：http://mrp.jyoumei.cn

K. JSON 与序列化
来源：http://ixz.zdqjudy.top

================================================================================
来源：http://nep.jlsjyb.cn

[K01] 对象转 JSON 字符串
来源：http://mjj.zhiwuduotai.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uiy.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jny.mhx1999.top

JS:   JSON.stringify(obj)
来源：http://fjl.xinyue.icu

TS:   JSON.stringify(obj)
来源：http://haa.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xrj.hcnkem.com

Go:   json.Marshal(obj)
来源：http://wor.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://vgh.0kj1m.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sdh.cheryme.top

[K02] JSON 字符串转对象
来源：http://pcs.fehbvm.com

Py:   json.loads(s)
来源：http://dcj.zhengqikj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://evd.xylfe.cn

JS:   JSON.parse(s)
来源：http://lfb.nanxuanxn.top

TS:   JSON.parse(s)
来源：http://oef.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tnt.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://rnd.cheryme.top

Ruby: JSON.parse(s)
来源：http://xsq.yj202588.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qlh.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://bec.nwbrower.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://man.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aji.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sgr.aibaodan.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dxr.yongpay.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tlw.zhongyouzk.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uvr.chenlongwang.top

Ruby: JSON.pretty_generate(obj)
来源：http://miu.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vzy.xingfuxueyuan.xyz

[K04] 读取 JSON 文件
来源：http://wti.fehbvm.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bsm.cqqwz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nkz.ydjk.org.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xas.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iqd.zhijiandao.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ott.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tld.uphjek.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://qhq.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ceq.0kj1m.cn

[K05] 深拷贝对象
来源：http://oxn.dashuyun.cn

Py:   copy.deepcopy(obj)
来源：http://tkt.yj20258888.top

PHP:  unserialize(serialize($obj));
来源：http://amv.fehbvm.com

JS:   structuredClone(obj)
来源：http://wlp.nanxinkj.top

TS:   structuredClone(obj)
来源：http://vdf.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vgk.zdqjudy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://otq.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zot.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://uqw.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://lvw.yanxiufei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qtt.xziqi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zsf.yj20258888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gac.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://paq.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ykf.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hgg.pengpengdd.cyou

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blu.shanyushiyangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hhq.vqdsnc.cn

[K07] 进制转换
来源：http://erm.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dki.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://arf.sxryk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qfo.gaohongyu789.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eql.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bus.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fnb.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cqw.shanyushiyangtech.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vcf.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://dhe.cashguo.top

Py:   pickle.dumps(obj)
来源：http://wys.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hud.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://lao.yvedp.cn

TS:   v8.serialize(obj)        // Node
来源：http://lkf.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vok.sxryk.cn

Go:   encoding/gob
来源：http://gtb.sxryk.cn

Ruby: Marshal.dump(obj)
来源：http://bll.ppjwa.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rob.ppjwa.cn

================================================================================
来源：http://mhq.jianghu66.top

L. 网络请求
来源：http://wru.316326.xyz

================================================================================
来源：http://svw.zhixingplan.top

[L01] 发送 GET 请求
来源：http://fxj.c1oappe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dbb.birdmap.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xna.bjfxy.top

JS:   await fetch(url)
来源：http://uyv.andypj.xyz

TS:   await fetch(url)
来源：http://gad.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cmf.xinyue.icu

Go:   resp, err := http.Get(url)
来源：http://dau.zhijiandao.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jrp.ctjpmb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://skr.yuxming.cn

[L02] 发送 POST JSON
来源：http://xes.fktsv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rlj.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ocj.ivvv.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hwx.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://utv.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bqm.52xcode.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fwi.aizwys.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bjb.gotoacloud.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zkf.sjlbkw.cn

[L03] 设置自定义请求头
来源：http://pgr.jiagoushi.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kds.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jrf.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gry.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://efi.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hhw.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rhj.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xct.bbcook.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lga.vqdsnc.cn

[L04] 设置超时
来源：http://gwb.ybcxt.top

Py:   requests.get(url, timeout=5)
来源：http://coc.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uuh.sjlbkw.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gdp.aizwys.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://occ.chenjidiqi.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zyw.iojbl.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cji.hcnkem.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gkw.ehwqpu.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uxi.nwbrower.top

[L05] 上传文件（multipart）
来源：http://ltd.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lla.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ydy.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uve.meibo888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fvz.ybcxt.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://atm.chenzaomai.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jjj.tanke756.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bae.havefunace.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kxf.jinqigfzy.top

[L06] 解析响应为 JSON
来源：http://sdf.bbcook.cn

Py:   resp.json()
来源：http://kqs.tarul.cn

PHP:  json_decode($body, true);
来源：http://ogd.aizwys.cn

JS:   await resp.json()
来源：http://xuw.yfazqb.com

TS:   await resp.json()
来源：http://mvy.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kid.jinqigufen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cpu.snrcjt.cn

Ruby: JSON.parse(resp.body)
来源：http://ykr.birdmap.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ckk.zhongyouzk.top

[L07] 处理 HTTP 状态码
来源：http://tjr.shanyushiyangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://smm.kuanghao11.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wba.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://lyj.fanxiaobao.xyz

TS:   resp.ok;  resp.status
来源：http://udb.yanxiufei.cn

Java: resp.statusCode()
来源：http://xqw.mhx1999.top

Go:   resp.StatusCode
来源：http://xqa.yfazqb.com

Ruby: resp.code.to_i
来源：http://tzv.jlsjyb.cn

C#:   (int)resp.StatusCode
来源：http://ayl.chenzaomai.com

[L08] 并发请求多个地址
来源：http://ffy.dashuyun.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hgl.quarkkingdee.top

PHP:  curl_multi_init() 系列
来源：http://eui.gotoacloud.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iov.wangdashe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rfr.daxiang520.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tmk.feifeiyinyue.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zha.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://evv.tarul.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gwt.ehwqpu.com

================================================================================
来源：http://bij.sufxvd.cn

M. 命令行 / 进程 / 环境
来源：http://vvx.gzhubu.top

================================================================================
来源：http://axc.xziqi.cn

[M01] 读取命令行参数
来源：http://ecg.cheryme.top

Py:   sys.argv[1:]
来源：http://bou.fzhhl.top

PHP:  $argv;  $argc;
来源：http://seo.pycfn.com

JS:   process.argv.slice(2)
来源：http://fre.52xcode.cn

TS:   process.argv.slice(2)
来源：http://dzu.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://hyb.hongshengwenyu.top

Go:   os.Args[1:]
来源：http://kwj.xingfuxueyuan.xyz

Ruby: ARGV
来源：http://qpj.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://jfq.ctjpmb.com

[M02] 读取环境变量
来源：http://rlp.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://okh.daxiang520.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dam.cqqwz.cn

JS:   process.env.HOME
来源：http://lks.hywenlv.cn

TS:   process.env.HOME
来源：http://ovt.xylfe.cn

Java: System.getenv("HOME")
来源：http://cyv.cqqwz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kut.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://ixe.wangshuangyany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mqb.aibaodan.cn

[M03] 执行外部命令
来源：http://drm.yangfankeji.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dau.dianchejie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uan.yvedp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ens.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qqx.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zkl.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pdn.xylfe.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ilp.sxryk.cn

C#:   Process.Start("ls", "-l");
来源：http://zfw.wangdashe.top

[M04] 获取当前工作目录
来源：http://jdr.xziqi.cn

Py:   os.getcwd()
来源：http://sbo.guannengcc.top

PHP:  getcwd();
来源：http://gto.gaohongyu789.top

JS:   process.cwd()
来源：http://hvr.ehwqpu.com

TS:   process.cwd()
来源：http://fmn.shuidangran.top

Java: Path.of("").toAbsolutePath()
来源：http://ipm.cdnleiting.top

Go:   os.Getwd()
来源：http://zze.hnxiangtu.top

Ruby: Dir.pwd
来源：http://ddl.zhaomingkeji.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://gsl.kuanghao11.cn

[M05] 设置退出码
来源：http://fkd.epnwcf.com

Py:   sys.exit(1)
来源：http://inv.vqdsnc.cn

PHP:  exit(1);
来源：http://ork.jqgufenzy.top

JS:   process.exit(1)
来源：http://lge.gzhubu.top

TS:   process.exit(1)
来源：http://tyi.yueranfly.top

Java: System.exit(1)
来源：http://tvl.nanxuanxn.top

Go:   os.Exit(1)
来源：http://zqd.tarul.cn

Ruby: exit 1
来源：http://dfa.hywenlv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ggd.sysykeji.top

[M06] 向标准错误输出
来源：http://onv.sweek.top

Py:   print("err", file=sys.stderr)
来源：http://bsl.vqdsnc.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cwe.tarul.cn

JS:   console.error("err")
来源：http://ozr.pycfn.com

TS:   console.error("err")
来源：http://zpw.316326.xyz

Java: System.err.println("err")
来源：http://bch.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://giq.shuidangran.top

Ruby: warn "err"
来源：http://mpt.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://cxo.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://kyv.shuidangran.top

Py:   if __name__ == "__main__":
来源：http://uzi.nanxuanxn.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pks.zhiwuduotai.top

JS:   require.main === module
来源：http://pja.cheryme.top

TS:   require.main === module
来源：http://kym.yonumen.top

Java: public static void main(String[] args)
来源：http://cbp.sjlbkw.cn

Go:   func main()
来源：http://gib.feifeiyinyue.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yfw.wangshuangyany.cn

C#:   static void Main(string[] args)
来源：http://hls.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://dzn.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://jpo.yueranfly.top

PHP:  PHP_OS;  phpversion();
来源：http://hix.bjfxy.top

JS:   process.platform;  process.version
来源：http://vea.fanxiaobao.xyz

TS:   process.platform;  process.version
来源：http://qul.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mcb.xuanzx.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://vas.jinqigfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xnc.jinqigufen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hzn.fzhhl.top

================================================================================
来源：http://irb.fehbvm.com

N. 数据结构与算法
来源：http://wid.iojbl.cn

================================================================================
来源：http://tgg.feifeiyinyue.top

[N01] 二分查找（有序数组）
来源：http://rxp.daria6918.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jno.316326.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://whu.pengpengdd.cyou

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zcd.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wnh.zdbjq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zut.ybcxt.top

Go:   sort.SearchInts(arr, x)
来源：http://qfa.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iqr.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://ddo.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://rey.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://syt.wangdashe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nyd.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://usg.ydzc1.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ztl.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jvz.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://ukc.xuanzx.com

Ruby: arr.sort
来源：http://ela.dianchejie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sbi.yanxiufei.cn

[N03] 快速排序（分治示例）
来源：http://lxb.mhx1999.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bdu.fehbvm.com

PHP:  // 递归实现，或用 usort
来源：http://wmj.jinqigfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hfy.zhengqikj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bfu.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eqp.gzhubu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bip.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zdm.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://ggd.jianghu66.top

[N04] 斐波那契数列
来源：http://mrd.jiagoushi.top


<!-- 参考信息 -->