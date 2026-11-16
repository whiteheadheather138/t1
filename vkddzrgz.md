代发 wailian999

J. 日期与时间
来源：http://mrx.yj202588.top

================================================================================
来源：http://ulx.tian-w.cn

[J01] 获取当前时间
来源：http://bta.vqdsnc.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rfe.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fpi.fanxiaobao.xyz

JS:   new Date();  Date.now()
来源：http://ewi.tian-w.cn

TS:   new Date();  Date.now()
来源：http://rbs.aibaodan.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vbo.yonumen.top

Go:   time.Now()
来源：http://uph.sysykeji.top

Ruby: Time.now
来源：http://odj.yj202588.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sts.jinghuilouyu.cn

[J02] 格式化输出
来源：http://akv.ivvv.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lyl.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xpv.epnwcf.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ijw.daxiang520.top

TS:   d.toISOString()
来源：http://pxr.hnqzz.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dqh.dianchejie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gtq.hywenlv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wtp.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pog.zdbjq.cn

[J03] 字符串解析为日期
来源：http://zfa.yanxiufei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qnj.aizwys.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ovv.tian-w.cn

JS:   new Date("2024-01-02")
来源：http://awu.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://eoz.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://ekh.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ojy.yuanzhike.top

Ruby: Date.parse("2024-01-02")
来源：http://fyy.guannengcc.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tbv.hcnkem.com

[J04] 时间戳与日期互转
来源：http://hkn.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://prd.pengpengdd.cyou

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lab.ivvv.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://odx.vehdjk.com

TS:   Math.floor(Date.now() / 1000)
来源：http://luy.zhijiandao.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://luf.nanxuanxn.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jfb.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bym.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qdp.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://wkn.316326.xyz

Py:   now + timedelta(days=7)
来源：http://zbb.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xkb.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zyd.zycfv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://buv.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://rrl.xuetiantiany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xdj.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://cje.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tub.shanyushiyangkeji.top

[J06] 计算两时间之差
来源：http://tzs.vehdjk.com

Py:   (end - start).total_seconds()
来源：http://udy.zycfv.cn

PHP:  $end->diff($start)->days;
来源：http://jhg.gogol.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wph.meibo888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://now.jiagoushi.top

Java: Duration.between(start, end).toSeconds()
来源：http://mlm.sxryk.cn

Go:   end.Sub(start).Hours()
来源：http://wxl.fengsongda.top

Ruby: end - start                 # 返回秒数
来源：http://qcv.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://rte.kuanghao11.cn

[J07] 比较两个日期
来源：http://rck.dianchejie.cn

Py:   d1 < d2;  d1 == d2
来源：http://spg.jinghuilouyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vwm.c1oappe.top

JS:   d1.getTime() < d2.getTime()
来源：http://xkk.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://goh.zycfv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ujn.ctjpmb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mii.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://ynr.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://lfd.316326.xyz

[J08] 提取年月日与星期
来源：http://uka.fanxiaobao.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mba.yj20258.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pgq.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://krx.xuanzx.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lct.tian-w.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xun.zdbjq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://khv.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vbj.wangshuangyany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zgi.chenlongwang.top

[J09] 时区处理
来源：http://ztl.yanxiufei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vxn.jinqigufen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wec.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wcr.fehbvm.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mpt.ctjpmb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://scf.zhiwuduotai.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://veb.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cvl.gotoacloud.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iuu.fzhhl.top

[J10] 取今天 / 本月第一天
来源：http://syk.jinqigfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ovu.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ozm.xingfuxueyuan.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://elt.uphjek.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wou.xylfe.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://stl.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sgt.c1oappe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yin.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kvq.nanxinkj.top

================================================================================
来源：http://jzv.jqgfzy.top

K. JSON 与序列化
来源：http://zey.nanxuanxn.top

================================================================================
来源：http://mvr.jinghuilouyu.cn

[K01] 对象转 JSON 字符串
来源：http://mjr.zdbjq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wjv.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qbp.yfazqb.com

JS:   JSON.stringify(obj)
来源：http://ira.ehwqpu.com

TS:   JSON.stringify(obj)
来源：http://knq.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vcs.ybcxt.top

Go:   json.Marshal(obj)
来源：http://xod.dashuyun.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tei.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rrd.andypj.xyz

[K02] JSON 字符串转对象
来源：http://snv.hnxiangtu.top

Py:   json.loads(s)
来源：http://dqr.hnxiangtu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ccj.yongpay.top

JS:   JSON.parse(s)
来源：http://rve.havefunace.top

TS:   JSON.parse(s)
来源：http://liu.tianlin.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jjj.redwolf501.top

Go:   json.Unmarshal(data, &v)
来源：http://jtr.fehbvm.com

Ruby: JSON.parse(s)
来源：http://zur.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cro.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://rak.sjlbkw.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ler.bjfxy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ndm.sweek.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tds.yongpay.top

TS:   JSON.stringify(obj, null, 2)
来源：http://eur.zhengqikj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nqb.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gir.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xcg.meibo888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uni.hnqzz.top

[K04] 读取 JSON 文件
来源：http://okq.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ljr.sxryk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tej.bbcook.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ixr.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fsl.pycfn.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://old.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gbx.jlsjyb.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://axg.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nlf.ppjwa.cn

[K05] 深拷贝对象
来源：http://sds.tarul.cn

Py:   copy.deepcopy(obj)
来源：http://ivz.jlsjyb.cn

PHP:  unserialize(serialize($obj));
来源：http://izz.yangfankeji.com

JS:   structuredClone(obj)
来源：http://wqh.smart0.xyz

TS:   structuredClone(obj)
来源：http://dhi.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://htl.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://god.fzhhl.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nnc.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://hib.nwbrower.top

[K06] 解析 URL 查询串
来源：http://scz.zdqjudy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vby.zhengqikj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iff.zhoulong.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qax.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dcc.hfpthk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ybc.ywan-chungtsiang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wsb.gaohongyu789.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nln.aibaodan.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lwz.chenzaomai.com

[K07] 进制转换
来源：http://xat.bbcook.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cjz.kuanghao11.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://muv.sufxvd.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vgg.uphjek.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pjg.xuetiantiany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jmq.sjlbkw.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pfc.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rhm.iojbl.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cqu.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://ryg.epnwcf.com

Py:   pickle.dumps(obj)
来源：http://ada.hongshengwenyu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nin.jqgfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://apx.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://ulm.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://owh.yj20258.top

Go:   encoding/gob
来源：http://cjy.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://drn.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xei.jinqigfzy.top

================================================================================
来源：http://gze.feifeiyinyue.top

L. 网络请求
来源：http://lia.gotoacloud.top

================================================================================
来源：http://jkz.pycfn.com

[L01] 发送 GET 请求
来源：http://ymx.shanyushiyangtech.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mel.shanyushiyangtech.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://alo.fehbvm.com

JS:   await fetch(url)
来源：http://vcd.xylfe.cn

TS:   await fetch(url)
来源：http://pbe.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ncu.gotoacloud.top

Go:   resp, err := http.Get(url)
来源：http://pwu.smart0.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://pwl.yj20258.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://odz.tanke756.top

[L02] 发送 POST JSON
来源：http://pue.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://rjk.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mni.meibo888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://brx.cashguo.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mzx.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zzu.jinghuilouyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jqd.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qkz.dashuyun.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fly.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://fqz.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ewc.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zsj.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xwt.chenjidiqi.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eqa.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jrm.shanyushiyangtech.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mzv.chenlongwang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ald.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mmk.snrcjt.cn

[L04] 设置超时
来源：http://ilb.zhixingplan.top

Py:   requests.get(url, timeout=5)
来源：http://nww.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dck.zdbjq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jzj.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mdz.birdmap.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lut.jinqigufen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zhh.zdbjq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mle.meibo888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bju.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://tws.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oga.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ijo.ybcxt.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://imo.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ubp.kuanghao11.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://egn.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zho.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ljq.shuidangran.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wbe.hammf.cn

[L06] 解析响应为 JSON
来源：http://pav.nanxuanxn.top

Py:   resp.json()
来源：http://aqs.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://lok.jyoumei.cn

JS:   await resp.json()
来源：http://sux.zycfv.cn

TS:   await resp.json()
来源：http://rnk.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bxb.ywan-chungtsiang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xal.aibaodan.cn

Ruby: JSON.parse(resp.body)
来源：http://lxt.zycfv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://veu.xuetiantiany.cn

[L07] 处理 HTTP 状态码
来源：http://sto.snrcjt.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cwk.ydzc1.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jcc.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://imm.hnxiangtu.top

TS:   resp.ok;  resp.status
来源：http://hak.yj202588.top

Java: resp.statusCode()
来源：http://anl.meibo888.top

Go:   resp.StatusCode
来源：http://spw.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://hhx.quarkkingdee.top

C#:   (int)resp.StatusCode
来源：http://ntk.ywan-chungtsiang.top

[L08] 并发请求多个地址
来源：http://wgd.hesvh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vdm.nanxinkj.top

PHP:  curl_multi_init() 系列
来源：http://vqc.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uox.jianghu66.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://opa.yj202588.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ckh.redwolf501.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uod.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fpw.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kfg.kuanghao11.cn

================================================================================
来源：http://dzn.shanyushiyangtech.top

M. 命令行 / 进程 / 环境
来源：http://frx.fengsongda.top

================================================================================
来源：http://sjg.birdmap.top

[M01] 读取命令行参数
来源：http://yit.hcnkem.com

Py:   sys.argv[1:]
来源：http://aqn.ctjpmb.com

PHP:  $argv;  $argc;
来源：http://nby.daxiang520.top

JS:   process.argv.slice(2)
来源：http://kia.jinqigfzy.top

TS:   process.argv.slice(2)
来源：http://qsj.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://wcz.hnxiangtu.top

Go:   os.Args[1:]
来源：http://aes.hysaishi.cn

Ruby: ARGV
来源：http://mjv.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://dqp.yj202588.top

[M02] 读取环境变量
来源：http://ide.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://zjf.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://obx.nanxinkj.top

JS:   process.env.HOME
来源：http://ycl.yvedp.cn

TS:   process.env.HOME
来源：http://nzd.9152youxi.cn

Java: System.getenv("HOME")
来源：http://jbo.hnxiangtu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://esy.dashuyun.cn

Ruby: ENV["HOME"]
来源：http://oqo.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uns.hnqzz.top

[M03] 执行外部命令
来源：http://mpo.hnqzz.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://edb.yanxiufei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ken.aizwys.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lsr.daxiang520.top

TS:   child_process.execSync("ls -l").toString()
来源：http://daa.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mmg.hnqzz.top

Go:   exec.Command("ls", "-l").Output()
来源：http://son.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://nhc.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://xvu.wangdashe.top

[M04] 获取当前工作目录
来源：http://pll.gotoacloud.top

Py:   os.getcwd()
来源：http://lrs.yj202588.top

PHP:  getcwd();
来源：http://tgq.ehwqpu.com

JS:   process.cwd()
来源：http://erm.jinghuilouyu.cn

TS:   process.cwd()
来源：http://xow.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://wkt.chenjidiqi.icu

Go:   os.Getwd()
来源：http://hsk.yonumen.top

Ruby: Dir.pwd
来源：http://bsg.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tqy.jianghu66.top

[M05] 设置退出码
来源：http://zle.jqgfzy.top

Py:   sys.exit(1)
来源：http://mzn.jqgfzy.top

PHP:  exit(1);
来源：http://afx.nanxuanxn.top

JS:   process.exit(1)
来源：http://fve.shuidangran.top

TS:   process.exit(1)
来源：http://dgv.aizwys.cn

Java: System.exit(1)
来源：http://sgq.yvedp.cn

Go:   os.Exit(1)
来源：http://qlg.jqgfzy.top

Ruby: exit 1
来源：http://rhf.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xsh.jqgfzy.top

[M06] 向标准错误输出
来源：http://rxj.jyoumei.cn

Py:   print("err", file=sys.stderr)
来源：http://vgu.xylfe.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xrv.jqgufenzy.top

JS:   console.error("err")
来源：http://fhu.sysykeji.top

TS:   console.error("err")
来源：http://ihp.shuidangran.top

Java: System.err.println("err")
来源：http://izz.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hhk.xingfuxueyuan.xyz

Ruby: warn "err"
来源：http://roq.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://vtn.zhijiandao.cn

[M07] 判断是否为主入口
来源：http://gwo.yj20258888.top


<!-- 参考信息 -->