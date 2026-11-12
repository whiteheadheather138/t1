代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://hsb.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://ofm.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://scd.hammf.cn

C#:   (end - start).TotalSeconds
来源：http://gxq.yfazqb.com

[J07] 比较两个日期
来源：http://gjq.yuxming.cn

Py:   d1 < d2;  d1 == d2
来源：http://syq.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ltc.chenzaomai.com

JS:   d1.getTime() < d2.getTime()
来源：http://zab.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ixf.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mus.zdqjudy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pyo.ydjk.org.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hsv.yonumen.top

C#:   d1 < d2;  d1 == d2
来源：http://pci.ydzc1.top

[J08] 提取年月日与星期
来源：http://ebd.sysykeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nim.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xlf.zhijiandao.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ftc.wangshuangyany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pkz.andypj.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sql.jinghuilouyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vkz.nwbrower.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vwg.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cfr.gogol.net.cn

[J09] 时区处理
来源：http://upf.dianchejie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vhb.hywenlv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jxf.9152youxi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pzt.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sdc.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://goj.shuidangran.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://brd.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qny.316326.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lfv.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://njv.iojbl.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://blr.mhx1999.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pwm.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://igf.smart0.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tkl.hnxiangtu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wrg.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dxs.52xcode.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://adn.tanke756.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vbc.vqdsnc.cn

================================================================================
来源：http://qfg.zdbjq.cn

K. JSON 与序列化
来源：http://bed.ywan-chungtsiang.top

================================================================================
来源：http://cyy.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://nfo.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ivc.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dlf.yangfankeji.com

JS:   JSON.stringify(obj)
来源：http://brt.yj20258.top

TS:   JSON.stringify(obj)
来源：http://dyc.tian-w.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wgr.zhaomingkeji.xyz

Go:   json.Marshal(obj)
来源：http://pmg.ydzc1.top

Ruby: obj.to_json                                     // require "json"
来源：http://dmp.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gsc.daria6918.cn

[K02] JSON 字符串转对象
来源：http://qns.aibaodan.cn

Py:   json.loads(s)
来源：http://tzk.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gvb.jlsjyb.cn

JS:   JSON.parse(s)
来源：http://ahx.hywenlv.cn

TS:   JSON.parse(s)
来源：http://gfy.sjlbkw.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dpn.haohaochexian.top

Go:   json.Unmarshal(data, &v)
来源：http://wow.jinyuanbaomall.cn

Ruby: JSON.parse(s)
来源：http://yyy.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cmu.tian-w.cn

[K03] JSON 美化输出（带缩进）
来源：http://yon.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://neh.xylfe.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iph.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://aut.zhoulong.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://chx.smart0.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xef.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bms.jinqigfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://eln.nwbrower.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fyd.zdbjq.cn

[K04] 读取 JSON 文件
来源：http://uvc.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ouy.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ehu.aizwys.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xrr.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cte.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uxv.pycfn.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ryo.hammf.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ukf.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iwj.yfazqb.com

[K05] 深拷贝对象
来源：http://gkv.yongpay.top

Py:   copy.deepcopy(obj)
来源：http://cry.cqqwz.cn

PHP:  unserialize(serialize($obj));
来源：http://mqq.zhijiandao.cn

JS:   structuredClone(obj)
来源：http://kbc.hywenlv.cn

TS:   structuredClone(obj)
来源：http://vdn.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gao.fengsongda.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mlm.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://aad.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://jba.nwbrower.top

[K06] 解析 URL 查询串
来源：http://ivl.hfpthk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cfy.fanxiaobao.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oxb.hnqzz.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hmr.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vgp.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ryh.zdbjq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wyn.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zwg.nwbrower.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zan.jinyuanbaomall.cn

[K07] 进制转换
来源：http://npj.hcnkem.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://taf.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pqc.ivvv.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wet.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qdk.ydjk.org.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hzv.jinghuilouyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kcp.meibo888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kwt.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lbu.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://bol.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://rdt.vehdjk.com

PHP:  serialize($obj);  unserialize($s);
来源：http://wej.bbcook.cn

JS:   v8.serialize(obj)        // Node
来源：http://mka.sysykeji.top

TS:   v8.serialize(obj)        // Node
来源：http://qdi.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://thw.nwbrower.top

Go:   encoding/gob
来源：http://hfw.316326.xyz

Ruby: Marshal.dump(obj)
来源：http://prf.shzxlz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bdb.ywan-chungtsiang.top

================================================================================
来源：http://vmp.fanxiaobao.xyz

L. 网络请求
来源：http://zzt.jqgufenzy.top

================================================================================
来源：http://zrz.ywan-chungtsiang.top

[L01] 发送 GET 请求
来源：http://rxv.ehwqpu.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://obe.shzxlz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jea.316326.xyz

JS:   await fetch(url)
来源：http://whq.andypj.xyz

TS:   await fetch(url)
来源：http://hyv.ydzc1.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rzq.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://orb.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://moo.jqgufenzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fyy.ywan-chungtsiang.top

[L02] 发送 POST JSON
来源：http://crt.fktsv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://alg.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cvl.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yyt.yj20258.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rso.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uje.shanyushiyangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://efi.hysaishi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wbe.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rfr.hcnkem.com

[L03] 设置自定义请求头
来源：http://xuw.chenlongwang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jva.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://arn.jinyuanbaomall.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dox.yj20258.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vfx.cashguo.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lgj.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vto.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vce.0kj1m.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uyu.zdbjq.cn

[L04] 设置超时
来源：http://mod.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://jeq.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vzw.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ofi.gzhubu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kaf.jqgufenzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ihm.cashguo.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fkn.uphjek.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fjy.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wsu.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://muy.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vqh.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wsf.yuxming.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qgs.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wqt.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pir.yfazqb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nbt.meibo888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zjp.gaohongyu789.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vcp.zdqjudy.top

[L06] 解析响应为 JSON
来源：http://hzb.cdnleiting.top

Py:   resp.json()
来源：http://ubx.ybcxt.top

PHP:  json_decode($body, true);
来源：http://ujg.yongpay.top

JS:   await resp.json()
来源：http://ful.sxryk.cn

TS:   await resp.json()
来源：http://hfo.ctjpmb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://swn.daria6918.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rae.shangyingyoupin.top

Ruby: JSON.parse(resp.body)
来源：http://alu.jlsjyb.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://edo.jianghu66.top

[L07] 处理 HTTP 状态码
来源：http://dyz.yueranfly.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cbp.52xcode.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gah.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://ame.fzhhl.top

TS:   resp.ok;  resp.status
来源：http://lpb.yangfankeji.com

Java: resp.statusCode()
来源：http://xen.yj20258.top

Go:   resp.StatusCode
来源：http://bwq.sweek.top

Ruby: resp.code.to_i
来源：http://pfn.yueranfly.top

C#:   (int)resp.StatusCode
来源：http://ftr.zhixingplan.top

[L08] 并发请求多个地址
来源：http://uqu.yueranfly.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lvp.hcnkem.com

PHP:  curl_multi_init() 系列
来源：http://atu.daria6918.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aav.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qgg.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jli.ctjpmb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gwo.cdnleiting.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rgx.wangdashe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hnp.yvedp.cn

================================================================================
来源：http://zzj.gzhubu.top

M. 命令行 / 进程 / 环境
来源：http://axn.hfpthk.cn

================================================================================
来源：http://spa.iojbl.cn

[M01] 读取命令行参数
来源：http://jzu.ivvv.top

Py:   sys.argv[1:]
来源：http://dra.shzxlz.cn

PHP:  $argv;  $argc;
来源：http://wke.guowangkeji.top

JS:   process.argv.slice(2)
来源：http://qhn.yj20258.top

TS:   process.argv.slice(2)
来源：http://aoe.yj20258888.top

Java: args 数组（main 方法参数）
来源：http://pgy.yuanzhike.top

Go:   os.Args[1:]
来源：http://zoa.smart0.xyz

Ruby: ARGV
来源：http://kkf.zycfv.cn

C#:   args 数组（Main 方法参数）
来源：http://shw.zhengqikj.top

[M02] 读取环境变量
来源：http://oqz.sufxvd.cn

Py:   os.environ.get("HOME")
来源：http://vee.hammf.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ckw.guowangkeji.top

JS:   process.env.HOME
来源：http://bca.jqgufenzy.top

TS:   process.env.HOME
来源：http://myh.aibaodan.cn

Java: System.getenv("HOME")
来源：http://mps.xziqi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qtd.52xcode.cn

Ruby: ENV["HOME"]
来源：http://evi.zhixingplan.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rms.hywenlv.cn

[M03] 执行外部命令
来源：http://kvi.yj202588.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fvp.zdqjudy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cry.zdbjq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yfa.yj20258888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cvr.ydjk.org.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jiq.yueranfly.top

Go:   exec.Command("ls", "-l").Output()
来源：http://uio.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://rki.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://dzg.zycfv.cn

[M04] 获取当前工作目录
来源：http://iyb.hesvh.cn

Py:   os.getcwd()
来源：http://mnl.uphjek.com

PHP:  getcwd();
来源：http://bow.vqdsnc.cn

JS:   process.cwd()
来源：http://zdj.dianchejie.cn

TS:   process.cwd()
来源：http://tny.fktsv.cn

Java: Path.of("").toAbsolutePath()
来源：http://wqg.zdqjudy.top

Go:   os.Getwd()
来源：http://ryt.quarkkingdee.top

Ruby: Dir.pwd
来源：http://irz.hysaishi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pcw.guowangkeji.top

[M05] 设置退出码
来源：http://wbt.sufxvd.cn

Py:   sys.exit(1)
来源：http://hly.jianghu66.top

PHP:  exit(1);
来源：http://gky.xingfuxueyuan.xyz

JS:   process.exit(1)
来源：http://ith.gotoacloud.top

TS:   process.exit(1)
来源：http://yrs.fktsv.cn

Java: System.exit(1)
来源：http://dop.cheryme.top

Go:   os.Exit(1)
来源：http://cim.gotoacloud.top

Ruby: exit 1
来源：http://gtk.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kbu.zhoulong.xyz

[M06] 向标准错误输出
来源：http://iwg.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://bvo.iojbl.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://iow.bbcook.cn

JS:   console.error("err")
来源：http://yxp.yanxiufei.cn

TS:   console.error("err")
来源：http://mbf.bjfxy.top

Java: System.err.println("err")
来源：http://ret.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rmd.ybcxt.top

Ruby: warn "err"
来源：http://mge.guowangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://zsd.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://pjc.vehdjk.com

Py:   if __name__ == "__main__":
来源：http://zby.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://urn.daxiang520.top

JS:   require.main === module
来源：http://alu.hnxiangtu.top

TS:   require.main === module
来源：http://ejb.jyoumei.cn

Java: public static void main(String[] args)
来源：http://vww.haohaochexian.top

Go:   func main()
来源：http://mnv.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vfc.316326.xyz

C#:   static void Main(string[] args)
来源：http://jnl.nwbrower.top

[M08] 获取系统与运行时信息
来源：http://beu.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://wfj.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://giu.aibaodan.cn

JS:   process.platform;  process.version
来源：http://gnx.sufxvd.cn

TS:   process.platform;  process.version
来源：http://gof.yongpay.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nrg.quarkkingdee.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bct.zhiwuduotai.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://azi.xuanzx.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://wqn.jinqigufen.top

================================================================================
来源：http://knj.sjlbkw.cn

N. 数据结构与算法
来源：http://riw.sufxvd.cn

================================================================================
来源：http://nun.yueranfly.top

[N01] 二分查找（有序数组）
来源：http://kkl.meibo888.top

Py:   bisect.bisect_left(arr, x)
来源：http://cbq.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eva.pengpengdd.cyou

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qie.shanyushiyangtech.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uxf.jinghuilouyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://egc.quarkkingdee.top

Go:   sort.SearchInts(arr, x)
来源：http://lgo.haohaochexian.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://otk.jianghu66.top

C#:   Array.BinarySearch(arr, x)
来源：http://pfe.hcnkem.com

[N02] 排序（工程实践用内置实现）
来源：http://gxp.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://yyc.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hua.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mdf.dianchejie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ugx.yongpay.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pfd.xinyue.icu

Go:   slices.Sort(arr)
来源：http://rox.shangyingyoupin.top

Ruby: arr.sort
来源：http://zbs.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wtq.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://zwn.yanxiufei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mnn.fehbvm.com

PHP:  // 递归实现，或用 usort
来源：http://jls.shangyingyoupin.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nax.yfazqb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ghq.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rdp.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tmu.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eop.hysaishi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gyp.havefunace.top

[N04] 斐波那契数列
来源：http://riq.xziqi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oal.pengpengdd.cyou

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gpa.hysaishi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tjv.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xea.quarkkingdee.top


<!-- 参考信息 -->