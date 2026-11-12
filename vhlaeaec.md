代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ntn.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eqw.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jkq.jyoumei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sct.9152youxi.cn

[J03] 字符串解析为日期
来源：http://tgs.xziqi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wbc.yj202588.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ywg.mhx1999.top

JS:   new Date("2024-01-02")
来源：http://soy.xuetiantiany.cn

TS:   new Date("2024-01-02")
来源：http://xis.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://tub.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bgy.shanyushiyangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://zzz.shuidangran.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sou.jqgfzy.top

[J04] 时间戳与日期互转
来源：http://gfi.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hha.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fat.svipenyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jrp.zdqjudy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vlb.sjlbkw.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fna.jyoumei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zpb.yvedp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wnz.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xrb.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://ced.dashuyun.cn

Py:   now + timedelta(days=7)
来源：http://kbb.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ayd.xziqi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mxv.jinyuanbaomall.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xgd.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://xmr.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gnb.chenjidiqi.icu

Ruby: Time.now + 7 * 86400
来源：http://pmb.hesvh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rzk.xinyue.icu

[J06] 计算两时间之差
来源：http://cas.fktsv.cn

Py:   (end - start).total_seconds()
来源：http://vnd.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://qwl.birdmap.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kri.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xfl.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://ish.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://wzh.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://ibf.tian-w.cn

C#:   (end - start).TotalSeconds
来源：http://rpc.wangshuangyany.cn

[J07] 比较两个日期
来源：http://oor.zhijiandao.cn

Py:   d1 < d2;  d1 == d2
来源：http://efk.hywenlv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://apn.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://fkw.yvedp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zfu.redwolf501.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gdz.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mfo.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gus.gzhubu.top

C#:   d1 < d2;  d1 == d2
来源：http://nlc.chenzaomai.com

[J08] 提取年月日与星期
来源：http://gzp.ctjpmb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wxp.daria6918.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uzg.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wor.jyoumei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gxq.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rna.hongshengwenyu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fkh.tian-w.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lxw.zhoulong.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zby.chenlongwang.top

[J09] 时区处理
来源：http://zmo.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ooe.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://klm.hfpthk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tnt.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fau.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kda.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tnz.9152youxi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ffd.tian-w.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jdq.xuetiantiany.cn

[J10] 取今天 / 本月第一天
来源：http://sdi.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xio.jinghuilouyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ywd.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://poe.svipenyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ein.yanxiufei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zee.sweek.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zub.yj20258888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qbi.cucudq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wkm.xingfuxueyuan.xyz

================================================================================
来源：http://bej.fzhhl.top

K. JSON 与序列化
来源：http://nbf.hysaishi.cn

================================================================================
来源：http://qem.9152youxi.cn

[K01] 对象转 JSON 字符串
来源：http://non.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jdf.pycfn.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://obg.yfazqb.com

JS:   JSON.stringify(obj)
来源：http://ilu.316326.xyz

TS:   JSON.stringify(obj)
来源：http://kwy.zhijiandao.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pzc.ybcxt.top

Go:   json.Marshal(obj)
来源：http://pen.zhengqikj.top

Ruby: obj.to_json                                     // require "json"
来源：http://rtf.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ykx.52xcode.cn

[K02] JSON 字符串转对象
来源：http://iqo.hesvh.cn

Py:   json.loads(s)
来源：http://oau.chenjidiqi.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yjn.sweek.top

JS:   JSON.parse(s)
来源：http://vml.ywan-chungtsiang.top

TS:   JSON.parse(s)
来源：http://cwu.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jxq.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://bhz.havefunace.top

Ruby: JSON.parse(s)
来源：http://enn.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lnm.cqqwz.cn

[K03] JSON 美化输出（带缩进）
来源：http://pdh.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qcb.yfazqb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://irt.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://chv.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://loz.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wnb.nanxuanxn.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oqs.uphjek.com

Ruby: JSON.pretty_generate(obj)
来源：http://hzy.gotoacloud.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dtp.jlsjyb.cn

[K04] 读取 JSON 文件
来源：http://rrv.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cal.316326.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vvc.quarkkingdee.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lkb.bbcook.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qza.birdmap.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://otj.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rui.tanke756.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yum.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://osg.daxiang520.top

[K05] 深拷贝对象
来源：http://jzz.sysykeji.top

Py:   copy.deepcopy(obj)
来源：http://ysu.sjlbkw.cn

PHP:  unserialize(serialize($obj));
来源：http://zmn.yuxming.cn

JS:   structuredClone(obj)
来源：http://zeg.cashguo.top

TS:   structuredClone(obj)
来源：http://wrk.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://edf.ybcxt.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wjx.yfazqb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://som.hcnkem.com

C#:   // 序列化往返，或自定义 Clone
来源：http://kub.hongshengwenyu.top

[K06] 解析 URL 查询串
来源：http://yfr.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nyz.9152youxi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hye.daxiang520.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://elv.zdbjq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qpv.gaohongyu789.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dnb.jqgufenzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nhg.ywan-chungtsiang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zha.yongpay.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hhe.zhongyouzk.top

[K07] 进制转换
来源：http://yjj.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://toi.yfazqb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lhe.chenjidiqi.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ghz.jqgufenzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xin.wangdashe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ion.zdqjudy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://osa.bbcook.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nti.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xlj.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://woc.zdqjudy.top

Py:   pickle.dumps(obj)
来源：http://xse.c1oappe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ozv.dianchejie.cn

JS:   v8.serialize(obj)        // Node
来源：http://yjw.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://rig.yangfankeji.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yyb.ybcxt.top

Go:   encoding/gob
来源：http://sat.tianlin.xyz

Ruby: Marshal.dump(obj)
来源：http://uwp.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lvs.jinyuanbaomall.cn

================================================================================
来源：http://vzd.jinqigufen.top

L. 网络请求
来源：http://psx.bjfxy.top

================================================================================
来源：http://ome.316326.xyz

[L01] 发送 GET 请求
来源：http://uad.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ypj.fktsv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jnd.dianchejie.cn

JS:   await fetch(url)
来源：http://uyv.vqdsnc.cn

TS:   await fetch(url)
来源：http://lny.xylfe.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iju.hnxiangtu.top

Go:   resp, err := http.Get(url)
来源：http://pgv.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://efi.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dlf.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://bag.bbcook.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rbt.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://omf.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://itg.fktsv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zrm.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sev.redwolf501.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pmi.zhengqikj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kas.jiagoushi.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gxq.gaohongyu789.top

[L03] 设置自定义请求头
来源：http://grl.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rsi.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ewv.zhixingplan.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dmn.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hrz.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dvd.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jel.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mrr.yj20258.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nwo.vehdjk.com

[L04] 设置超时
来源：http://vcv.zhaomingkeji.xyz

Py:   requests.get(url, timeout=5)
来源：http://ovz.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hxd.fengsongda.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hkw.ctjpmb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bbt.xinyue.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wkl.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sup.fzhhl.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nwn.hfpthk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ond.bbcook.cn

[L05] 上传文件（multipart）
来源：http://phe.chenzaomai.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xks.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cph.316326.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://icf.zdqjudy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bch.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vtk.cdnleiting.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qpt.zhongyouzk.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tsh.zycfv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ftr.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://fwy.hcnkem.com

Py:   resp.json()
来源：http://ufl.daxiang520.top

PHP:  json_decode($body, true);
来源：http://fxm.jinghuilouyu.cn

JS:   await resp.json()
来源：http://yse.shuidangran.top

TS:   await resp.json()
来源：http://kfq.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vxk.hongshengwenyu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rhm.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://lon.pengpengdd.cyou

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cki.shuidangran.top

[L07] 处理 HTTP 状态码
来源：http://mnr.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://clz.ehwqpu.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://apn.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://prk.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://cpj.svipenyu.cn

Java: resp.statusCode()
来源：http://mps.aibaodan.cn

Go:   resp.StatusCode
来源：http://lfp.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://eub.yvedp.cn

C#:   (int)resp.StatusCode
来源：http://fwb.bjfxy.top

[L08] 并发请求多个地址
来源：http://lvo.zhoulong.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mhb.yonumen.top

PHP:  curl_multi_init() 系列
来源：http://dgv.jyoumei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hqp.meibo888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yry.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mmi.meibo888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ndw.shanyushiyangtech.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nur.fzhhl.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jlm.jianghu66.top

================================================================================
来源：http://cxa.meibo888.top

M. 命令行 / 进程 / 环境
来源：http://tbd.ybcxt.top

================================================================================
来源：http://hrq.yj20258.top

[M01] 读取命令行参数
来源：http://vro.aibaodan.cn

Py:   sys.argv[1:]
来源：http://sdq.mhx1999.top

PHP:  $argv;  $argc;
来源：http://ulu.vehdjk.com

JS:   process.argv.slice(2)
来源：http://lnj.jinqigfzy.top

TS:   process.argv.slice(2)
来源：http://esp.svipenyu.cn

Java: args 数组（main 方法参数）
来源：http://vvv.jinghuilouyu.cn

Go:   os.Args[1:]
来源：http://gkt.xuanzx.com

Ruby: ARGV
来源：http://cky.jqgfzy.top

C#:   args 数组（Main 方法参数）
来源：http://dlt.cucudq.cn

[M02] 读取环境变量
来源：http://sjp.zhoulong.xyz

Py:   os.environ.get("HOME")
来源：http://kto.zycfv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sbn.xinyue.icu

JS:   process.env.HOME
来源：http://iph.fanxiaobao.xyz

TS:   process.env.HOME
来源：http://pkh.wangdashe.top

Java: System.getenv("HOME")
来源：http://xiz.gaohongyu789.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uxm.yj20258888.top

Ruby: ENV["HOME"]
来源：http://ule.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jcm.sufxvd.cn

[M03] 执行外部命令
来源：http://mij.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iiu.ctjpmb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wle.snrcjt.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ldw.jinqigfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fiv.haohaochexian.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gum.xylfe.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uvc.fzhhl.top

Ruby: system("ls -l");  `ls -l`
来源：http://niz.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://hym.hnqzz.top

[M04] 获取当前工作目录
来源：http://vie.zhiwuduotai.top

Py:   os.getcwd()
来源：http://evw.zhixingplan.top

PHP:  getcwd();
来源：http://ltr.wangshuangyany.cn

JS:   process.cwd()
来源：http://uqu.zhoulong.xyz

TS:   process.cwd()
来源：http://hlf.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://chp.fzhhl.top

Go:   os.Getwd()
来源：http://vsg.redwolf501.top

Ruby: Dir.pwd
来源：http://bup.316326.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://enj.jiagoushi.top

[M05] 设置退出码
来源：http://bpc.guannengcc.top

Py:   sys.exit(1)
来源：http://imr.fzhhl.top

PHP:  exit(1);
来源：http://nph.xylfe.cn

JS:   process.exit(1)
来源：http://sww.cheryme.top

TS:   process.exit(1)
来源：http://mqp.andypj.xyz

Java: System.exit(1)
来源：http://owv.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://wlx.jyoumei.cn

Ruby: exit 1
来源：http://erg.jlsjyb.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://acv.fehbvm.com

[M06] 向标准错误输出
来源：http://smx.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://lql.redwolf501.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qgd.svipenyu.cn

JS:   console.error("err")
来源：http://iwb.0kj1m.cn

TS:   console.error("err")
来源：http://vkd.meibo888.top

Java: System.err.println("err")
来源：http://aop.wangshuangyany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ygm.hnxiangtu.top

Ruby: warn "err"
来源：http://xkl.fzhhl.top

C#:   Console.Error.WriteLine("err")
来源：http://ucw.sysykeji.top

[M07] 判断是否为主入口
来源：http://omo.shangyingyoupin.top

Py:   if __name__ == "__main__":
来源：http://yqw.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://erc.daria6918.cn

JS:   require.main === module
来源：http://bga.316326.xyz

TS:   require.main === module
来源：http://wug.zhongyouzk.top

Java: public static void main(String[] args)
来源：http://sfy.hywenlv.cn

Go:   func main()
来源：http://vge.yangfankeji.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tab.guowangkeji.top

C#:   static void Main(string[] args)
来源：http://ooo.kuanghao11.cn

[M08] 获取系统与运行时信息
来源：http://uew.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://nzn.fzhhl.top

PHP:  PHP_OS;  phpversion();
来源：http://ouz.pycfn.com

JS:   process.platform;  process.version
来源：http://sjn.sysykeji.top

TS:   process.platform;  process.version
来源：http://ffj.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zhc.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ifp.yfazqb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tgq.ybcxt.top


<!-- 参考信息 -->