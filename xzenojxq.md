代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rzy.ydzc1.top

JS:   new Date();  Date.now()
来源：http://psg.zhijiandao.cn

TS:   new Date();  Date.now()
来源：http://kmw.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ycj.epnwcf.com

Go:   time.Now()
来源：http://lcq.sxryk.cn

Ruby: Time.now
来源：http://bgj.yanxiufei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vii.ctjpmb.com

[J02] 格式化输出
来源：http://zuo.jinqigfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mad.shuidangran.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nrh.fehbvm.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://erw.zhiwuduotai.top

TS:   d.toISOString()
来源：http://eox.tanke756.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://whc.gaohongyu789.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xkk.hysaishi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vul.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qix.ppjwa.cn

[J03] 字符串解析为日期
来源：http://jil.jinqigufen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yli.yanxiufei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pvb.gotoacloud.top

JS:   new Date("2024-01-02")
来源：http://ksx.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://zgd.jyoumei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mma.bjfxy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ysr.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://uqn.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bdv.aibaodan.cn

[J04] 时间戳与日期互转
来源：http://jbt.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wbv.gaohongyu789.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aiw.dashuyun.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vnd.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://drs.hongshengwenyu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tfh.9152youxi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://deu.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ixh.smart0.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nuc.gzhubu.top

[J05] 时间加减（加 7 天）
来源：http://rmu.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://ycp.c1oappe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ztn.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wcv.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://asj.ppjwa.cn

Java: LocalDate.now().plusDays(7)
来源：http://eeh.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hgu.cqqwz.cn

Ruby: Time.now + 7 * 86400
来源：http://ewp.redwolf501.top

C#:   DateTime.Now.AddDays(7)
来源：http://ubs.316326.xyz

[J06] 计算两时间之差
来源：http://xpz.sysykeji.top

Py:   (end - start).total_seconds()
来源：http://gxs.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://xmk.hnxiangtu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dxt.ehwqpu.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qry.daxiang520.top

Java: Duration.between(start, end).toSeconds()
来源：http://lhv.hammf.cn

Go:   end.Sub(start).Hours()
来源：http://qeu.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://ecc.sweek.top

C#:   (end - start).TotalSeconds
来源：http://qiu.yvedp.cn

[J07] 比较两个日期
来源：http://trg.ydzc1.top

Py:   d1 < d2;  d1 == d2
来源：http://eua.quarkkingdee.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rfi.nwbrower.top

JS:   d1.getTime() < d2.getTime()
来源：http://iqj.mhx1999.top

TS:   d1.getTime() < d2.getTime()
来源：http://qbs.daria6918.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kqk.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xrg.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://wbp.zhaomingkeji.xyz

C#:   d1 < d2;  d1 == d2
来源：http://fww.yfazqb.com

[J08] 提取年月日与星期
来源：http://djv.fanxiaobao.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://svx.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wci.ybcxt.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vxw.pengpengdd.cyou

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gnc.aizwys.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eap.shangyingyoupin.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xig.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tzx.fehbvm.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://csh.guannengcc.top

[J09] 时区处理
来源：http://tty.hnqzz.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qhh.ctjpmb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bcy.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ukh.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://azh.yuxming.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://org.sysykeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xxc.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yot.yanxiufei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dgc.fktsv.cn

[J10] 取今天 / 本月第一天
来源：http://eyc.kuanghao11.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ctk.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hem.xinyue.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rqz.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jtd.ctjpmb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jda.zhoulong.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://awq.feifeiyinyue.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://too.meibo888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jot.yonumen.top

================================================================================
来源：http://xpk.ywan-chungtsiang.top

K. JSON 与序列化
来源：http://alb.nanxinkj.top

================================================================================
来源：http://rpe.xinyue.icu

[K01] 对象转 JSON 字符串
来源：http://uyo.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qgx.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://owv.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://ygp.daria6918.cn

TS:   JSON.stringify(obj)
来源：http://xim.yuxming.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://szp.0kj1m.cn

Go:   json.Marshal(obj)
来源：http://dmc.chenzaomai.com

Ruby: obj.to_json                                     // require "json"
来源：http://ani.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cjy.hammf.cn

[K02] JSON 字符串转对象
来源：http://nzh.ctjpmb.com

Py:   json.loads(s)
来源：http://szg.ydzc1.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mon.316326.xyz

JS:   JSON.parse(s)
来源：http://cdx.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://jms.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://neh.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://ves.ctjpmb.com

Ruby: JSON.parse(s)
来源：http://gjt.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dfu.hcnkem.com

[K03] JSON 美化输出（带缩进）
来源：http://ewu.tarul.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kdh.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://slp.jinyuanbaomall.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lpq.jinqigfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://grj.gogol.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ewj.gogol.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dko.0kj1m.cn

Ruby: JSON.pretty_generate(obj)
来源：http://blj.shuidangran.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yex.hammf.cn

[K04] 读取 JSON 文件
来源：http://plj.wangdashe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aka.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gvr.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yjo.fanxiaobao.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://guh.zhijiandao.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fiw.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://itr.tarul.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cjs.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ypg.cheryme.top

[K05] 深拷贝对象
来源：http://wqp.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://rxr.pengpengdd.cyou

PHP:  unserialize(serialize($obj));
来源：http://rqr.tianlin.xyz

JS:   structuredClone(obj)
来源：http://pbu.mhx1999.top

TS:   structuredClone(obj)
来源：http://hrm.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gbo.sufxvd.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sbf.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nqj.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lug.cdnleiting.top

[K06] 解析 URL 查询串
来源：http://mcz.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vxp.kuanghao11.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yve.shzxlz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ydb.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jwi.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dcs.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kur.hesvh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dlh.fengsongda.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bdo.gzhubu.top

[K07] 进制转换
来源：http://jvk.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://onk.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sov.shanyushiyangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rgs.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iro.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oac.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wwo.ywan-chungtsiang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ocv.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fxa.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://rqb.yj20258888.top

Py:   pickle.dumps(obj)
来源：http://ugl.gogol.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rrf.yuanzhike.top

JS:   v8.serialize(obj)        // Node
来源：http://ynr.wangdashe.top

TS:   v8.serialize(obj)        // Node
来源：http://nfu.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mqc.ydzc1.top

Go:   encoding/gob
来源：http://gic.tarul.cn

Ruby: Marshal.dump(obj)
来源：http://sah.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://trz.wangdashe.top

================================================================================
来源：http://ozx.sysykeji.top

L. 网络请求
来源：http://mkw.andypj.xyz

================================================================================
来源：http://ris.aibaodan.cn

[L01] 发送 GET 请求
来源：http://yyh.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ajg.jqgufenzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sco.hnxiangtu.top

JS:   await fetch(url)
来源：http://lbx.yuanzhike.top

TS:   await fetch(url)
来源：http://vfp.hfpthk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kyf.yfazqb.com

Go:   resp, err := http.Get(url)
来源：http://eqc.svipenyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://quq.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ksx.xingfuxueyuan.xyz

[L02] 发送 POST JSON
来源：http://tfs.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vhu.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rqa.jlsjyb.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qgv.yj20258.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ycj.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sub.yfazqb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ybg.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iiw.xylfe.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lbq.kuanghao11.cn

[L03] 设置自定义请求头
来源：http://pan.jinyuanbaomall.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sol.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fie.chenjidiqi.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ogj.zdbjq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oji.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oih.shanyushiyangtech.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xgf.c1oappe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ids.sysykeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jsr.ydjk.org.cn

[L04] 设置超时
来源：http://zrm.sxryk.cn

Py:   requests.get(url, timeout=5)
来源：http://fec.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qby.yongpay.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mrm.gaohongyu789.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wzk.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cge.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cqm.hesvh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qof.gzhubu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oka.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://sqf.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gcv.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kbz.svipenyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://asn.ppjwa.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vio.jinqigufen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rsb.dianchejie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iac.jqgufenzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://quv.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xzw.yfazqb.com

[L06] 解析响应为 JSON
来源：http://dzu.iojbl.cn

Py:   resp.json()
来源：http://exb.9152youxi.cn

PHP:  json_decode($body, true);
来源：http://hhm.dianchejie.cn

JS:   await resp.json()
来源：http://cdx.jianghu66.top

TS:   await resp.json()
来源：http://aed.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nxo.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://doa.sjlbkw.cn

Ruby: JSON.parse(resp.body)
来源：http://kmw.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cbb.sweek.top

[L07] 处理 HTTP 状态码
来源：http://kqw.daria6918.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sck.hysaishi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zlb.chenlongwang.top

JS:   resp.ok;  resp.status
来源：http://zyw.havefunace.top

TS:   resp.ok;  resp.status
来源：http://ilw.316326.xyz

Java: resp.statusCode()
来源：http://nia.haohaochexian.top

Go:   resp.StatusCode
来源：http://xav.yvedp.cn

Ruby: resp.code.to_i
来源：http://yzc.cashguo.top

C#:   (int)resp.StatusCode
来源：http://yex.xuanzx.com

[L08] 并发请求多个地址
来源：http://enc.gotoacloud.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jhv.yuxming.cn

PHP:  curl_multi_init() 系列
来源：http://grp.9152youxi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eiw.epnwcf.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vnn.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://faf.fehbvm.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://omu.316326.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ccq.jinyuanbaomall.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yyn.meibo888.top

================================================================================
来源：http://rld.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://kev.havefunace.top

================================================================================
来源：http://xaz.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://ook.mhx1999.top

Py:   sys.argv[1:]
来源：http://rij.vqdsnc.cn

PHP:  $argv;  $argc;
来源：http://fpv.c1oappe.top

JS:   process.argv.slice(2)
来源：http://ikw.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://tla.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://hyv.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://ppc.bbcook.cn

Ruby: ARGV
来源：http://gra.nanxinkj.top

C#:   args 数组（Main 方法参数）
来源：http://aua.vehdjk.com

[M02] 读取环境变量
来源：http://svt.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://jtg.birdmap.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://okn.ehwqpu.com

JS:   process.env.HOME
来源：http://pgb.ydzc1.top

TS:   process.env.HOME
来源：http://mqw.yangfankeji.com

Java: System.getenv("HOME")
来源：http://yyw.hywenlv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ikd.hfpthk.cn

Ruby: ENV["HOME"]
来源：http://noz.0kj1m.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dyj.zhaomingkeji.xyz

[M03] 执行外部命令
来源：http://dhw.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qmj.fehbvm.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dyc.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xqf.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://mig.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xdq.gogol.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fpz.epnwcf.com

Ruby: system("ls -l");  `ls -l`
来源：http://btc.tanke756.top

C#:   Process.Start("ls", "-l");
来源：http://wbj.jqgufenzy.top

[M04] 获取当前工作目录
来源：http://nqt.fengsongda.top

Py:   os.getcwd()
来源：http://tcn.jinqigufen.top

PHP:  getcwd();
来源：http://nef.haohaochexian.top

JS:   process.cwd()
来源：http://vzd.redwolf501.top

TS:   process.cwd()
来源：http://nch.vqdsnc.cn

Java: Path.of("").toAbsolutePath()
来源：http://tlz.haohaochexian.top

Go:   os.Getwd()
来源：http://etw.jianghu66.top

Ruby: Dir.pwd
来源：http://pck.ywan-chungtsiang.top

C#:   Directory.GetCurrentDirectory()
来源：http://aem.pengpengdd.cyou

[M05] 设置退出码
来源：http://qbr.jiagoushi.top

Py:   sys.exit(1)
来源：http://zbe.vqdsnc.cn

PHP:  exit(1);
来源：http://epd.chenlongwang.top

JS:   process.exit(1)
来源：http://sdb.yvedp.cn

TS:   process.exit(1)
来源：http://gbk.0kj1m.cn

Java: System.exit(1)
来源：http://pia.smart0.xyz

Go:   os.Exit(1)
来源：http://cjy.wangdashe.top

Ruby: exit 1
来源：http://fap.shanyushiyangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hfg.shuidangran.top

[M06] 向标准错误输出
来源：http://wdp.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://iah.zhengqikj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pzg.ydzc1.top

JS:   console.error("err")
来源：http://bcu.hywenlv.cn

TS:   console.error("err")
来源：http://jpb.fktsv.cn

Java: System.err.println("err")
来源：http://eny.yfazqb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rbz.yongpay.top

Ruby: warn "err"
来源：http://trj.shangyingyoupin.top

C#:   Console.Error.WriteLine("err")
来源：http://vkv.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://dje.shzxlz.cn

Py:   if __name__ == "__main__":
来源：http://itk.gogol.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dmf.zhengqikj.top

JS:   require.main === module
来源：http://ogk.chenjidiqi.icu

TS:   require.main === module
来源：http://fgj.sufxvd.cn


<!-- 参考信息 -->