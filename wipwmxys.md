代发 wailian999

J. 日期与时间
来源：http://vst.zhixingplan.top

================================================================================
来源：http://nnx.aizwys.cn

[J01] 获取当前时间
来源：http://brb.tarul.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qjt.tanke756.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://naa.ydzc1.top

JS:   new Date();  Date.now()
来源：http://kxo.tanke756.top

TS:   new Date();  Date.now()
来源：http://ncb.meibo888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xaq.xinyue.icu

Go:   time.Now()
来源：http://ohh.hywenlv.cn

Ruby: Time.now
来源：http://uff.gotoacloud.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mns.daxiang520.top

[J02] 格式化输出
来源：http://mht.shuidangran.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ppy.0kj1m.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tqn.xuetiantiany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lvv.chenjidiqi.icu

TS:   d.toISOString()
来源：http://nqm.ivvv.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nym.nwbrower.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vqs.xingfuxueyuan.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kbk.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://asp.iojbl.cn

[J03] 字符串解析为日期
来源：http://clu.nanxuanxn.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yht.yj20258888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vdq.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://uzd.jianghu66.top

TS:   new Date("2024-01-02")
来源：http://ccb.pycfn.com

Java: LocalDate.parse("2024-01-02")
来源：http://lnz.yangfankeji.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ehu.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://geh.shzxlz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mvn.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://qqx.sysykeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rwa.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rex.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yiz.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zup.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ukh.jinqigfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qpc.nwbrower.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zhv.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jqg.zdqjudy.top

[J05] 时间加减（加 7 天）
来源：http://vjp.snrcjt.cn

Py:   now + timedelta(days=7)
来源：http://oxw.fengsongda.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rrk.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yft.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oqm.epnwcf.com

Java: LocalDate.now().plusDays(7)
来源：http://ghf.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pmh.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://crq.bjfxy.top

C#:   DateTime.Now.AddDays(7)
来源：http://cpw.vqdsnc.cn

[J06] 计算两时间之差
来源：http://fpe.sweek.top

Py:   (end - start).total_seconds()
来源：http://kbn.xuetiantiany.cn

PHP:  $end->diff($start)->days;
来源：http://qvx.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jhx.hcnkem.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uzj.yuanzhike.top

Java: Duration.between(start, end).toSeconds()
来源：http://xwu.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://bgx.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://qhf.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://cdc.sweek.top

[J07] 比较两个日期
来源：http://urz.wangdashe.top

Py:   d1 < d2;  d1 == d2
来源：http://zbq.cdnleiting.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dvl.52xcode.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wkx.xylfe.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sax.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jaj.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zqy.ivvv.top

Ruby: d1 < d2;  d1 == d2
来源：http://pzy.0kj1m.cn

C#:   d1 < d2;  d1 == d2
来源：http://hip.birdmap.top

[J08] 提取年月日与星期
来源：http://pxq.ehwqpu.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vgm.xuetiantiany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tqg.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pov.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aam.chenzaomai.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ros.9152youxi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ccw.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fnj.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vpw.yj202588.top

[J09] 时区处理
来源：http://azz.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mgs.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lxv.bjfxy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ssy.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bwi.iojbl.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uok.dianchejie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eug.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nil.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ext.cashguo.top

[J10] 取今天 / 本月第一天
来源：http://vjm.zhongyouzk.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cqf.jinghuilouyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ilf.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ukz.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://shs.cucudq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://usg.sweek.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vds.zdbjq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yno.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://odh.dashuyun.cn

================================================================================
来源：http://mgb.jlsjyb.cn

K. JSON 与序列化
来源：http://htb.shangyingyoupin.top

================================================================================
来源：http://fui.cucudq.cn

[K01] 对象转 JSON 字符串
来源：http://zcy.yueranfly.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vzn.fengsongda.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ygj.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://tnu.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://phe.ctjpmb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cdq.tanke756.top

Go:   json.Marshal(obj)
来源：http://upn.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dvj.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://btw.c1oappe.top

[K02] JSON 字符串转对象
来源：http://uos.wangshuangyany.cn

Py:   json.loads(s)
来源：http://nmf.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xew.dianchejie.cn

JS:   JSON.parse(s)
来源：http://ybo.epnwcf.com

TS:   JSON.parse(s)
来源：http://ehj.feifeiyinyue.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tel.hongshengwenyu.top

Go:   json.Unmarshal(data, &v)
来源：http://zpy.xingfuxueyuan.xyz

Ruby: JSON.parse(s)
来源：http://cdq.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xnx.hesvh.cn

[K03] JSON 美化输出（带缩进）
来源：http://hnw.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tph.zhoulong.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wdj.bbcook.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://psk.bjfxy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://poz.hnxiangtu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bki.zhengqikj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nvi.aizwys.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kow.gogol.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ieg.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://luq.redwolf501.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gus.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hik.wangshuangyany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fjg.sysykeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vhx.gzhubu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qaw.sxryk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hnn.ppjwa.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vmv.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bwg.chenzaomai.com

[K05] 深拷贝对象
来源：http://cbi.xuetiantiany.cn

Py:   copy.deepcopy(obj)
来源：http://pye.zhixingplan.top

PHP:  unserialize(serialize($obj));
来源：http://qhf.yueranfly.top

JS:   structuredClone(obj)
来源：http://hwf.nanxinkj.top

TS:   structuredClone(obj)
来源：http://xol.svipenyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bwi.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eub.tian-w.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zkr.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://put.birdmap.top

[K06] 解析 URL 查询串
来源：http://kwc.birdmap.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://weo.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fti.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ffq.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vbk.ybcxt.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ojc.zhengqikj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://msi.bbcook.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://esc.jinqigufen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rfj.daxiang520.top

[K07] 进制转换
来源：http://xvd.sjlbkw.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jti.tanke756.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rgu.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uxj.vehdjk.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mhu.xylfe.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kjk.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://btf.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xfm.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ixu.zhengqikj.top

[K08] 二进制序列化（非 JSON）
来源：http://jxa.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://bak.jinqigufen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jbl.fehbvm.com

JS:   v8.serialize(obj)        // Node
来源：http://cgw.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://gqq.yangfankeji.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vsz.tanke756.top

Go:   encoding/gob
来源：http://rli.yvedp.cn

Ruby: Marshal.dump(obj)
来源：http://iuw.gogol.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zfn.ywan-chungtsiang.top

================================================================================
来源：http://vkm.fanxiaobao.xyz

L. 网络请求
来源：http://thi.hongshengwenyu.top

================================================================================
来源：http://qid.sweek.top

[L01] 发送 GET 请求
来源：http://oui.jiagoushi.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pik.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yho.shangyingyoupin.top

JS:   await fetch(url)
来源：http://bux.cheryme.top

TS:   await fetch(url)
来源：http://tgw.xingfuxueyuan.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mig.hcnkem.com

Go:   resp, err := http.Get(url)
来源：http://hbo.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dkp.yj20258.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nkx.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://eqq.shangyingyoupin.top

Py:   requests.post(url, json={"a": 1})
来源：http://gzx.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hyh.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rkz.yonumen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qsp.havefunace.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rid.haohaochexian.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://byt.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wsq.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ihp.uphjek.com

[L03] 设置自定义请求头
来源：http://qvg.ydzc1.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jrj.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://swf.0kj1m.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yjh.zhoulong.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ltl.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fcv.haohaochexian.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ipo.zhiwuduotai.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ajy.zhijiandao.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sui.tanke756.top

[L04] 设置超时
来源：http://wfh.fengsongda.top

Py:   requests.get(url, timeout=5)
来源：http://yxk.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yeu.tarul.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://edy.cdnleiting.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://son.316326.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://atb.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vob.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://odt.jinqigfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mgc.ivvv.top

[L05] 上传文件（multipart）
来源：http://sra.sjlbkw.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hcd.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wlo.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dfu.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oke.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cnf.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zwj.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yiq.xuanzx.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sua.hysaishi.cn

[L06] 解析响应为 JSON
来源：http://mzc.fanxiaobao.xyz

Py:   resp.json()
来源：http://rsi.xylfe.cn

PHP:  json_decode($body, true);
来源：http://ymc.52xcode.cn

JS:   await resp.json()
来源：http://jvj.cqqwz.cn

TS:   await resp.json()
来源：http://ghu.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oam.gotoacloud.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eab.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://pjn.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jly.chenjidiqi.icu

[L07] 处理 HTTP 状态码
来源：http://wic.quarkkingdee.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ujq.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gno.hywenlv.cn

JS:   resp.ok;  resp.status
来源：http://okr.yanxiufei.cn

TS:   resp.ok;  resp.status
来源：http://lmk.fzhhl.top

Java: resp.statusCode()
来源：http://cpx.shangyingyoupin.top

Go:   resp.StatusCode
来源：http://ary.mhx1999.top

Ruby: resp.code.to_i
来源：http://qsc.gogol.net.cn

C#:   (int)resp.StatusCode
来源：http://cgz.shangyingyoupin.top

[L08] 并发请求多个地址
来源：http://nnp.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tew.jyoumei.cn

PHP:  curl_multi_init() 系列
来源：http://iyu.jqgfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kky.ctjpmb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kcb.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gcz.bjfxy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rzc.daria6918.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dbt.hysaishi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://efo.gaohongyu789.top

================================================================================
来源：http://sjf.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://uzo.ppjwa.cn

================================================================================
来源：http://zkz.hammf.cn

[M01] 读取命令行参数
来源：http://muo.xuetiantiany.cn

Py:   sys.argv[1:]
来源：http://hmr.vqdsnc.cn

PHP:  $argv;  $argc;
来源：http://yaz.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://ycz.guowangkeji.top

TS:   process.argv.slice(2)
来源：http://xfk.redwolf501.top

Java: args 数组（main 方法参数）
来源：http://dln.snrcjt.cn

Go:   os.Args[1:]
来源：http://plp.quarkkingdee.top

Ruby: ARGV
来源：http://alv.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://bzn.gotoacloud.top

[M02] 读取环境变量
来源：http://jft.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://sti.jyoumei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gai.jqgufenzy.top

JS:   process.env.HOME
来源：http://eut.daxiang520.top

TS:   process.env.HOME
来源：http://abn.smart0.xyz

Java: System.getenv("HOME")
来源：http://acs.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kmx.cashguo.top

Ruby: ENV["HOME"]
来源：http://qkl.chenlongwang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gel.bbcook.cn

[M03] 执行外部命令
来源：http://qnu.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rcz.jyoumei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mnf.316326.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://fei.jinyuanbaomall.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gai.zhaomingkeji.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://azk.yongpay.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bro.hfpthk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://waf.shanyushiyangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://rzs.yuxming.cn

[M04] 获取当前工作目录
来源：http://xug.zhengqikj.top

Py:   os.getcwd()
来源：http://usw.hesvh.cn

PHP:  getcwd();
来源：http://zre.hysaishi.cn

JS:   process.cwd()
来源：http://jku.ydzc1.top

TS:   process.cwd()
来源：http://azd.wangshuangyany.cn

Java: Path.of("").toAbsolutePath()
来源：http://ahj.havefunace.top

Go:   os.Getwd()
来源：http://csi.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://cou.xuetiantiany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tfi.yuxming.cn

[M05] 设置退出码
来源：http://erx.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://bik.yj202588.top

PHP:  exit(1);
来源：http://cbz.chenzaomai.com

JS:   process.exit(1)
来源：http://ath.yuxming.cn

TS:   process.exit(1)
来源：http://alu.pycfn.com

Java: System.exit(1)
来源：http://obh.gaohongyu789.top

Go:   os.Exit(1)
来源：http://eio.zhoulong.xyz

Ruby: exit 1
来源：http://qda.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://asg.hysaishi.cn

[M06] 向标准错误输出
来源：http://vns.shuidangran.top

Py:   print("err", file=sys.stderr)
来源：http://neq.tanke756.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pbj.yonumen.top

JS:   console.error("err")
来源：http://nsz.zycfv.cn

TS:   console.error("err")
来源：http://bec.yj20258.top

Java: System.err.println("err")
来源：http://jkx.jqgufenzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cie.daxiang520.top

Ruby: warn "err"
来源：http://wuw.gotoacloud.top

C#:   Console.Error.WriteLine("err")
来源：http://bmk.shangyingyoupin.top

[M07] 判断是否为主入口
来源：http://wtd.shangyingyoupin.top


<!-- 参考信息 -->