代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aiq.yongpay.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vzc.xylfe.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://owm.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yjc.chenjidiqi.icu

[J03] 字符串解析为日期
来源：http://dqm.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://juy.chenjidiqi.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blw.dianchejie.cn

JS:   new Date("2024-01-02")
来源：http://cxx.chenlongwang.top

TS:   new Date("2024-01-02")
来源：http://gso.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wmm.daxiang520.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zkt.feifeiyinyue.top

Ruby: Date.parse("2024-01-02")
来源：http://gim.shangyingyoupin.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bnc.sufxvd.cn

[J04] 时间戳与日期互转
来源：http://dyj.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eao.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vmh.dianchejie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://btk.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ujl.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bim.ctjpmb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iwr.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rzd.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rzj.fengsongda.top

[J05] 时间加减（加 7 天）
来源：http://xmk.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://lds.svipenyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bju.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rkn.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xio.jqgfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://whk.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zqu.zycfv.cn

Ruby: Time.now + 7 * 86400
来源：http://xcw.nwbrower.top

C#:   DateTime.Now.AddDays(7)
来源：http://wgy.ybcxt.top

[J06] 计算两时间之差
来源：http://nwi.ctjpmb.com

Py:   (end - start).total_seconds()
来源：http://ggo.jqgufenzy.top

PHP:  $end->diff($start)->days;
来源：http://yyz.chenlongwang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ofj.andypj.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vbi.shangyingyoupin.top

Java: Duration.between(start, end).toSeconds()
来源：http://xof.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://rdw.c1oappe.top

Ruby: end - start                 # 返回秒数
来源：http://dkv.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://drl.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://rmf.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://ftx.jlsjyb.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://png.smart0.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://qfd.jinqigufen.top

TS:   d1.getTime() < d2.getTime()
来源：http://efq.zhoulong.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hek.ivvv.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qvi.hnqzz.top

Ruby: d1 < d2;  d1 == d2
来源：http://blu.shuidangran.top

C#:   d1 < d2;  d1 == d2
来源：http://hgh.zycfv.cn

[J08] 提取年月日与星期
来源：http://tqj.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gcm.bbcook.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wqq.tian-w.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wiv.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cek.yueranfly.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pog.bjfxy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zeo.mhx1999.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pjw.cucudq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zjv.ywan-chungtsiang.top

[J09] 时区处理
来源：http://uoq.havefunace.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ygu.tanke756.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vwu.jlsjyb.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://stq.yj20258888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oqr.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xyw.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://duz.chenlongwang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gib.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://puf.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://ies.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hgk.andypj.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fgh.svipenyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fxc.chenlongwang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kkv.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tnn.kuanghao11.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mom.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://grp.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yjg.tarul.cn

================================================================================
来源：http://tgd.yangfankeji.com

K. JSON 与序列化
来源：http://rvg.chenjidiqi.icu

================================================================================
来源：http://ogs.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://iul.ivvv.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ocq.hongshengwenyu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://whj.yongpay.top

JS:   JSON.stringify(obj)
来源：http://jto.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://anw.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vzn.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://zxs.sysykeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://jcq.daxiang520.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wmf.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://fxe.chenzaomai.com

Py:   json.loads(s)
来源：http://bpp.yongpay.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vnx.gzhubu.top

JS:   JSON.parse(s)
来源：http://xuk.xuanzx.com

TS:   JSON.parse(s)
来源：http://wqw.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://irj.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://wjs.0kj1m.cn

Ruby: JSON.parse(s)
来源：http://rpk.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gqe.hnxiangtu.top

[K03] JSON 美化输出（带缩进）
来源：http://hdl.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://btj.ctjpmb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://czd.tianlin.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://zvh.xylfe.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pbs.zhiwuduotai.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hen.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gac.jinqigfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://dmn.9152youxi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tck.chenlongwang.top

[K04] 读取 JSON 文件
来源：http://mch.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rqr.yuxming.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ryq.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yxx.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ceq.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ogi.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bro.smart0.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://vvz.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://foe.smart0.xyz

[K05] 深拷贝对象
来源：http://ehu.chenjidiqi.icu

Py:   copy.deepcopy(obj)
来源：http://wbm.xziqi.cn

PHP:  unserialize(serialize($obj));
来源：http://iow.yuxming.cn

JS:   structuredClone(obj)
来源：http://fif.ydzc1.top

TS:   structuredClone(obj)
来源：http://bju.jlsjyb.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://skt.xziqi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ngd.zhongyouzk.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xir.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rpd.mhx1999.top

[K06] 解析 URL 查询串
来源：http://uob.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rbi.meibo888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ciq.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uno.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zvf.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cru.316326.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://lmw.xingfuxueyuan.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rdj.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ilb.ydjk.org.cn

[K07] 进制转换
来源：http://mxc.yvedp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xyd.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gqd.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kpy.fanxiaobao.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ghm.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mcz.xinyue.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://epk.zhiwuduotai.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oyi.xuetiantiany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hqg.zhengqikj.top

[K08] 二进制序列化（非 JSON）
来源：http://qjw.havefunace.top

Py:   pickle.dumps(obj)
来源：http://nop.hammf.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ano.snrcjt.cn

JS:   v8.serialize(obj)        // Node
来源：http://ztr.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://lpz.epnwcf.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vfg.yonumen.top

Go:   encoding/gob
来源：http://otq.xingfuxueyuan.xyz

Ruby: Marshal.dump(obj)
来源：http://lhr.shanyushiyangtech.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rgx.uphjek.com

================================================================================
来源：http://ubb.aizwys.cn

L. 网络请求
来源：http://wtn.fzhhl.top

================================================================================
来源：http://nld.316326.xyz

[L01] 发送 GET 请求
来源：http://xdn.bbcook.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://igc.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://isr.havefunace.top

JS:   await fetch(url)
来源：http://yjs.yongpay.top

TS:   await fetch(url)
来源：http://ofk.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vak.sweek.top

Go:   resp, err := http.Get(url)
来源：http://pji.ybcxt.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vgc.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://woo.svipenyu.cn

[L02] 发送 POST JSON
来源：http://xzm.jinqigufen.top

Py:   requests.post(url, json={"a": 1})
来源：http://eam.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://grk.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kyo.feifeiyinyue.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vwb.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lje.tarul.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bea.birdmap.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://trl.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gno.aibaodan.cn

[L03] 设置自定义请求头
来源：http://toc.yuxming.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cxz.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rpk.cqqwz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dtx.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cxg.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hnw.hongshengwenyu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://czo.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://osv.chenjidiqi.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://miu.zdqjudy.top

[L04] 设置超时
来源：http://ypa.bjfxy.top

Py:   requests.get(url, timeout=5)
来源：http://udl.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dth.shanyushiyangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rjp.zdbjq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://urr.ybcxt.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wyf.cashguo.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yhn.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pae.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vwp.fzhhl.top

[L05] 上传文件（multipart）
来源：http://cqv.daria6918.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lpg.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://djs.shzxlz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://guk.jqgfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qeu.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tdi.52xcode.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bch.vqdsnc.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jxi.meibo888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://onu.hcnkem.com

[L06] 解析响应为 JSON
来源：http://pkt.xingfuxueyuan.xyz

Py:   resp.json()
来源：http://cog.sweek.top

PHP:  json_decode($body, true);
来源：http://yki.daria6918.cn

JS:   await resp.json()
来源：http://ock.yuanzhike.top

TS:   await resp.json()
来源：http://ujc.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mek.cucudq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pwc.nwbrower.top

Ruby: JSON.parse(resp.body)
来源：http://kvm.hnqzz.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hmu.yj202588.top

[L07] 处理 HTTP 状态码
来源：http://jhs.yongpay.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wri.aizwys.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://twp.zhengqikj.top

JS:   resp.ok;  resp.status
来源：http://lyj.hongshengwenyu.top

TS:   resp.ok;  resp.status
来源：http://dhv.tian-w.cn

Java: resp.statusCode()
来源：http://tyn.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://lyt.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://kmd.yj20258.top

C#:   (int)resp.StatusCode
来源：http://axp.tarul.cn

[L08] 并发请求多个地址
来源：http://jtp.zhoulong.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pdw.tian-w.cn

PHP:  curl_multi_init() 系列
来源：http://vmm.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zyc.nanxuanxn.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://acv.snrcjt.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kln.shuidangran.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://san.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cky.yuxming.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://slh.ywan-chungtsiang.top

================================================================================
来源：http://kph.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://zym.jqgufenzy.top

================================================================================
来源：http://amk.ydjk.org.cn

[M01] 读取命令行参数
来源：http://sxk.epnwcf.com

Py:   sys.argv[1:]
来源：http://yvy.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://djz.andypj.xyz

JS:   process.argv.slice(2)
来源：http://qbq.tian-w.cn

TS:   process.argv.slice(2)
来源：http://pob.zhoulong.xyz

Java: args 数组（main 方法参数）
来源：http://lte.birdmap.top

Go:   os.Args[1:]
来源：http://pjv.nanxuanxn.top

Ruby: ARGV
来源：http://gnt.shanyushiyangtech.top

C#:   args 数组（Main 方法参数）
来源：http://kcu.ybcxt.top

[M02] 读取环境变量
来源：http://xkt.chenjidiqi.icu

Py:   os.environ.get("HOME")
来源：http://yvk.ctjpmb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uos.zdbjq.cn

JS:   process.env.HOME
来源：http://juw.daxiang520.top

TS:   process.env.HOME
来源：http://mwd.ywan-chungtsiang.top

Java: System.getenv("HOME")
来源：http://iov.zhengqikj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://npu.shuidangran.top

Ruby: ENV["HOME"]
来源：http://mmd.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cua.52xcode.cn

[M03] 执行外部命令
来源：http://vle.tarul.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mzb.yongpay.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://htg.mhx1999.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nql.jlsjyb.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hbu.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dbm.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uae.haohaochexian.top

Ruby: system("ls -l");  `ls -l`
来源：http://eeq.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://dfs.fzhhl.top

[M04] 获取当前工作目录
来源：http://nao.redwolf501.top

Py:   os.getcwd()
来源：http://taa.ydzc1.top

PHP:  getcwd();
来源：http://fvo.ppjwa.cn

JS:   process.cwd()
来源：http://ueu.ybcxt.top

TS:   process.cwd()
来源：http://gli.birdmap.top

Java: Path.of("").toAbsolutePath()
来源：http://ibb.feifeiyinyue.top

Go:   os.Getwd()
来源：http://vsq.guannengcc.top

Ruby: Dir.pwd
来源：http://mvb.ywan-chungtsiang.top

C#:   Directory.GetCurrentDirectory()
来源：http://khd.chenjidiqi.icu

[M05] 设置退出码
来源：http://ank.bjfxy.top

Py:   sys.exit(1)
来源：http://yil.jlsjyb.cn

PHP:  exit(1);
来源：http://nvq.cdnleiting.top

JS:   process.exit(1)
来源：http://xus.shuidangran.top

TS:   process.exit(1)
来源：http://jzi.fzhhl.top

Java: System.exit(1)
来源：http://dtr.hysaishi.cn

Go:   os.Exit(1)
来源：http://dmy.havefunace.top

Ruby: exit 1
来源：http://cer.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://owb.nanxinkj.top

[M06] 向标准错误输出
来源：http://iqc.redwolf501.top

Py:   print("err", file=sys.stderr)
来源：http://xdc.quarkkingdee.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cym.ctjpmb.com

JS:   console.error("err")
来源：http://ubp.daxiang520.top

TS:   console.error("err")
来源：http://mln.sysykeji.top

Java: System.err.println("err")
来源：http://bte.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yqg.hywenlv.cn

Ruby: warn "err"
来源：http://qti.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://xko.cheryme.top

[M07] 判断是否为主入口
来源：http://fax.wangdashe.top

Py:   if __name__ == "__main__":
来源：http://tjg.uphjek.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://alm.hnqzz.top

JS:   require.main === module
来源：http://ooq.shanyushiyangtech.top

TS:   require.main === module
来源：http://sqg.xziqi.cn

Java: public static void main(String[] args)
来源：http://bbq.wangdashe.top

Go:   func main()
来源：http://ixj.shuidangran.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cco.daxiang520.top

C#:   static void Main(string[] args)
来源：http://ozk.uphjek.com

[M08] 获取系统与运行时信息
来源：http://ibt.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://zpc.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://bxi.jiagoushi.top

JS:   process.platform;  process.version
来源：http://fwz.ctjpmb.com

TS:   process.platform;  process.version
来源：http://fvs.zhoulong.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lnv.guannengcc.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://iwm.yangfankeji.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dfs.ydzc1.top


<!-- 参考信息 -->