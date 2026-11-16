代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gqt.vqdsnc.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://txg.yueranfly.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://brl.pengpengdd.cyou

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tub.zhoulong.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://grd.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fas.jiagoushi.top

[J05] 时间加减（加 7 天）
来源：http://wuz.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://yyl.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fph.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://owo.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://afi.jiagoushi.top

Java: LocalDate.now().plusDays(7)
来源：http://yul.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://thu.yj20258.top

Ruby: Time.now + 7 * 86400
来源：http://crc.hfpthk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pcm.cashguo.top

[J06] 计算两时间之差
来源：http://gre.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://yow.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://qci.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kfa.9152youxi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xzj.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://jub.sweek.top

Go:   end.Sub(start).Hours()
来源：http://svl.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://ljk.9152youxi.cn

C#:   (end - start).TotalSeconds
来源：http://ouu.fktsv.cn

[J07] 比较两个日期
来源：http://bck.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://pne.daria6918.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tqw.epnwcf.com

JS:   d1.getTime() < d2.getTime()
来源：http://qir.tianlin.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://vrf.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://toc.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bgw.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sdn.chenjidiqi.icu

C#:   d1 < d2;  d1 == d2
来源：http://xph.ivvv.top

[J08] 提取年月日与星期
来源：http://skk.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ltr.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nrq.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gzm.yj20258.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vdg.wangshuangyany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://evv.yonumen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qzu.jianghu66.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lfv.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://orq.jinyuanbaomall.cn

[J09] 时区处理
来源：http://tbu.yuanzhike.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qlv.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hze.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jfa.shuidangran.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xgh.hesvh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eep.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vgu.jlsjyb.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pnd.ydjk.org.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xfe.ppjwa.cn

[J10] 取今天 / 本月第一天
来源：http://gub.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vqi.fzhhl.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dxh.feifeiyinyue.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qdm.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zcf.jinqigufen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ykb.yueranfly.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://siv.yonumen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wlz.yanxiufei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://joh.nanxinkj.top

================================================================================
来源：http://czz.yonumen.top

K. JSON 与序列化
来源：http://wfm.fehbvm.com

================================================================================
来源：http://sgi.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://dpj.zycfv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mfk.52xcode.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hca.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://jbn.ppjwa.cn

TS:   JSON.stringify(obj)
来源：http://gnr.hesvh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aef.gzhubu.top

Go:   json.Marshal(obj)
来源：http://zpr.chenjidiqi.icu

Ruby: obj.to_json                                     // require "json"
来源：http://mvj.smart0.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://tjv.hammf.cn

[K02] JSON 字符串转对象
来源：http://ljc.yfazqb.com

Py:   json.loads(s)
来源：http://wdd.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lwh.aizwys.cn

JS:   JSON.parse(s)
来源：http://ywg.jqgfzy.top

TS:   JSON.parse(s)
来源：http://tby.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://upa.kuanghao11.cn

Go:   json.Unmarshal(data, &v)
来源：http://jfw.shuidangran.top

Ruby: JSON.parse(s)
来源：http://jal.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yuf.shuidangran.top

[K03] JSON 美化输出（带缩进）
来源：http://foj.yongpay.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rje.hywenlv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nco.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://dzz.shanyushiyangtech.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hsc.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rfm.vehdjk.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://myq.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://gps.hammf.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tqu.52xcode.cn

[K04] 读取 JSON 文件
来源：http://eds.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zhk.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://maq.feifeiyinyue.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hih.shzxlz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dbc.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pvp.ctjpmb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zzd.ybcxt.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pow.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://doc.fzhhl.top

[K05] 深拷贝对象
来源：http://uhq.cheryme.top

Py:   copy.deepcopy(obj)
来源：http://pcu.hnxiangtu.top

PHP:  unserialize(serialize($obj));
来源：http://ugp.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://atn.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://bvp.wangshuangyany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hxt.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tdn.hongshengwenyu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dfp.fzhhl.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yoy.zdqjudy.top

[K06] 解析 URL 查询串
来源：http://ylm.mhx1999.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://idp.gotoacloud.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hck.shzxlz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jly.quarkkingdee.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ljp.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mur.yanxiufei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wnk.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://joj.jqgfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fss.jinyuanbaomall.cn

[K07] 进制转换
来源：http://phn.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pcf.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vrv.sufxvd.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aof.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://abo.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mtg.nanxinkj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pgi.cqqwz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kax.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ebl.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://vgx.nwbrower.top

Py:   pickle.dumps(obj)
来源：http://tcr.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kqn.birdmap.top

JS:   v8.serialize(obj)        // Node
来源：http://mqz.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://qug.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bzp.hysaishi.cn

Go:   encoding/gob
来源：http://oos.yuanzhike.top

Ruby: Marshal.dump(obj)
来源：http://wzg.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lwn.gzhubu.top

================================================================================
来源：http://xrq.gzhubu.top

L. 网络请求
来源：http://dof.yongpay.top

================================================================================
来源：http://kip.xylfe.cn

[L01] 发送 GET 请求
来源：http://kqv.kuanghao11.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ueb.fktsv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rrb.aizwys.cn

JS:   await fetch(url)
来源：http://hwi.zycfv.cn

TS:   await fetch(url)
来源：http://ghf.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pfj.yueranfly.top

Go:   resp, err := http.Get(url)
来源：http://fkb.ydjk.org.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mgk.pycfn.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vrk.yj202588.top

[L02] 发送 POST JSON
来源：http://awk.shangyingyoupin.top

Py:   requests.post(url, json={"a": 1})
来源：http://jdi.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vkg.cqqwz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dxp.haohaochexian.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dec.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ydr.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pmc.quarkkingdee.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oiv.ydjk.org.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mhz.cqqwz.cn

[L03] 设置自定义请求头
来源：http://ujn.yj20258888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tcd.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kzs.hfpthk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xka.shuidangran.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ydx.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mgl.cucudq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yzu.c1oappe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rsq.zhixingplan.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jxw.pycfn.com

[L04] 设置超时
来源：http://dqg.hysaishi.cn

Py:   requests.get(url, timeout=5)
来源：http://yfm.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eyq.yfazqb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yjs.sweek.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kdr.jlsjyb.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pom.jiagoushi.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wqw.meibo888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zvn.zhiwuduotai.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://unw.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://ivt.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ovc.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uwf.haohaochexian.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dbd.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kqk.vqdsnc.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mnw.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iba.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nca.zhongyouzk.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kgr.316326.xyz

[L06] 解析响应为 JSON
来源：http://jql.chenjidiqi.icu

Py:   resp.json()
来源：http://qjh.andypj.xyz

PHP:  json_decode($body, true);
来源：http://uzk.chenlongwang.top

JS:   await resp.json()
来源：http://nge.yj20258888.top

TS:   await resp.json()
来源：http://tlf.chenzaomai.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wxx.ywan-chungtsiang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jxb.fengsongda.top

Ruby: JSON.parse(resp.body)
来源：http://hhw.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ant.yuxming.cn

[L07] 处理 HTTP 状态码
来源：http://cut.bjfxy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://whj.tarul.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tuz.fanxiaobao.xyz

JS:   resp.ok;  resp.status
来源：http://xqk.hnxiangtu.top

TS:   resp.ok;  resp.status
来源：http://xtf.316326.xyz

Java: resp.statusCode()
来源：http://tly.zhengqikj.top

Go:   resp.StatusCode
来源：http://mkh.bjfxy.top

Ruby: resp.code.to_i
来源：http://cma.aibaodan.cn

C#:   (int)resp.StatusCode
来源：http://tur.cheryme.top

[L08] 并发请求多个地址
来源：http://zcd.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rev.shuidangran.top

PHP:  curl_multi_init() 系列
来源：http://rdc.aizwys.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hkk.hnxiangtu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hdn.ywan-chungtsiang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vme.sjlbkw.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bpj.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://avs.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wot.andypj.xyz

================================================================================
来源：http://pxe.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://gxn.jinqigufen.top

================================================================================
来源：http://rez.xinyue.icu

[M01] 读取命令行参数
来源：http://stn.xinyue.icu

Py:   sys.argv[1:]
来源：http://ubo.daria6918.cn

PHP:  $argv;  $argc;
来源：http://llj.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://xbe.bjfxy.top

TS:   process.argv.slice(2)
来源：http://rkw.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://ynw.aibaodan.cn

Go:   os.Args[1:]
来源：http://yls.fehbvm.com

Ruby: ARGV
来源：http://tox.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://anv.chenzaomai.com

[M02] 读取环境变量
来源：http://ley.tianlin.xyz

Py:   os.environ.get("HOME")
来源：http://wnd.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ktj.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://ogp.yfazqb.com

TS:   process.env.HOME
来源：http://odp.jinghuilouyu.cn

Java: System.getenv("HOME")
来源：http://flq.zhongyouzk.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xhd.svipenyu.cn

Ruby: ENV["HOME"]
来源：http://cvt.cucudq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://onm.quarkkingdee.top

[M03] 执行外部命令
来源：http://orq.iojbl.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mdb.hywenlv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rex.ybcxt.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xzu.jlsjyb.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nlf.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ccx.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gqa.hnxiangtu.top

Ruby: system("ls -l");  `ls -l`
来源：http://fcd.haohaochexian.top

C#:   Process.Start("ls", "-l");
来源：http://owa.chenlongwang.top

[M04] 获取当前工作目录
来源：http://zgq.jyoumei.cn

Py:   os.getcwd()
来源：http://jsx.fzhhl.top

PHP:  getcwd();
来源：http://aik.yuxming.cn

JS:   process.cwd()
来源：http://lmh.jinghuilouyu.cn

TS:   process.cwd()
来源：http://wkt.52xcode.cn

Java: Path.of("").toAbsolutePath()
来源：http://cmp.hcnkem.com

Go:   os.Getwd()
来源：http://coj.ehwqpu.com

Ruby: Dir.pwd
来源：http://yph.shanyushiyangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://cvd.c1oappe.top

[M05] 设置退出码
来源：http://eia.hesvh.cn

Py:   sys.exit(1)
来源：http://rhb.shzxlz.cn

PHP:  exit(1);
来源：http://hqv.yj20258.top

JS:   process.exit(1)
来源：http://qkp.jinqigufen.top

TS:   process.exit(1)
来源：http://mpw.smart0.xyz

Java: System.exit(1)
来源：http://wqa.feifeiyinyue.top

Go:   os.Exit(1)
来源：http://oqz.tanke756.top

Ruby: exit 1
来源：http://xhs.jyoumei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hbq.shuidangran.top

[M06] 向标准错误输出
来源：http://rrl.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://kbo.ydzc1.top

PHP:  fwrite(STDERR, "err\n");
来源：http://euj.guowangkeji.top

JS:   console.error("err")
来源：http://iul.cheryme.top

TS:   console.error("err")
来源：http://vzm.vqdsnc.cn

Java: System.err.println("err")
来源：http://syy.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://efz.ppjwa.cn

Ruby: warn "err"
来源：http://sui.dianchejie.cn

C#:   Console.Error.WriteLine("err")
来源：http://jup.wangshuangyany.cn

[M07] 判断是否为主入口
来源：http://ird.vehdjk.com

Py:   if __name__ == "__main__":
来源：http://ymb.hnxiangtu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bqd.shanyushiyangkeji.top

JS:   require.main === module
来源：http://usk.c1oappe.top

TS:   require.main === module
来源：http://yql.cashguo.top

Java: public static void main(String[] args)
来源：http://zsu.gotoacloud.top

Go:   func main()
来源：http://nnb.gzhubu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mnq.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://dfz.yuxming.cn

[M08] 获取系统与运行时信息
来源：http://qaw.zhaomingkeji.xyz

Py:   platform.system();  platform.python_version()
来源：http://mfa.xingfuxueyuan.xyz

PHP:  PHP_OS;  phpversion();
来源：http://bvb.jianghu66.top

JS:   process.platform;  process.version
来源：http://yye.jyoumei.cn

TS:   process.platform;  process.version
来源：http://xya.nanxinkj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uju.hammf.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yom.fanxiaobao.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dcd.zhoulong.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://syk.zhijiandao.cn

================================================================================
来源：http://lpl.cheryme.top

N. 数据结构与算法
来源：http://ndv.guannengcc.top

================================================================================
来源：http://qtv.cdnleiting.top

[N01] 二分查找（有序数组）
来源：http://fqp.xziqi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://klr.nwbrower.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wxx.cucudq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ydt.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ffj.ehwqpu.com

Java: Arrays.binarySearch(arr, x)
来源：http://kup.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://tlz.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rwm.sweek.top

C#:   Array.BinarySearch(arr, x)
来源：http://xgz.jinghuilouyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://mfk.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://yhf.andypj.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cal.jyoumei.cn


<!-- 参考信息 -->