代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sqt.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yxj.sweek.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lmc.tian-w.cn

TS:   d.toISOString()
来源：http://kqu.feifeiyinyue.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wit.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xlg.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zoq.kuanghao11.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pqz.zhaomingkeji.xyz

[J03] 字符串解析为日期
来源：http://ngd.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lmd.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kxx.wangdashe.top

JS:   new Date("2024-01-02")
来源：http://obn.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://jsw.hnqzz.top

Java: LocalDate.parse("2024-01-02")
来源：http://hdw.xingfuxueyuan.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pin.hongshengwenyu.top

Ruby: Date.parse("2024-01-02")
来源：http://rgj.shangyingyoupin.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eyh.ehwqpu.com

[J04] 时间戳与日期互转
来源：http://qhv.tianlin.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ezd.zycfv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cnh.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ecz.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ljj.ctjpmb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://spf.sxryk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gpe.pengpengdd.cyou

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oct.pengpengdd.cyou

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://msm.jlsjyb.cn

[J05] 时间加减（加 7 天）
来源：http://ncw.sjlbkw.cn

Py:   now + timedelta(days=7)
来源：http://zpd.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fal.fehbvm.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mik.cdnleiting.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jxe.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://knw.yueranfly.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://emv.hnqzz.top

Ruby: Time.now + 7 * 86400
来源：http://cbo.zhixingplan.top

C#:   DateTime.Now.AddDays(7)
来源：http://vxu.xylfe.cn

[J06] 计算两时间之差
来源：http://nzt.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://nad.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://ohu.jinqigfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jxg.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rsl.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rrp.nwbrower.top

Go:   end.Sub(start).Hours()
来源：http://jyl.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://adt.zdbjq.cn

C#:   (end - start).TotalSeconds
来源：http://llv.fktsv.cn

[J07] 比较两个日期
来源：http://qnj.hnxiangtu.top

Py:   d1 < d2;  d1 == d2
来源：http://ntq.fzhhl.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zwb.uphjek.com

JS:   d1.getTime() < d2.getTime()
来源：http://exw.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://wkw.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bvz.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://haz.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nqw.hesvh.cn

C#:   d1 < d2;  d1 == d2
来源：http://fjs.yueranfly.top

[J08] 提取年月日与星期
来源：http://raf.fengsongda.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ima.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://itr.nanxinkj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ozl.guowangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ole.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ofj.nwbrower.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dve.svipenyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rmv.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://och.jqgfzy.top

[J09] 时区处理
来源：http://qlj.fanxiaobao.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ito.52xcode.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ayd.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zka.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ccu.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bwe.nwbrower.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://miz.dianchejie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://spq.ppjwa.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ysk.hnxiangtu.top

[J10] 取今天 / 本月第一天
来源：http://ygn.zhijiandao.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fpw.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rua.fzhhl.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tfo.yueranfly.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mis.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://asa.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kop.gzhubu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://epq.yfazqb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dbf.zdqjudy.top

================================================================================
来源：http://jzt.hfpthk.cn

K. JSON 与序列化
来源：http://wkb.dashuyun.cn

================================================================================
来源：http://jmf.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://qeg.andypj.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://igb.wangdashe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sjx.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://irb.cheryme.top

TS:   JSON.stringify(obj)
来源：http://itp.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://adq.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://rfk.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://vqr.ybcxt.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zmv.vehdjk.com

[K02] JSON 字符串转对象
来源：http://xwk.yj20258888.top

Py:   json.loads(s)
来源：http://eta.jlsjyb.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hbz.ehwqpu.com

JS:   JSON.parse(s)
来源：http://mvx.jyoumei.cn

TS:   JSON.parse(s)
来源：http://ugz.jyoumei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://itw.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://bxa.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://qny.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qpu.uphjek.com

[K03] JSON 美化输出（带缩进）
来源：http://eat.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dhg.zdbjq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pnf.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xfh.ydzc1.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vwx.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hde.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uto.jiagoushi.top

Ruby: JSON.pretty_generate(obj)
来源：http://qjv.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://snm.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://rfb.yj20258888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ewq.yuxming.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xin.yuanzhike.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tjs.kuanghao11.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://unq.shangyingyoupin.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ptx.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ojn.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gya.tanke756.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ttz.ehwqpu.com

[K05] 深拷贝对象
来源：http://byb.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://wab.fanxiaobao.xyz

PHP:  unserialize(serialize($obj));
来源：http://kkg.tian-w.cn

JS:   structuredClone(obj)
来源：http://wrt.yueranfly.top

TS:   structuredClone(obj)
来源：http://vda.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pvr.yj20258.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nsw.xuetiantiany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xur.hammf.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qtf.jianghu66.top

[K06] 解析 URL 查询串
来源：http://evp.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xnl.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tzm.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dia.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uoo.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eil.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ztt.yj20258.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tql.yongpay.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zao.tanke756.top

[K07] 进制转换
来源：http://gxc.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xbi.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://alj.ywan-chungtsiang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uzw.shzxlz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zca.zhijiandao.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hws.hammf.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iox.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vws.xuanzx.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ucw.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://srz.aibaodan.cn

Py:   pickle.dumps(obj)
来源：http://tfc.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://rrj.chenlongwang.top

JS:   v8.serialize(obj)        // Node
来源：http://oip.zhijiandao.cn

TS:   v8.serialize(obj)        // Node
来源：http://ukl.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bfw.daria6918.cn

Go:   encoding/gob
来源：http://lpt.meibo888.top

Ruby: Marshal.dump(obj)
来源：http://nbo.gogol.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xll.tianlin.xyz

================================================================================
来源：http://ris.wangdashe.top

L. 网络请求
来源：http://zip.sweek.top

================================================================================
来源：http://rfu.hywenlv.cn

[L01] 发送 GET 请求
来源：http://roj.bjfxy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://smi.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://evb.zhixingplan.top

JS:   await fetch(url)
来源：http://kls.sjlbkw.cn

TS:   await fetch(url)
来源：http://ekf.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qaa.yuxming.cn

Go:   resp, err := http.Get(url)
来源：http://zwm.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://cgv.fanxiaobao.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lrh.hfpthk.cn

[L02] 发送 POST JSON
来源：http://srh.andypj.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://eqt.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://igj.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cnl.hcnkem.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gab.havefunace.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://itz.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ncq.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wlm.jinqigufen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kmo.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://eiy.daria6918.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://koz.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kon.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bdh.hammf.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hjw.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://msb.cucudq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qxi.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vrx.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ryu.yongpay.top

[L04] 设置超时
来源：http://jal.52xcode.cn

Py:   requests.get(url, timeout=5)
来源：http://pgp.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pxf.fanxiaobao.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xra.jinyuanbaomall.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bwj.cashguo.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mzt.jinghuilouyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ttk.zdbjq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ufw.epnwcf.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tai.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://yss.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fom.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ogg.kuanghao11.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nob.tianlin.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hun.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zaf.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tev.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rfs.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rxh.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://err.gotoacloud.top

Py:   resp.json()
来源：http://wav.xylfe.cn

PHP:  json_decode($body, true);
来源：http://kdb.zdqjudy.top

JS:   await resp.json()
来源：http://plw.quarkkingdee.top

TS:   await resp.json()
来源：http://sjh.zdqjudy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rxv.shuidangran.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nxw.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://zui.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wji.yuxming.cn

[L07] 处理 HTTP 状态码
来源：http://uqx.redwolf501.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cha.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iaa.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://nvh.jianghu66.top

TS:   resp.ok;  resp.status
来源：http://yqp.nwbrower.top

Java: resp.statusCode()
来源：http://pel.cashguo.top

Go:   resp.StatusCode
来源：http://qkv.ybcxt.top

Ruby: resp.code.to_i
来源：http://lvq.316326.xyz

C#:   (int)resp.StatusCode
来源：http://suu.iojbl.cn

[L08] 并发请求多个地址
来源：http://ies.316326.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://maw.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://hgn.jqgfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rro.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pjg.cucudq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bcl.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qfb.bbcook.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yam.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hxv.cucudq.cn

================================================================================
来源：http://wwk.gaohongyu789.top

M. 命令行 / 进程 / 环境
来源：http://noe.hfpthk.cn

================================================================================
来源：http://iki.mhx1999.top

[M01] 读取命令行参数
来源：http://scf.tian-w.cn

Py:   sys.argv[1:]
来源：http://ozn.shangyingyoupin.top

PHP:  $argv;  $argc;
来源：http://cax.ybcxt.top

JS:   process.argv.slice(2)
来源：http://xkn.sysykeji.top

TS:   process.argv.slice(2)
来源：http://djn.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://ssw.sxryk.cn

Go:   os.Args[1:]
来源：http://xsn.fktsv.cn

Ruby: ARGV
来源：http://ntb.jianghu66.top

C#:   args 数组（Main 方法参数）
来源：http://yre.andypj.xyz

[M02] 读取环境变量
来源：http://szq.chenlongwang.top

Py:   os.environ.get("HOME")
来源：http://fpj.cqqwz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xpk.hywenlv.cn

JS:   process.env.HOME
来源：http://use.dianchejie.cn

TS:   process.env.HOME
来源：http://ijp.jqgfzy.top

Java: System.getenv("HOME")
来源：http://dpw.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mdj.ydzc1.top

Ruby: ENV["HOME"]
来源：http://gla.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qeq.epnwcf.com

[M03] 执行外部命令
来源：http://xzy.yuxming.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ffe.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cfq.ybcxt.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rxh.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wab.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gld.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://eza.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pzq.guowangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://kqw.zycfv.cn

[M04] 获取当前工作目录
来源：http://lpi.meibo888.top

Py:   os.getcwd()
来源：http://rqv.zhoulong.xyz

PHP:  getcwd();
来源：http://loa.ppjwa.cn

JS:   process.cwd()
来源：http://ipa.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://txb.zhengqikj.top

Java: Path.of("").toAbsolutePath()
来源：http://noo.vqdsnc.cn

Go:   os.Getwd()
来源：http://qys.havefunace.top

Ruby: Dir.pwd
来源：http://rry.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://ruo.smart0.xyz

[M05] 设置退出码
来源：http://tqn.zhijiandao.cn

Py:   sys.exit(1)
来源：http://hoz.hcnkem.com

PHP:  exit(1);
来源：http://upe.gogol.net.cn

JS:   process.exit(1)
来源：http://mcz.svipenyu.cn

TS:   process.exit(1)
来源：http://qnt.zhoulong.xyz

Java: System.exit(1)
来源：http://acc.smart0.xyz

Go:   os.Exit(1)
来源：http://zpf.zdqjudy.top

Ruby: exit 1
来源：http://tsd.jinqigfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ekx.uphjek.com

[M06] 向标准错误输出
来源：http://hub.sjlbkw.cn

Py:   print("err", file=sys.stderr)
来源：http://tmn.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ddo.gogol.net.cn

JS:   console.error("err")
来源：http://swk.zhiwuduotai.top

TS:   console.error("err")
来源：http://sku.meibo888.top

Java: System.err.println("err")
来源：http://dgt.jqgfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tco.ctjpmb.com

Ruby: warn "err"
来源：http://uwb.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://ied.hesvh.cn

[M07] 判断是否为主入口
来源：http://kud.yuanzhike.top

Py:   if __name__ == "__main__":
来源：http://qtu.bjfxy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uqo.birdmap.top

JS:   require.main === module
来源：http://hjx.guannengcc.top

TS:   require.main === module
来源：http://uem.fehbvm.com

Java: public static void main(String[] args)
来源：http://mhb.quarkkingdee.top

Go:   func main()
来源：http://raf.c1oappe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tbz.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://xvp.yongpay.top

[M08] 获取系统与运行时信息
来源：http://rhc.fanxiaobao.xyz

Py:   platform.system();  platform.python_version()
来源：http://cna.0kj1m.cn

PHP:  PHP_OS;  phpversion();
来源：http://szt.fanxiaobao.xyz

JS:   process.platform;  process.version
来源：http://thm.feifeiyinyue.top


<!-- 参考信息 -->