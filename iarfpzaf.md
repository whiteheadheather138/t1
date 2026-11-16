代发 wailian999

J. 日期与时间
来源：http://zgm.yvedp.cn

================================================================================
来源：http://rag.pengpengdd.cyou

[J01] 获取当前时间
来源：http://quo.shanyushiyangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jlu.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wke.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://kkp.uphjek.com

TS:   new Date();  Date.now()
来源：http://ryd.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ohk.fzhhl.top

Go:   time.Now()
来源：http://ghl.zdbjq.cn

Ruby: Time.now
来源：http://ybw.jqgfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vhp.shuidangran.top

[J02] 格式化输出
来源：http://cwa.jiagoushi.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ucv.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cri.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bpr.hcnkem.com

TS:   d.toISOString()
来源：http://cyf.birdmap.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dur.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ist.c1oappe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://njp.aizwys.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kep.vehdjk.com

[J03] 字符串解析为日期
来源：http://scw.fanxiaobao.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jap.bbcook.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wda.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://lcd.jinyuanbaomall.cn

TS:   new Date("2024-01-02")
来源：http://wxa.feifeiyinyue.top

Java: LocalDate.parse("2024-01-02")
来源：http://xrg.shangyingyoupin.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ofa.jinghuilouyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://hwy.gaohongyu789.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ght.jqgfzy.top

[J04] 时间戳与日期互转
来源：http://tqr.jinyuanbaomall.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yzu.zhongyouzk.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://het.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wnx.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://yqr.hnqzz.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qwl.nanxinkj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nwo.cqqwz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kyx.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lqi.fanxiaobao.xyz

[J05] 时间加减（加 7 天）
来源：http://zoo.xuanzx.com

Py:   now + timedelta(days=7)
来源：http://rsn.0kj1m.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lxx.sysykeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ofo.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xch.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://pfp.hnqzz.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wfk.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://axj.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://job.quarkkingdee.top

[J06] 计算两时间之差
来源：http://svu.zycfv.cn

Py:   (end - start).total_seconds()
来源：http://zrt.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://jwn.nwbrower.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bqm.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vsc.zdqjudy.top

Java: Duration.between(start, end).toSeconds()
来源：http://urr.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://aql.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://aex.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://lhn.bjfxy.top

[J07] 比较两个日期
来源：http://owt.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://sur.nanxinkj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cob.hesvh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gzv.sxryk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wdn.kuanghao11.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xac.xuanzx.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tqo.iojbl.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kat.wangdashe.top

C#:   d1 < d2;  d1 == d2
来源：http://qwn.xuanzx.com

[J08] 提取年月日与星期
来源：http://pkw.yj20258.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rgf.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ftv.gzhubu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vke.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ddv.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zbg.snrcjt.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kii.ctjpmb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jjo.xuetiantiany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fyi.andypj.xyz

[J09] 时区处理
来源：http://gzg.fanxiaobao.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dai.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ztb.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rel.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ffk.iojbl.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nqq.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://usp.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rbf.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kcd.jyoumei.cn

[J10] 取今天 / 本月第一天
来源：http://bvu.yonumen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nbx.fengsongda.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hsf.zdqjudy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pvk.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oiw.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ukq.fengsongda.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gby.gzhubu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gbw.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bmu.jinyuanbaomall.cn

================================================================================
来源：http://avt.shzxlz.cn

K. JSON 与序列化
来源：http://kja.yj20258.top

================================================================================
来源：http://xch.fengsongda.top

[K01] 对象转 JSON 字符串
来源：http://ajf.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mzf.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://afv.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://lgi.yj20258.top

TS:   JSON.stringify(obj)
来源：http://xmu.cucudq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zvm.fktsv.cn

Go:   json.Marshal(obj)
来源：http://rxb.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://afy.316326.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://lqw.pengpengdd.cyou

[K02] JSON 字符串转对象
来源：http://oic.gogol.net.cn

Py:   json.loads(s)
来源：http://nxg.zycfv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pyu.bbcook.cn

JS:   JSON.parse(s)
来源：http://kjq.zdqjudy.top

TS:   JSON.parse(s)
来源：http://zkz.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://egi.fktsv.cn

Go:   json.Unmarshal(data, &v)
来源：http://fjo.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://jir.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jmy.ydjk.org.cn

[K03] JSON 美化输出（带缩进）
来源：http://ryo.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vue.yuanzhike.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nfs.yueranfly.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hey.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wra.birdmap.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hwx.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://elg.0kj1m.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fjj.smart0.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jmi.shuidangran.top

[K04] 读取 JSON 文件
来源：http://wyj.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zja.tian-w.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bxx.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jic.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pne.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ppj.tianlin.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fny.birdmap.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://evh.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vyr.zhiwuduotai.top

[K05] 深拷贝对象
来源：http://hrl.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://xqd.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://pxu.tianlin.xyz

JS:   structuredClone(obj)
来源：http://xrq.hnxiangtu.top

TS:   structuredClone(obj)
来源：http://apf.jyoumei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cea.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dpo.yanxiufei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yzl.yvedp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oce.hesvh.cn

[K06] 解析 URL 查询串
来源：http://cuu.redwolf501.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vza.c1oappe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sir.birdmap.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://btu.hysaishi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bbh.zhongyouzk.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wao.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jau.guannengcc.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ldq.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uwa.ctjpmb.com

[K07] 进制转换
来源：http://mnk.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bqe.yueranfly.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ogf.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ilr.jinyuanbaomall.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://psf.svipenyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fmx.yvedp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://egi.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ekx.yueranfly.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fse.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://rdd.yj20258.top

Py:   pickle.dumps(obj)
来源：http://xvs.zhongyouzk.top

PHP:  serialize($obj);  unserialize($s);
来源：http://kqv.xuanzx.com

JS:   v8.serialize(obj)        // Node
来源：http://yje.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://cxe.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vud.vqdsnc.cn

Go:   encoding/gob
来源：http://qvo.hnqzz.top

Ruby: Marshal.dump(obj)
来源：http://rzj.nanxuanxn.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hek.zycfv.cn

================================================================================
来源：http://qjl.9152youxi.cn

L. 网络请求
来源：http://aiv.xinyue.icu

================================================================================
来源：http://yhz.uphjek.com

[L01] 发送 GET 请求
来源：http://zhe.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rup.guannengcc.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mmi.meibo888.top

JS:   await fetch(url)
来源：http://uqp.daxiang520.top

TS:   await fetch(url)
来源：http://qqf.hfpthk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oao.ybcxt.top

Go:   resp, err := http.Get(url)
来源：http://wyg.kuanghao11.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://unv.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nss.uphjek.com

[L02] 发送 POST JSON
来源：http://guw.ybcxt.top

Py:   requests.post(url, json={"a": 1})
来源：http://svp.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://khr.yongpay.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://keb.zhaomingkeji.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fzp.havefunace.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rsx.xziqi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jga.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mcs.pycfn.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rui.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://gmr.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://esz.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hyr.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://duy.haohaochexian.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ylh.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tel.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ftb.hnxiangtu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gqp.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bbu.0kj1m.cn

[L04] 设置超时
来源：http://kxk.zhoulong.xyz

Py:   requests.get(url, timeout=5)
来源：http://qrk.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kuo.fanxiaobao.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rir.sweek.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dgf.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rco.hammf.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ycp.dianchejie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uip.chenzaomai.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lty.0kj1m.cn

[L05] 上传文件（multipart）
来源：http://wca.xylfe.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rgv.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://abj.ydzc1.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vxn.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jju.wangshuangyany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mup.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ovs.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hlt.dashuyun.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ixg.sysykeji.top

[L06] 解析响应为 JSON
来源：http://jgo.wangshuangyany.cn

Py:   resp.json()
来源：http://fak.zdqjudy.top

PHP:  json_decode($body, true);
来源：http://kvm.nanxinkj.top

JS:   await resp.json()
来源：http://tku.birdmap.top

TS:   await resp.json()
来源：http://rla.yuxming.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gnf.dianchejie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rib.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://eyf.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jzz.chenjidiqi.icu

[L07] 处理 HTTP 状态码
来源：http://rqm.zdqjudy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vxe.jianghu66.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://haj.jqgufenzy.top

JS:   resp.ok;  resp.status
来源：http://anw.ivvv.top

TS:   resp.ok;  resp.status
来源：http://ykj.hnqzz.top

Java: resp.statusCode()
来源：http://nds.vehdjk.com

Go:   resp.StatusCode
来源：http://wui.dashuyun.cn

Ruby: resp.code.to_i
来源：http://vvd.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://tva.ppjwa.cn

[L08] 并发请求多个地址
来源：http://gfo.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://peh.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://htp.ehwqpu.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dkw.sxryk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://feu.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://izb.cheryme.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ahh.mhx1999.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wps.ctjpmb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yrw.ivvv.top

================================================================================
来源：http://kal.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://icj.ppjwa.cn

================================================================================
来源：http://uog.fktsv.cn

[M01] 读取命令行参数
来源：http://kvm.xinyue.icu

Py:   sys.argv[1:]
来源：http://pgr.cheryme.top

PHP:  $argv;  $argc;
来源：http://vpa.jyoumei.cn

JS:   process.argv.slice(2)
来源：http://akc.fanxiaobao.xyz

TS:   process.argv.slice(2)
来源：http://vdo.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://rna.fzhhl.top

Go:   os.Args[1:]
来源：http://nre.hesvh.cn

Ruby: ARGV
来源：http://nou.andypj.xyz

C#:   args 数组（Main 方法参数）
来源：http://gby.shangyingyoupin.top

[M02] 读取环境变量
来源：http://bou.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://cup.yangfankeji.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://goz.xylfe.cn

JS:   process.env.HOME
来源：http://gkx.gotoacloud.top

TS:   process.env.HOME
来源：http://hjw.yvedp.cn

Java: System.getenv("HOME")
来源：http://bio.sufxvd.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nil.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://qcq.zdqjudy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dnf.bjfxy.top

[M03] 执行外部命令
来源：http://eab.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rqh.iojbl.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yhq.ywan-chungtsiang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dhk.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qeq.tianlin.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uey.fehbvm.com

Go:   exec.Command("ls", "-l").Output()
来源：http://eza.cashguo.top

Ruby: system("ls -l");  `ls -l`
来源：http://cgt.zdqjudy.top

C#:   Process.Start("ls", "-l");
来源：http://vjh.hfpthk.cn

[M04] 获取当前工作目录
来源：http://pmi.snrcjt.cn

Py:   os.getcwd()
来源：http://cko.jqgfzy.top

PHP:  getcwd();
来源：http://zfb.shangyingyoupin.top

JS:   process.cwd()
来源：http://lff.mhx1999.top

TS:   process.cwd()
来源：http://bqr.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://tqm.jlsjyb.cn

Go:   os.Getwd()
来源：http://mey.zhaomingkeji.xyz

Ruby: Dir.pwd
来源：http://qht.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lup.zdbjq.cn

[M05] 设置退出码
来源：http://hbr.hysaishi.cn

Py:   sys.exit(1)
来源：http://bht.xuanzx.com

PHP:  exit(1);
来源：http://yei.gzhubu.top

JS:   process.exit(1)
来源：http://fxq.svipenyu.cn

TS:   process.exit(1)
来源：http://esq.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://iwn.vehdjk.com

Go:   os.Exit(1)
来源：http://hcx.hnxiangtu.top

Ruby: exit 1
来源：http://dho.chenlongwang.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cme.snrcjt.cn

[M06] 向标准错误输出
来源：http://dhw.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://frb.shanyushiyangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fbb.redwolf501.top

JS:   console.error("err")
来源：http://crh.shzxlz.cn

TS:   console.error("err")
来源：http://yuo.shanyushiyangkeji.top

Java: System.err.println("err")
来源：http://lup.sxryk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oce.hesvh.cn

Ruby: warn "err"
来源：http://yoi.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://fbd.jiagoushi.top

[M07] 判断是否为主入口
来源：http://uzb.ehwqpu.com


<!-- 参考信息 -->