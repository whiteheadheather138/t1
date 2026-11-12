代发 wailian999

Go:   time.Now()
来源：http://cim.quarkkingdee.top

Ruby: Time.now
来源：http://eob.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ryv.zhijiandao.cn

[J02] 格式化输出
来源：http://pyp.haohaochexian.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bdb.jinyuanbaomall.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ubz.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dlr.zhijiandao.cn

TS:   d.toISOString()
来源：http://tbl.jinyuanbaomall.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mtl.jianghu66.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eer.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://udt.uphjek.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bwf.snrcjt.cn

[J03] 字符串解析为日期
来源：http://yxt.fanxiaobao.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jwd.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://htx.guannengcc.top

JS:   new Date("2024-01-02")
来源：http://nwg.guannengcc.top

TS:   new Date("2024-01-02")
来源：http://xcp.shzxlz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lnf.jqgfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://szb.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://cmm.fanxiaobao.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jrk.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://zoh.havefunace.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gqc.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cbv.jinghuilouyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qku.zhoulong.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://jzv.pycfn.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qtr.9152youxi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fkg.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iip.quarkkingdee.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vgj.jinghuilouyu.cn

[J05] 时间加减（加 7 天）
来源：http://bud.pycfn.com

Py:   now + timedelta(days=7)
来源：http://nri.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qnm.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ake.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xnj.hnqzz.top

Java: LocalDate.now().plusDays(7)
来源：http://ydg.ywan-chungtsiang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zwq.xylfe.cn

Ruby: Time.now + 7 * 86400
来源：http://kmi.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://mtr.smart0.xyz

[J06] 计算两时间之差
来源：http://szw.vqdsnc.cn

Py:   (end - start).total_seconds()
来源：http://ptl.jinyuanbaomall.cn

PHP:  $end->diff($start)->days;
来源：http://hpg.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yhn.quarkkingdee.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zns.ydjk.org.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xzf.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://esh.gaohongyu789.top

Ruby: end - start                 # 返回秒数
来源：http://bsv.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://rkz.havefunace.top

[J07] 比较两个日期
来源：http://bvu.hammf.cn

Py:   d1 < d2;  d1 == d2
来源：http://hxx.bjfxy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fac.9152youxi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oqu.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://kgd.tianlin.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zcg.haohaochexian.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ytk.jqgufenzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://bna.chenzaomai.com

C#:   d1 < d2;  d1 == d2
来源：http://vun.yj20258.top

[J08] 提取年月日与星期
来源：http://xuq.wangdashe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ujf.pycfn.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gah.uphjek.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dhh.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://elq.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://utt.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gax.xingfuxueyuan.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ilq.zhiwuduotai.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xsi.yvedp.cn

[J09] 时区处理
来源：http://vhf.epnwcf.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lpo.chenlongwang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gzi.vqdsnc.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jwr.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pgd.hammf.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hjj.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hle.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cdm.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zta.hnxiangtu.top

[J10] 取今天 / 本月第一天
来源：http://stx.jiagoushi.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mwh.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://azx.wangshuangyany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tdi.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://czt.sufxvd.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://usn.daxiang520.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hhf.shzxlz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tzz.sxryk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://exy.jiagoushi.top

================================================================================
来源：http://jmd.zhongyouzk.top

K. JSON 与序列化
来源：http://hgu.tanke756.top

================================================================================
来源：http://rfr.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://ugn.jqgufenzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qtn.fengsongda.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wkm.aibaodan.cn

JS:   JSON.stringify(obj)
来源：http://deb.chenzaomai.com

TS:   JSON.stringify(obj)
来源：http://bkm.epnwcf.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ftw.wangshuangyany.cn

Go:   json.Marshal(obj)
来源：http://wje.jinyuanbaomall.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lxu.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://kde.vehdjk.com

[K02] JSON 字符串转对象
来源：http://dtx.zhixingplan.top

Py:   json.loads(s)
来源：http://fmd.bjfxy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rwd.fzhhl.top

JS:   JSON.parse(s)
来源：http://cso.epnwcf.com

TS:   JSON.parse(s)
来源：http://jhw.dianchejie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hxo.zdqjudy.top

Go:   json.Unmarshal(data, &v)
来源：http://qka.xuetiantiany.cn

Ruby: JSON.parse(s)
来源：http://qyy.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qbk.wangshuangyany.cn

[K03] JSON 美化输出（带缩进）
来源：http://vey.pycfn.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hpg.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://exm.c1oappe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vmr.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://sua.zdbjq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ejd.kuanghao11.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hsl.yj202588.top

Ruby: JSON.pretty_generate(obj)
来源：http://wea.redwolf501.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://adu.cucudq.cn

[K04] 读取 JSON 文件
来源：http://rke.yvedp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vpx.hcnkem.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zwx.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dbx.xingfuxueyuan.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ofk.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jzz.aizwys.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dhy.zhoulong.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://jyx.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cxo.zhongyouzk.top

[K05] 深拷贝对象
来源：http://hgu.shuidangran.top

Py:   copy.deepcopy(obj)
来源：http://kdw.yj202588.top

PHP:  unserialize(serialize($obj));
来源：http://nth.svipenyu.cn

JS:   structuredClone(obj)
来源：http://nam.yonumen.top

TS:   structuredClone(obj)
来源：http://gtp.mhx1999.top

Java: // 手写拷贝构造，或序列化往返
来源：http://urv.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cug.jqgfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qym.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sng.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://pby.vehdjk.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ohf.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jnj.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kdt.0kj1m.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yfw.yvedp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cpl.yongpay.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ddy.shuidangran.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tnu.guowangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yah.uphjek.com

[K07] 进制转换
来源：http://rlk.hywenlv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mex.smart0.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zyu.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gsv.andypj.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oeq.gogol.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pkh.chenlongwang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rib.yueranfly.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://aew.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ddm.shanyushiyangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://zwi.guannengcc.top

Py:   pickle.dumps(obj)
来源：http://vvl.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://njy.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://vyh.vehdjk.com

TS:   v8.serialize(obj)        // Node
来源：http://xlh.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hsz.yonumen.top

Go:   encoding/gob
来源：http://zpp.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://slq.yj20258.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vpn.yuxming.cn

================================================================================
来源：http://unu.sjlbkw.cn

L. 网络请求
来源：http://pdd.vqdsnc.cn

================================================================================
来源：http://bee.ppjwa.cn

[L01] 发送 GET 请求
来源：http://aze.zhongyouzk.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cqp.cheryme.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cgt.daria6918.cn

JS:   await fetch(url)
来源：http://cat.tianlin.xyz

TS:   await fetch(url)
来源：http://qbs.ctjpmb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eol.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://yde.jqgufenzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dxd.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mjx.nanxuanxn.top

[L02] 发送 POST JSON
来源：http://qep.cqqwz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://iob.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rrk.epnwcf.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gbf.cashguo.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xxe.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tqq.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rpo.smart0.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bck.daria6918.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qqv.sufxvd.cn

[L03] 设置自定义请求头
来源：http://wah.nanxuanxn.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://err.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://emu.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qrg.xylfe.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uto.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mrl.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qjc.hongshengwenyu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ynv.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fkw.sysykeji.top

[L04] 设置超时
来源：http://hvv.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://lpn.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bpn.redwolf501.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mph.yongpay.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vpb.hesvh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cdy.yonumen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://htc.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zbq.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yvl.bbcook.cn

[L05] 上传文件（multipart）
来源：http://slx.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nsv.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://via.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cro.zhijiandao.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://etg.yuanzhike.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dwb.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hkh.xylfe.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fyl.zhongyouzk.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ghp.sxryk.cn

[L06] 解析响应为 JSON
来源：http://qyk.yuanzhike.top

Py:   resp.json()
来源：http://vbw.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://dav.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://nwo.xinyue.icu

TS:   await resp.json()
来源：http://lmd.redwolf501.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aco.tian-w.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nld.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://ski.yangfankeji.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kos.ctjpmb.com

[L07] 处理 HTTP 状态码
来源：http://qjj.shangyingyoupin.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tbv.kuanghao11.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jee.zhijiandao.cn

JS:   resp.ok;  resp.status
来源：http://lga.xinyue.icu

TS:   resp.ok;  resp.status
来源：http://luu.sjlbkw.cn

Java: resp.statusCode()
来源：http://diw.sufxvd.cn

Go:   resp.StatusCode
来源：http://zuu.tarul.cn

Ruby: resp.code.to_i
来源：http://rai.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://msz.kuanghao11.cn

[L08] 并发请求多个地址
来源：http://tpl.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hfr.zhixingplan.top

PHP:  curl_multi_init() 系列
来源：http://qmy.bjfxy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://evx.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zjo.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yqw.yuxming.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bgf.zhaomingkeji.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xmj.fengsongda.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zdl.jinyuanbaomall.cn

================================================================================
来源：http://crx.gotoacloud.top

M. 命令行 / 进程 / 环境
来源：http://vbc.zhengqikj.top

================================================================================
来源：http://yjp.ydjk.org.cn

[M01] 读取命令行参数
来源：http://zhb.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://gfu.nanxuanxn.top

PHP:  $argv;  $argc;
来源：http://gfi.aibaodan.cn

JS:   process.argv.slice(2)
来源：http://meu.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://fsx.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://zvc.xziqi.cn

Go:   os.Args[1:]
来源：http://wec.gotoacloud.top

Ruby: ARGV
来源：http://udm.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://dvo.fehbvm.com

[M02] 读取环境变量
来源：http://yyp.hongshengwenyu.top

Py:   os.environ.get("HOME")
来源：http://rga.fanxiaobao.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vvj.jinqigfzy.top

JS:   process.env.HOME
来源：http://ahb.tianlin.xyz

TS:   process.env.HOME
来源：http://szj.havefunace.top

Java: System.getenv("HOME")
来源：http://ros.chenjidiqi.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oqn.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://sym.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jfx.xuetiantiany.cn

[M03] 执行外部命令
来源：http://lbk.aibaodan.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://boa.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gnk.sjlbkw.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dee.xuetiantiany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yni.vqdsnc.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tvl.shanyushiyangtech.top

Go:   exec.Command("ls", "-l").Output()
来源：http://edu.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://fsy.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://szw.gaohongyu789.top

[M04] 获取当前工作目录
来源：http://gih.bbcook.cn

Py:   os.getcwd()
来源：http://eki.smart0.xyz

PHP:  getcwd();
来源：http://obj.yanxiufei.cn

JS:   process.cwd()
来源：http://vjt.tarul.cn

TS:   process.cwd()
来源：http://opj.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://wfb.zhaomingkeji.xyz

Go:   os.Getwd()
来源：http://jfa.gaohongyu789.top

Ruby: Dir.pwd
来源：http://kzp.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yor.fzhhl.top

[M05] 设置退出码
来源：http://zpt.zhixingplan.top

Py:   sys.exit(1)
来源：http://icg.zycfv.cn

PHP:  exit(1);
来源：http://qkw.hnqzz.top

JS:   process.exit(1)
来源：http://dfv.guowangkeji.top

TS:   process.exit(1)
来源：http://ykc.yueranfly.top

Java: System.exit(1)
来源：http://uen.iojbl.cn

Go:   os.Exit(1)
来源：http://ikb.guowangkeji.top

Ruby: exit 1
来源：http://cbi.pycfn.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jmq.shanyushiyangtech.top

[M06] 向标准错误输出
来源：http://uwl.ydzc1.top

Py:   print("err", file=sys.stderr)
来源：http://tpx.pengpengdd.cyou

PHP:  fwrite(STDERR, "err\n");
来源：http://pjs.cqqwz.cn

JS:   console.error("err")
来源：http://yvq.chenzaomai.com

TS:   console.error("err")
来源：http://xlz.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://ocn.fktsv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zqi.ehwqpu.com

Ruby: warn "err"
来源：http://kra.hysaishi.cn

C#:   Console.Error.WriteLine("err")
来源：http://tti.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://ndy.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://btb.sxryk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rta.chenjidiqi.icu

JS:   require.main === module
来源：http://yzm.sysykeji.top

TS:   require.main === module
来源：http://axg.shanyushiyangtech.top

Java: public static void main(String[] args)
来源：http://kkk.pengpengdd.cyou

Go:   func main()
来源：http://mtz.nanxuanxn.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wcf.ydzc1.top

C#:   static void Main(string[] args)
来源：http://fdd.hesvh.cn


<!-- 参考信息 -->