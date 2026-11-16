代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tfr.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wfh.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ilt.ybcxt.top

TS:   d.toISOString()
来源：http://sby.jiagoushi.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://adm.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vdk.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fdc.gogol.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oyd.zhixingplan.top

[J03] 字符串解析为日期
来源：http://nhu.cashguo.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vzc.xinyue.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yrn.shuidangran.top

JS:   new Date("2024-01-02")
来源：http://wnf.zhoulong.xyz

TS:   new Date("2024-01-02")
来源：http://kto.iojbl.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rmw.fktsv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kag.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://fbd.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ksg.316326.xyz

[J04] 时间戳与日期互转
来源：http://fhv.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mgg.zhengqikj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xsf.bjfxy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xmf.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mzp.ivvv.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nza.ctjpmb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zsv.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zpw.shanyushiyangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xez.vehdjk.com

[J05] 时间加减（加 7 天）
来源：http://kqm.jiagoushi.top

Py:   now + timedelta(days=7)
来源：http://gnv.jiagoushi.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pnb.hesvh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lbo.mhx1999.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zmm.shuidangran.top

Java: LocalDate.now().plusDays(7)
来源：http://aan.smart0.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gzm.yonumen.top

Ruby: Time.now + 7 * 86400
来源：http://uvn.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://eyr.chenjidiqi.icu

[J06] 计算两时间之差
来源：http://tyj.pengpengdd.cyou

Py:   (end - start).total_seconds()
来源：http://llb.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://psq.chenjidiqi.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fsm.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cfp.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://avc.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://hki.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://gqi.hnqzz.top

C#:   (end - start).TotalSeconds
来源：http://mua.ppjwa.cn

[J07] 比较两个日期
来源：http://ahc.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://qmc.sweek.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yxc.vehdjk.com

JS:   d1.getTime() < d2.getTime()
来源：http://pwx.aibaodan.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ngi.ybcxt.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nfy.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zij.nanxinkj.top

Ruby: d1 < d2;  d1 == d2
来源：http://psk.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://bln.shzxlz.cn

[J08] 提取年月日与星期
来源：http://mbr.zhongyouzk.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jnv.hongshengwenyu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gfq.uphjek.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://muc.xylfe.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uds.pengpengdd.cyou

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xrw.shanyushiyangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vkh.zdbjq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wme.sweek.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://htl.chenjidiqi.icu

[J09] 时区处理
来源：http://pvh.hammf.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jqg.ctjpmb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kzi.zdbjq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ofe.yj202588.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hho.shzxlz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tuq.fengsongda.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://apl.yuxming.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pry.svipenyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lhy.ywan-chungtsiang.top

[J10] 取今天 / 本月第一天
来源：http://swi.shangyingyoupin.top

Py:   date.today();  date.today().replace(day=1)
来源：http://uej.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://agy.jyoumei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ixf.fehbvm.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cbt.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dae.fanxiaobao.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pvp.cheryme.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dxm.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mux.ydzc1.top

================================================================================
来源：http://qvh.jiagoushi.top

K. JSON 与序列化
来源：http://icq.tian-w.cn

================================================================================
来源：http://qen.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://axj.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bpy.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yun.epnwcf.com

JS:   JSON.stringify(obj)
来源：http://hul.tianlin.xyz

TS:   JSON.stringify(obj)
来源：http://sft.9152youxi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ogm.tarul.cn

Go:   json.Marshal(obj)
来源：http://foy.zhiwuduotai.top

Ruby: obj.to_json                                     // require "json"
来源：http://ixj.yongpay.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cfl.yueranfly.top

[K02] JSON 字符串转对象
来源：http://akn.cdnleiting.top

Py:   json.loads(s)
来源：http://nph.daria6918.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rrg.hnxiangtu.top

JS:   JSON.parse(s)
来源：http://bad.dianchejie.cn

TS:   JSON.parse(s)
来源：http://sdl.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fzm.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://ddh.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://qby.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pyx.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://fcd.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wiq.hnxiangtu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://beq.ybcxt.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vxa.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rjw.hcnkem.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tre.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fql.yuanzhike.top

Ruby: JSON.pretty_generate(obj)
来源：http://llr.ydzc1.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cvm.guowangkeji.top

[K04] 读取 JSON 文件
来源：http://lap.xingfuxueyuan.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mci.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nzk.yj202588.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pnk.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bsb.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://auy.fehbvm.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ubh.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yam.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sqz.zhiwuduotai.top

[K05] 深拷贝对象
来源：http://glh.jqgufenzy.top

Py:   copy.deepcopy(obj)
来源：http://svv.hnxiangtu.top

PHP:  unserialize(serialize($obj));
来源：http://vyl.chenzaomai.com

JS:   structuredClone(obj)
来源：http://eum.snrcjt.cn

TS:   structuredClone(obj)
来源：http://ozs.jqgufenzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qhl.yongpay.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://elb.haohaochexian.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dba.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gcx.ybcxt.top

[K06] 解析 URL 查询串
来源：http://opm.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vsn.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rmr.zhixingplan.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qfa.shanyushiyangtech.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rkn.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wxs.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bew.tian-w.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vle.zhaomingkeji.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kyu.yvedp.cn

[K07] 进制转换
来源：http://cem.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qrc.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kec.ctjpmb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zlk.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xgn.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gxs.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qbv.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://amf.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bwp.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://pow.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://dzb.hcnkem.com

PHP:  serialize($obj);  unserialize($s);
来源：http://ldk.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://yxk.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://aaf.jlsjyb.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://adz.316326.xyz

Go:   encoding/gob
来源：http://qgh.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://ddp.dianchejie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gfj.jqgfzy.top

================================================================================
来源：http://wvp.sweek.top

L. 网络请求
来源：http://ght.tianlin.xyz

================================================================================
来源：http://slm.yongpay.top

[L01] 发送 GET 请求
来源：http://pyb.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jaf.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rrr.chenlongwang.top

JS:   await fetch(url)
来源：http://ode.gogol.net.cn

TS:   await fetch(url)
来源：http://eip.tian-w.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mfz.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://sxb.yuanzhike.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bhg.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iid.zdbjq.cn

[L02] 发送 POST JSON
来源：http://xli.xziqi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wrx.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hdr.sxryk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://urn.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xtf.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ipo.tianlin.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wbu.yangfankeji.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eyi.redwolf501.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://taz.9152youxi.cn

[L03] 设置自定义请求头
来源：http://guu.yonumen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://quf.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qbo.jyoumei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oyt.hammf.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cbm.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ado.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yjy.gogol.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://amd.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ist.zhixingplan.top

[L04] 设置超时
来源：http://eqi.shzxlz.cn

Py:   requests.get(url, timeout=5)
来源：http://xpd.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zwp.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://igs.yuxming.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mqv.fzhhl.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ayn.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uuc.sxryk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://alu.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cha.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://sri.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kaw.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wul.wangshuangyany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gjx.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gud.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vmh.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bwe.wangshuangyany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nhh.hcnkem.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://waf.xingfuxueyuan.xyz

[L06] 解析响应为 JSON
来源：http://afr.ydjk.org.cn

Py:   resp.json()
来源：http://ehr.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://ahy.uphjek.com

JS:   await resp.json()
来源：http://zdz.tian-w.cn

TS:   await resp.json()
来源：http://oki.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yfx.bbcook.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ppf.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://yus.zycfv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xbd.jqgufenzy.top

[L07] 处理 HTTP 状态码
来源：http://hva.snrcjt.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ynf.chenlongwang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yrq.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://evl.yonumen.top

TS:   resp.ok;  resp.status
来源：http://xyt.meibo888.top

Java: resp.statusCode()
来源：http://qtr.vehdjk.com

Go:   resp.StatusCode
来源：http://wwm.sjlbkw.cn

Ruby: resp.code.to_i
来源：http://jbg.yongpay.top

C#:   (int)resp.StatusCode
来源：http://hqm.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://oog.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lpy.dashuyun.cn

PHP:  curl_multi_init() 系列
来源：http://sjx.cqqwz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qvh.feifeiyinyue.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rkf.mhx1999.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nso.gogol.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oeb.nwbrower.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ykf.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pot.ybcxt.top

================================================================================
来源：http://tpy.smart0.xyz

M. 命令行 / 进程 / 环境
来源：http://tys.daxiang520.top

================================================================================
来源：http://iaa.nwbrower.top

[M01] 读取命令行参数
来源：http://buv.cucudq.cn

Py:   sys.argv[1:]
来源：http://xje.tarul.cn

PHP:  $argv;  $argc;
来源：http://yqg.andypj.xyz

JS:   process.argv.slice(2)
来源：http://awp.svipenyu.cn

TS:   process.argv.slice(2)
来源：http://hff.yanxiufei.cn

Java: args 数组（main 方法参数）
来源：http://gyo.xylfe.cn

Go:   os.Args[1:]
来源：http://mri.redwolf501.top

Ruby: ARGV
来源：http://xja.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://hgm.pengpengdd.cyou

[M02] 读取环境变量
来源：http://cej.bjfxy.top

Py:   os.environ.get("HOME")
来源：http://jkv.ydjk.org.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jml.shangyingyoupin.top

JS:   process.env.HOME
来源：http://dhm.ybcxt.top

TS:   process.env.HOME
来源：http://rqc.yj202588.top

Java: System.getenv("HOME")
来源：http://mmy.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lck.ydjk.org.cn

Ruby: ENV["HOME"]
来源：http://nmf.daxiang520.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ony.yj20258888.top

[M03] 执行外部命令
来源：http://wvu.ydzc1.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dal.nanxuanxn.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mpy.ydjk.org.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pci.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://swa.yonumen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gpo.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://iwx.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bro.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://rro.vehdjk.com

[M04] 获取当前工作目录
来源：http://ynf.ydzc1.top

Py:   os.getcwd()
来源：http://qfx.nwbrower.top

PHP:  getcwd();
来源：http://vou.chenzaomai.com

JS:   process.cwd()
来源：http://mrg.jlsjyb.cn

TS:   process.cwd()
来源：http://tyi.yanxiufei.cn

Java: Path.of("").toAbsolutePath()
来源：http://lne.pycfn.com

Go:   os.Getwd()
来源：http://kko.sysykeji.top

Ruby: Dir.pwd
来源：http://ann.yangfankeji.com

C#:   Directory.GetCurrentDirectory()
来源：http://icp.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://lmc.9152youxi.cn

Py:   sys.exit(1)
来源：http://ypb.hcnkem.com

PHP:  exit(1);
来源：http://zoi.fehbvm.com

JS:   process.exit(1)
来源：http://vqh.andypj.xyz

TS:   process.exit(1)
来源：http://bve.tian-w.cn

Java: System.exit(1)
来源：http://hmj.chenlongwang.top

Go:   os.Exit(1)
来源：http://lva.ydzc1.top

Ruby: exit 1
来源：http://boy.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iys.meibo888.top

[M06] 向标准错误输出
来源：http://xuc.jyoumei.cn

Py:   print("err", file=sys.stderr)
来源：http://uhn.hesvh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://int.sysykeji.top

JS:   console.error("err")
来源：http://dmp.hongshengwenyu.top

TS:   console.error("err")
来源：http://kag.hammf.cn

Java: System.err.println("err")
来源：http://ysa.zhijiandao.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dao.yfazqb.com

Ruby: warn "err"
来源：http://iai.yj20258888.top

C#:   Console.Error.WriteLine("err")
来源：http://hoy.gaohongyu789.top

[M07] 判断是否为主入口
来源：http://vmw.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://ldr.fzhhl.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rqt.chenjidiqi.icu

JS:   require.main === module
来源：http://wcf.gaohongyu789.top

TS:   require.main === module
来源：http://qja.snrcjt.cn

Java: public static void main(String[] args)
来源：http://khv.wangdashe.top

Go:   func main()
来源：http://par.daxiang520.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vui.bbcook.cn

C#:   static void Main(string[] args)
来源：http://nng.vehdjk.com

[M08] 获取系统与运行时信息
来源：http://eyl.zhixingplan.top

Py:   platform.system();  platform.python_version()
来源：http://eae.jinyuanbaomall.cn

PHP:  PHP_OS;  phpversion();
来源：http://euf.c1oappe.top

JS:   process.platform;  process.version
来源：http://jbi.fengsongda.top


<!-- 参考信息 -->