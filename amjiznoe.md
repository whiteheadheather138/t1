代发 wailian999

Go:   time.Now()
来源：http://moh.jinyuanbaomall.cn

Ruby: Time.now
来源：http://irg.fktsv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qht.fzhhl.top

[J02] 格式化输出
来源：http://mxm.hysaishi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://chv.9152youxi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bpl.ywan-chungtsiang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uts.hnqzz.top

TS:   d.toISOString()
来源：http://zik.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ssm.wangshuangyany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oxw.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://clz.jiagoushi.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cqp.zhengqikj.top

[J03] 字符串解析为日期
来源：http://ypw.hammf.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lyh.hfpthk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ywm.wangshuangyany.cn

JS:   new Date("2024-01-02")
来源：http://jyu.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://txq.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://sen.chenjidiqi.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ewl.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://nqt.cucudq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zzi.iojbl.cn

[J04] 时间戳与日期互转
来源：http://bah.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dyt.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://skh.wangshuangyany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ino.gzhubu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://btb.cucudq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kfm.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://har.zhixingplan.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://drl.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fzs.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://cvt.tian-w.cn

Py:   now + timedelta(days=7)
来源：http://uzf.hesvh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oho.quarkkingdee.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://imq.uphjek.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vqo.xuetiantiany.cn

Java: LocalDate.now().plusDays(7)
来源：http://jwe.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dwh.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://dai.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qno.jqgufenzy.top

[J06] 计算两时间之差
来源：http://bwi.uphjek.com

Py:   (end - start).total_seconds()
来源：http://fja.wangdashe.top

PHP:  $end->diff($start)->days;
来源：http://qnr.jiagoushi.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gek.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uxp.smart0.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://bzu.zhaomingkeji.xyz

Go:   end.Sub(start).Hours()
来源：http://gab.zdqjudy.top

Ruby: end - start                 # 返回秒数
来源：http://exx.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://cyx.andypj.xyz

[J07] 比较两个日期
来源：http://yrl.jqgfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://icx.aizwys.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://czi.cucudq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vox.zdqjudy.top

TS:   d1.getTime() < d2.getTime()
来源：http://ppl.zhongyouzk.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jcw.nwbrower.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ifx.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://mri.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://buy.fzhhl.top

[J08] 提取年月日与星期
来源：http://ajm.jinyuanbaomall.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wul.ppjwa.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://guh.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pny.ehwqpu.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tdf.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ptr.ydjk.org.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xhb.xylfe.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://phn.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yvw.yueranfly.top

[J09] 时区处理
来源：http://qdf.zhongyouzk.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xpf.kuanghao11.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rxs.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bfl.xingfuxueyuan.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yoz.epnwcf.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mwt.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eid.jiagoushi.top

Ruby: Time.now.getlocal("+08:00")
来源：http://squ.daria6918.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gcr.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://nxy.cdnleiting.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xmc.cucudq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bea.iojbl.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://msf.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gcz.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mbk.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xmv.fanxiaobao.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rtz.havefunace.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xro.hongshengwenyu.top

================================================================================
来源：http://byw.hnxiangtu.top

K. JSON 与序列化
来源：http://nsw.jqgfzy.top

================================================================================
来源：http://jrn.zhixingplan.top

[K01] 对象转 JSON 字符串
来源：http://kyb.aizwys.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bak.chenzaomai.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aoj.316326.xyz

JS:   JSON.stringify(obj)
来源：http://gtq.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://oge.quarkkingdee.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://onf.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://nut.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://hzp.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nnp.cucudq.cn

[K02] JSON 字符串转对象
来源：http://ljf.jiagoushi.top

Py:   json.loads(s)
来源：http://wos.xziqi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zvv.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://gjk.vqdsnc.cn

TS:   JSON.parse(s)
来源：http://xzq.sysykeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qop.shzxlz.cn

Go:   json.Unmarshal(data, &v)
来源：http://zyg.yuanzhike.top

Ruby: JSON.parse(s)
来源：http://lee.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://psb.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://ifo.yueranfly.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xya.fengsongda.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lvo.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pkt.9152youxi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fpd.zhixingplan.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nrz.havefunace.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://stt.hnxiangtu.top

Ruby: JSON.pretty_generate(obj)
来源：http://dun.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rxz.guowangkeji.top

[K04] 读取 JSON 文件
来源：http://ueo.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tiq.sjlbkw.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zhc.svipenyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jwx.mhx1999.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dcq.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gdb.jyoumei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fxe.yuanzhike.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lpx.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wxh.jyoumei.cn

[K05] 深拷贝对象
来源：http://xjc.cqqwz.cn

Py:   copy.deepcopy(obj)
来源：http://cpn.cdnleiting.top

PHP:  unserialize(serialize($obj));
来源：http://oma.zhixingplan.top

JS:   structuredClone(obj)
来源：http://elv.hywenlv.cn

TS:   structuredClone(obj)
来源：http://wej.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yvn.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bgs.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lqa.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hau.andypj.xyz

[K06] 解析 URL 查询串
来源：http://bdu.fktsv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lfk.ehwqpu.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qgs.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yvy.svipenyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jvr.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ohc.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lcg.hammf.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qqw.jinyuanbaomall.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oxw.gzhubu.top

[K07] 进制转换
来源：http://qsv.0kj1m.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sef.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://evg.fktsv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ihm.iojbl.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hdv.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://niz.xuanzx.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pvm.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hxv.jinghuilouyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bcl.feifeiyinyue.top

[K08] 二进制序列化（非 JSON）
来源：http://sqy.wangdashe.top

Py:   pickle.dumps(obj)
来源：http://iyh.tarul.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://abh.epnwcf.com

JS:   v8.serialize(obj)        // Node
来源：http://frc.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://oiv.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kof.vqdsnc.cn

Go:   encoding/gob
来源：http://tud.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://szx.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zvt.gogol.net.cn

================================================================================
来源：http://ehk.shanyushiyangtech.top

L. 网络请求
来源：http://zce.shanyushiyangkeji.top

================================================================================
来源：http://gpt.jiagoushi.top

[L01] 发送 GET 请求
来源：http://ebz.mhx1999.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fze.hnxiangtu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jqa.gzhubu.top

JS:   await fetch(url)
来源：http://ovt.havefunace.top

TS:   await fetch(url)
来源：http://bcb.sxryk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zog.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://bnh.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://sdo.haohaochexian.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kwk.jiagoushi.top

[L02] 发送 POST JSON
来源：http://afv.hongshengwenyu.top

Py:   requests.post(url, json={"a": 1})
来源：http://ccq.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mkn.sjlbkw.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ljn.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fco.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vpf.nanxuanxn.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://loy.cdnleiting.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lkh.quarkkingdee.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wtt.jqgufenzy.top

[L03] 设置自定义请求头
来源：http://dav.yueranfly.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vlf.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ukr.jinqigfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://idf.chenjidiqi.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://syb.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nnt.xingfuxueyuan.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nvv.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yed.havefunace.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mgi.shangyingyoupin.top

[L04] 设置超时
来源：http://mjq.gaohongyu789.top

Py:   requests.get(url, timeout=5)
来源：http://qpu.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kzk.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vul.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ktp.cashguo.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rtd.ivvv.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pvc.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://svg.chenzaomai.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fxc.zhiwuduotai.top

[L05] 上传文件（multipart）
来源：http://icr.nanxinkj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ffp.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ykb.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lcv.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ujs.gzhubu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mpl.0kj1m.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wuq.daxiang520.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ydv.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://znj.jinghuilouyu.cn

[L06] 解析响应为 JSON
来源：http://nrx.zhoulong.xyz

Py:   resp.json()
来源：http://iha.hammf.cn

PHP:  json_decode($body, true);
来源：http://cvl.ybcxt.top

JS:   await resp.json()
来源：http://sli.xuanzx.com

TS:   await resp.json()
来源：http://ixo.hammf.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eyr.sxryk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pfm.jinqigufen.top

Ruby: JSON.parse(resp.body)
来源：http://xzy.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://erw.zdqjudy.top

[L07] 处理 HTTP 状态码
来源：http://yvn.jinyuanbaomall.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ijs.shzxlz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oaz.yangfankeji.com

JS:   resp.ok;  resp.status
来源：http://qhg.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://hah.dashuyun.cn

Java: resp.statusCode()
来源：http://kcz.pycfn.com

Go:   resp.StatusCode
来源：http://zpi.zhiwuduotai.top

Ruby: resp.code.to_i
来源：http://uos.ivvv.top

C#:   (int)resp.StatusCode
来源：http://dmc.ydjk.org.cn

[L08] 并发请求多个地址
来源：http://pdd.nanxuanxn.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sdz.yanxiufei.cn

PHP:  curl_multi_init() 系列
来源：http://inv.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rcm.tianlin.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xub.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qec.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ykw.hnxiangtu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rmb.hnqzz.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://buk.fzhhl.top

================================================================================
来源：http://kis.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://hnt.hnqzz.top

================================================================================
来源：http://mnb.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://rkg.ehwqpu.com

Py:   sys.argv[1:]
来源：http://flo.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://dmt.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://brh.c1oappe.top

TS:   process.argv.slice(2)
来源：http://wqo.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://xep.bbcook.cn

Go:   os.Args[1:]
来源：http://tsd.fehbvm.com

Ruby: ARGV
来源：http://swt.tanke756.top

C#:   args 数组（Main 方法参数）
来源：http://nnl.yuxming.cn

[M02] 读取环境变量
来源：http://gwf.dashuyun.cn

Py:   os.environ.get("HOME")
来源：http://bfd.52xcode.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://itm.shangyingyoupin.top

JS:   process.env.HOME
来源：http://nfc.hesvh.cn

TS:   process.env.HOME
来源：http://ayx.gaohongyu789.top

Java: System.getenv("HOME")
来源：http://rgw.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uqe.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://dln.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://owr.sweek.top

[M03] 执行外部命令
来源：http://zlb.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qqa.gotoacloud.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://egy.tarul.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wfn.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://rgq.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ggx.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vls.xuetiantiany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ewj.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://wtt.yuanzhike.top

[M04] 获取当前工作目录
来源：http://suv.hfpthk.cn

Py:   os.getcwd()
来源：http://mig.ywan-chungtsiang.top

PHP:  getcwd();
来源：http://rcv.yonumen.top

JS:   process.cwd()
来源：http://ubr.aibaodan.cn

TS:   process.cwd()
来源：http://kwm.nwbrower.top

Java: Path.of("").toAbsolutePath()
来源：http://pyu.yuanzhike.top

Go:   os.Getwd()
来源：http://oau.hfpthk.cn

Ruby: Dir.pwd
来源：http://fau.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iqv.hammf.cn

[M05] 设置退出码
来源：http://eor.zhongyouzk.top

Py:   sys.exit(1)
来源：http://vbr.hywenlv.cn

PHP:  exit(1);
来源：http://tsw.jinqigufen.top

JS:   process.exit(1)
来源：http://xdo.wangshuangyany.cn

TS:   process.exit(1)
来源：http://pbs.xziqi.cn

Java: System.exit(1)
来源：http://tvf.dashuyun.cn

Go:   os.Exit(1)
来源：http://dyb.zdqjudy.top

Ruby: exit 1
来源：http://vga.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dyx.ybcxt.top

[M06] 向标准错误输出
来源：http://ejn.zhiwuduotai.top

Py:   print("err", file=sys.stderr)
来源：http://dvq.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://gvg.jinghuilouyu.cn

JS:   console.error("err")
来源：http://kax.tian-w.cn

TS:   console.error("err")
来源：http://viz.yj202588.top

Java: System.err.println("err")
来源：http://vgs.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bdi.nanxinkj.top

Ruby: warn "err"
来源：http://yqy.bbcook.cn

C#:   Console.Error.WriteLine("err")
来源：http://svj.dianchejie.cn

[M07] 判断是否为主入口
来源：http://sas.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://mbw.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xhx.gaohongyu789.top

JS:   require.main === module
来源：http://snh.sjlbkw.cn

TS:   require.main === module
来源：http://fic.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://syz.52xcode.cn

Go:   func main()
来源：http://haf.ehwqpu.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jck.gogol.net.cn

C#:   static void Main(string[] args)
来源：http://exv.shanyushiyangtech.top


<!-- 参考信息 -->