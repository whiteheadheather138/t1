代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tyk.xziqi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eax.sweek.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zib.quarkkingdee.top

TS:   d.toISOString()
来源：http://hpa.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://axu.tanke756.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bep.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oud.gotoacloud.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jid.cucudq.cn

[J03] 字符串解析为日期
来源：http://txz.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://caq.zycfv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ifw.shuidangran.top

JS:   new Date("2024-01-02")
来源：http://rvf.nwbrower.top

TS:   new Date("2024-01-02")
来源：http://rof.shanyushiyangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://jjb.cdnleiting.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zdz.hnqzz.top

Ruby: Date.parse("2024-01-02")
来源：http://ihw.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xui.hammf.cn

[J04] 时间戳与日期互转
来源：http://mru.xuetiantiany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://soi.xziqi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ntu.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kxd.epnwcf.com

TS:   Math.floor(Date.now() / 1000)
来源：http://tzd.fktsv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vfl.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ghe.hongshengwenyu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rtd.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tho.wangdashe.top

[J05] 时间加减（加 7 天）
来源：http://acd.yj202588.top

Py:   now + timedelta(days=7)
来源：http://ryk.nanxuanxn.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://aoa.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ght.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://khj.hongshengwenyu.top

Java: LocalDate.now().plusDays(7)
来源：http://enx.yonumen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sns.nwbrower.top

Ruby: Time.now + 7 * 86400
来源：http://gcr.ivvv.top

C#:   DateTime.Now.AddDays(7)
来源：http://dai.jianghu66.top

[J06] 计算两时间之差
来源：http://roe.xuanzx.com

Py:   (end - start).total_seconds()
来源：http://zxa.wangshuangyany.cn

PHP:  $end->diff($start)->days;
来源：http://ilr.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vdb.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kqu.jlsjyb.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xbz.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://ssn.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://txf.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://wok.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://qau.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://eqb.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://scf.shuidangran.top

JS:   d1.getTime() < d2.getTime()
来源：http://hop.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://uzm.fzhhl.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rhh.nwbrower.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xfj.zdbjq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://njm.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://fjh.tanke756.top

[J08] 提取年月日与星期
来源：http://awi.quarkkingdee.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cji.smart0.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wri.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nhk.yueranfly.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iiv.yj202588.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mta.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cyy.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uco.daria6918.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wso.xuetiantiany.cn

[J09] 时区处理
来源：http://sht.xylfe.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://duv.smart0.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bjv.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://coy.jinyuanbaomall.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ghr.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xqn.shuidangran.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://akm.sysykeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hbt.yangfankeji.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jdd.yvedp.cn

[J10] 取今天 / 本月第一天
来源：http://ged.zhongyouzk.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jix.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yzg.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zki.wangdashe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pvv.chenjidiqi.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gpe.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iig.hnqzz.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dmf.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gli.cheryme.top

================================================================================
来源：http://ant.jiagoushi.top

K. JSON 与序列化
来源：http://urq.zhoulong.xyz

================================================================================
来源：http://qbx.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://opb.xinyue.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rji.xuanzx.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://auf.ehwqpu.com

JS:   JSON.stringify(obj)
来源：http://pqz.andypj.xyz

TS:   JSON.stringify(obj)
来源：http://ylm.meibo888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bgb.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://uvo.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://xdt.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gij.jianghu66.top

[K02] JSON 字符串转对象
来源：http://fvy.yuanzhike.top

Py:   json.loads(s)
来源：http://syl.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hiz.zhijiandao.cn

JS:   JSON.parse(s)
来源：http://pll.daria6918.cn

TS:   JSON.parse(s)
来源：http://btq.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mwx.aizwys.cn

Go:   json.Unmarshal(data, &v)
来源：http://ael.mhx1999.top

Ruby: JSON.parse(s)
来源：http://smj.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pnz.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://xpz.yueranfly.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hfm.yfazqb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nzj.hcnkem.com

JS:   JSON.stringify(obj, null, 2)
来源：http://pwp.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://pgb.zhixingplan.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vkq.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qsl.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ayr.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jbr.cashguo.top

[K04] 读取 JSON 文件
来源：http://brb.aibaodan.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nsa.xuanzx.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dqs.chenzaomai.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tlo.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rzz.bjfxy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://acy.ehwqpu.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zkg.cashguo.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://iss.cheryme.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jki.gaohongyu789.top

[K05] 深拷贝对象
来源：http://ofb.zhijiandao.cn

Py:   copy.deepcopy(obj)
来源：http://zst.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://xll.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://hct.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://nni.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://clq.zdbjq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hbk.52xcode.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iwn.hcnkem.com

C#:   // 序列化往返，或自定义 Clone
来源：http://jhh.yuxming.cn

[K06] 解析 URL 查询串
来源：http://emb.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tuc.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yun.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dtt.dashuyun.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vvz.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hxx.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vkm.zhijiandao.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hnw.feifeiyinyue.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aod.ydzc1.top

[K07] 进制转换
来源：http://qzk.daxiang520.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hds.svipenyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xdh.vehdjk.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fle.gaohongyu789.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ezl.quarkkingdee.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mae.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xbl.yfazqb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nhp.ctjpmb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zov.tanke756.top

[K08] 二进制序列化（非 JSON）
来源：http://xif.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://rax.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fhi.yanxiufei.cn

JS:   v8.serialize(obj)        // Node
来源：http://ykz.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://xas.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pcd.gzhubu.top

Go:   encoding/gob
来源：http://cvy.yfazqb.com

Ruby: Marshal.dump(obj)
来源：http://vny.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nfn.chenlongwang.top

================================================================================
来源：http://wtw.tianlin.xyz

L. 网络请求
来源：http://zsx.hcnkem.com

================================================================================
来源：http://rzs.hywenlv.cn

[L01] 发送 GET 请求
来源：http://fck.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kqx.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qcd.fehbvm.com

JS:   await fetch(url)
来源：http://meb.ctjpmb.com

TS:   await fetch(url)
来源：http://ero.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ekv.xuetiantiany.cn

Go:   resp, err := http.Get(url)
来源：http://wqz.daria6918.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qdm.aizwys.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mwc.shanyushiyangtech.top

[L02] 发送 POST JSON
来源：http://shw.yonumen.top

Py:   requests.post(url, json={"a": 1})
来源：http://qmv.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://chu.redwolf501.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://afo.yfazqb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://erl.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://umr.ivvv.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xht.hesvh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fgl.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ooo.daria6918.cn

[L03] 设置自定义请求头
来源：http://ucx.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lxx.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lqf.guannengcc.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tte.gaohongyu789.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://exc.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nmu.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pyq.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vss.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tpo.bbcook.cn

[L04] 设置超时
来源：http://syk.gogol.net.cn

Py:   requests.get(url, timeout=5)
来源：http://zcz.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lri.quarkkingdee.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://euo.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nab.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qvo.fehbvm.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rlw.daria6918.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uud.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lyn.zhiwuduotai.top

[L05] 上传文件（multipart）
来源：http://kqs.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nbc.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uua.shanyushiyangtech.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ivq.gzhubu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dwy.jinghuilouyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oqm.yfazqb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pxz.havefunace.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dpo.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tvz.cdnleiting.top

[L06] 解析响应为 JSON
来源：http://yot.chenjidiqi.icu

Py:   resp.json()
来源：http://pbw.guannengcc.top

PHP:  json_decode($body, true);
来源：http://cgq.gotoacloud.top

JS:   await resp.json()
来源：http://ouk.vehdjk.com

TS:   await resp.json()
来源：http://wvk.chenlongwang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ooy.jinqigufen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://elk.havefunace.top

Ruby: JSON.parse(resp.body)
来源：http://nqi.nanxinkj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tqs.jianghu66.top

[L07] 处理 HTTP 状态码
来源：http://wqf.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tdr.ivvv.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bed.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://rfk.shanyushiyangkeji.top

TS:   resp.ok;  resp.status
来源：http://uqk.yuanzhike.top

Java: resp.statusCode()
来源：http://lkw.jlsjyb.cn

Go:   resp.StatusCode
来源：http://ayo.epnwcf.com

Ruby: resp.code.to_i
来源：http://trt.ydjk.org.cn

C#:   (int)resp.StatusCode
来源：http://fkq.yangfankeji.com

[L08] 并发请求多个地址
来源：http://gdn.jinghuilouyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ttb.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://zxo.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zff.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rob.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://njr.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://twq.andypj.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vsz.tianlin.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qyv.yvedp.cn

================================================================================
来源：http://oup.mhx1999.top

M. 命令行 / 进程 / 环境
来源：http://jhh.daxiang520.top

================================================================================
来源：http://wgt.pycfn.com

[M01] 读取命令行参数
来源：http://qrd.svipenyu.cn

Py:   sys.argv[1:]
来源：http://efz.fzhhl.top

PHP:  $argv;  $argc;
来源：http://eil.bjfxy.top

JS:   process.argv.slice(2)
来源：http://gxk.havefunace.top

TS:   process.argv.slice(2)
来源：http://iby.yj20258.top

Java: args 数组（main 方法参数）
来源：http://ynk.jiagoushi.top

Go:   os.Args[1:]
来源：http://uex.wangshuangyany.cn

Ruby: ARGV
来源：http://xob.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://lbk.daxiang520.top

[M02] 读取环境变量
来源：http://scw.zhixingplan.top

Py:   os.environ.get("HOME")
来源：http://rka.dianchejie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gvk.uphjek.com

JS:   process.env.HOME
来源：http://neb.cdnleiting.top

TS:   process.env.HOME
来源：http://ame.yongpay.top

Java: System.getenv("HOME")
来源：http://bky.mhx1999.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xcg.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://frd.jianghu66.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hdy.zhixingplan.top

[M03] 执行外部命令
来源：http://mod.yongpay.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lbg.jinyuanbaomall.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nof.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ibx.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rat.chenlongwang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aao.jinyuanbaomall.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uvi.0kj1m.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kyk.yj202588.top

C#:   Process.Start("ls", "-l");
来源：http://nkv.sweek.top

[M04] 获取当前工作目录
来源：http://zwv.tarul.cn

Py:   os.getcwd()
来源：http://mtd.yj20258.top

PHP:  getcwd();
来源：http://oti.xuetiantiany.cn

JS:   process.cwd()
来源：http://chj.nwbrower.top

TS:   process.cwd()
来源：http://hyv.shuidangran.top

Java: Path.of("").toAbsolutePath()
来源：http://asj.cashguo.top

Go:   os.Getwd()
来源：http://hcb.yj20258.top

Ruby: Dir.pwd
来源：http://gne.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cbe.hcnkem.com

[M05] 设置退出码
来源：http://cat.vehdjk.com

Py:   sys.exit(1)
来源：http://eud.hcnkem.com

PHP:  exit(1);
来源：http://alr.shzxlz.cn

JS:   process.exit(1)
来源：http://ekt.dianchejie.cn

TS:   process.exit(1)
来源：http://rti.gotoacloud.top

Java: System.exit(1)
来源：http://dne.yfazqb.com

Go:   os.Exit(1)
来源：http://mqc.epnwcf.com

Ruby: exit 1
来源：http://vyu.jlsjyb.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://igm.sjlbkw.cn

[M06] 向标准错误输出
来源：http://nvv.iojbl.cn

Py:   print("err", file=sys.stderr)
来源：http://rou.jiagoushi.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fnc.sjlbkw.cn

JS:   console.error("err")
来源：http://byp.yueranfly.top

TS:   console.error("err")
来源：http://uwe.fzhhl.top

Java: System.err.println("err")
来源：http://ktv.andypj.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dtw.gogol.net.cn

Ruby: warn "err"
来源：http://jau.yfazqb.com

C#:   Console.Error.WriteLine("err")
来源：http://npc.jqgfzy.top

[M07] 判断是否为主入口
来源：http://pnr.yj20258888.top

Py:   if __name__ == "__main__":
来源：http://lnx.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ntb.chenzaomai.com

JS:   require.main === module
来源：http://uju.sxryk.cn

TS:   require.main === module
来源：http://ttr.meibo888.top

Java: public static void main(String[] args)
来源：http://exf.wangshuangyany.cn

Go:   func main()
来源：http://lmi.chenlongwang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://urc.quarkkingdee.top

C#:   static void Main(string[] args)
来源：http://vsf.wangdashe.top

[M08] 获取系统与运行时信息
来源：http://oiw.xziqi.cn

Py:   platform.system();  platform.python_version()
来源：http://mmy.quarkkingdee.top

PHP:  PHP_OS;  phpversion();
来源：http://wob.tianlin.xyz

JS:   process.platform;  process.version
来源：http://dnj.ydjk.org.cn


<!-- 参考信息 -->