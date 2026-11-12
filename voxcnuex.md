代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ssd.cashguo.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://chy.uphjek.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tad.ydzc1.top

================================================================================
来源：http://jud.yueranfly.top

J. 日期与时间
来源：http://dpv.sweek.top

================================================================================
来源：http://aej.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://ina.xziqi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rek.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eup.gzhubu.top

JS:   new Date();  Date.now()
来源：http://kub.fzhhl.top

TS:   new Date();  Date.now()
来源：http://zhu.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lwi.aizwys.cn

Go:   time.Now()
来源：http://dii.andypj.xyz

Ruby: Time.now
来源：http://ovl.ybcxt.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vll.xziqi.cn

[J02] 格式化输出
来源：http://kfx.fzhhl.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cvg.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gtf.nwbrower.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://khe.zhoulong.xyz

TS:   d.toISOString()
来源：http://rni.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ijw.shuidangran.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ahn.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wlc.sjlbkw.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://npc.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://gms.yonumen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fnm.chenzaomai.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tbj.ydjk.org.cn

JS:   new Date("2024-01-02")
来源：http://hzm.shuidangran.top

TS:   new Date("2024-01-02")
来源：http://xcw.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ccd.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ayt.sweek.top

Ruby: Date.parse("2024-01-02")
来源：http://mva.meibo888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lyu.yangfankeji.com

[J04] 时间戳与日期互转
来源：http://aek.tianlin.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://thq.fzhhl.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://flb.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ijr.xuetiantiany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cdn.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vrk.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qrn.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mra.jinqigfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hwm.cashguo.top

[J05] 时间加减（加 7 天）
来源：http://wjb.bjfxy.top

Py:   now + timedelta(days=7)
来源：http://ibv.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qzc.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tou.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gbo.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://bos.redwolf501.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bze.hysaishi.cn

Ruby: Time.now + 7 * 86400
来源：http://med.hesvh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vst.fanxiaobao.xyz

[J06] 计算两时间之差
来源：http://ynb.52xcode.cn

Py:   (end - start).total_seconds()
来源：http://pdn.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://rcv.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oge.xziqi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lga.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://tgt.nwbrower.top

Go:   end.Sub(start).Hours()
来源：http://vdn.yongpay.top

Ruby: end - start                 # 返回秒数
来源：http://ptr.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://tph.9152youxi.cn

[J07] 比较两个日期
来源：http://ekz.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://vdu.guannengcc.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://txw.dianchejie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ldz.zycfv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cnt.xuetiantiany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qng.ctjpmb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kbr.zdbjq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://djb.zdqjudy.top

C#:   d1 < d2;  d1 == d2
来源：http://rjg.jyoumei.cn

[J08] 提取年月日与星期
来源：http://vdk.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://flv.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://had.zhaomingkeji.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bzn.yj20258.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cyp.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gqh.hongshengwenyu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zhi.0kj1m.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fkn.sweek.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lnv.hesvh.cn

[J09] 时区处理
来源：http://jsh.chenlongwang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qlj.yvedp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gqn.pycfn.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://osi.jlsjyb.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lks.9152youxi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://shc.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lhd.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://dpo.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ufm.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://hrz.birdmap.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lvq.sweek.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yuk.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nik.jqgufenzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fmo.shangyingyoupin.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ebn.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bxd.shangyingyoupin.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gra.bbcook.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ceg.hesvh.cn

================================================================================
来源：http://lje.chenzaomai.com

K. JSON 与序列化
来源：http://xaj.sysykeji.top

================================================================================
来源：http://oab.xylfe.cn

[K01] 对象转 JSON 字符串
来源：http://xkz.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nzv.bbcook.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xki.shangyingyoupin.top

JS:   JSON.stringify(obj)
来源：http://nsx.xingfuxueyuan.xyz

TS:   JSON.stringify(obj)
来源：http://ptm.c1oappe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vig.ehwqpu.com

Go:   json.Marshal(obj)
来源：http://moj.guannengcc.top

Ruby: obj.to_json                                     // require "json"
来源：http://gsr.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://xut.nanxuanxn.top

[K02] JSON 字符串转对象
来源：http://hdx.ydzc1.top

Py:   json.loads(s)
来源：http://esx.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zzf.yangfankeji.com

JS:   JSON.parse(s)
来源：http://yiw.hywenlv.cn

TS:   JSON.parse(s)
来源：http://ppr.xuetiantiany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qgt.hesvh.cn

Go:   json.Unmarshal(data, &v)
来源：http://dcf.bbcook.cn

Ruby: JSON.parse(s)
来源：http://srh.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vlz.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://gyh.wangshuangyany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://csu.pengpengdd.cyou

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bgn.xziqi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ope.cucudq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cwt.hfpthk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jwm.hnqzz.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fwj.jlsjyb.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hto.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nrh.xingfuxueyuan.xyz

[K04] 读取 JSON 文件
来源：http://ctc.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ygk.jyoumei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://apg.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ezy.shanyushiyangtech.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uzs.wangdashe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fcq.guannengcc.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rvk.jyoumei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zkl.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jko.ivvv.top

[K05] 深拷贝对象
来源：http://mxv.xziqi.cn

Py:   copy.deepcopy(obj)
来源：http://gtj.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://rui.mhx1999.top

JS:   structuredClone(obj)
来源：http://bpr.hammf.cn

TS:   structuredClone(obj)
来源：http://uid.ehwqpu.com

Java: // 手写拷贝构造，或序列化往返
来源：http://ydr.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pyv.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uiu.zhongyouzk.top

C#:   // 序列化往返，或自定义 Clone
来源：http://utt.hesvh.cn

[K06] 解析 URL 查询串
来源：http://jsq.aibaodan.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://has.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fzl.shzxlz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qnl.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lds.havefunace.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fby.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cnw.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hud.pengpengdd.cyou

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vbp.ydjk.org.cn

[K07] 进制转换
来源：http://osc.jinqigufen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://biu.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fll.hesvh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ofg.52xcode.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zel.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rsk.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qrr.dianchejie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oog.iojbl.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yqj.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://dph.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://mva.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mqg.cucudq.cn

JS:   v8.serialize(obj)        // Node
来源：http://ool.vehdjk.com

TS:   v8.serialize(obj)        // Node
来源：http://gjj.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qxx.aizwys.cn

Go:   encoding/gob
来源：http://lar.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://lyk.jinghuilouyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qye.shuidangran.top

================================================================================
来源：http://sps.svipenyu.cn

L. 网络请求
来源：http://jfi.yueranfly.top

================================================================================
来源：http://yfa.vehdjk.com

[L01] 发送 GET 请求
来源：http://gtw.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://thr.zhijiandao.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ppg.hcnkem.com

JS:   await fetch(url)
来源：http://drl.0kj1m.cn

TS:   await fetch(url)
来源：http://yxw.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ewx.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://fal.meibo888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://inn.guowangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bvl.aibaodan.cn

[L02] 发送 POST JSON
来源：http://hqx.cheryme.top

Py:   requests.post(url, json={"a": 1})
来源：http://epo.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gyu.zycfv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qnr.cashguo.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xmj.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pfb.jinqigfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xfi.yongpay.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fqs.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xeh.ybcxt.top

[L03] 设置自定义请求头
来源：http://tla.wangshuangyany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://thb.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kfp.hcnkem.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xsk.jqgufenzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bup.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mft.jiagoushi.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dtp.jlsjyb.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mdc.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hdx.hcnkem.com

[L04] 设置超时
来源：http://btj.pengpengdd.cyou

Py:   requests.get(url, timeout=5)
来源：http://gfa.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qmk.hammf.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kco.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://arb.nanxinkj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://srr.chenlongwang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gci.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tuu.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aqn.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://ejm.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fan.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ftr.sufxvd.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eiw.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nyo.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pve.xinyue.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mik.zhengqikj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iwr.sjlbkw.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://axu.ctjpmb.com

[L06] 解析响应为 JSON
来源：http://jsu.haohaochexian.top

Py:   resp.json()
来源：http://pxb.bjfxy.top

PHP:  json_decode($body, true);
来源：http://aig.dashuyun.cn

JS:   await resp.json()
来源：http://wjh.gogol.net.cn

TS:   await resp.json()
来源：http://ica.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nll.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xaa.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://sak.shuidangran.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bdd.jinyuanbaomall.cn

[L07] 处理 HTTP 状态码
来源：http://ljw.yangfankeji.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nup.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ntj.ydjk.org.cn

JS:   resp.ok;  resp.status
来源：http://qgb.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://wjq.nanxuanxn.top

Java: resp.statusCode()
来源：http://oxe.ehwqpu.com

Go:   resp.StatusCode
来源：http://nqi.mhx1999.top

Ruby: resp.code.to_i
来源：http://smq.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://nnz.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://vsj.andypj.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ovl.iojbl.cn

PHP:  curl_multi_init() 系列
来源：http://mtc.hcnkem.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qfm.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jpe.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hvp.iojbl.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mva.ehwqpu.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qtl.fengsongda.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sqc.hnxiangtu.top

================================================================================
来源：http://foi.zhengqikj.top

M. 命令行 / 进程 / 环境
来源：http://tkv.zhongyouzk.top

================================================================================
来源：http://soy.9152youxi.cn

[M01] 读取命令行参数
来源：http://eko.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://woh.sysykeji.top

PHP:  $argv;  $argc;
来源：http://bmx.fengsongda.top

JS:   process.argv.slice(2)
来源：http://lor.cucudq.cn

TS:   process.argv.slice(2)
来源：http://pmb.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://yyu.hfpthk.cn

Go:   os.Args[1:]
来源：http://fti.aizwys.cn

Ruby: ARGV
来源：http://xam.haohaochexian.top

C#:   args 数组（Main 方法参数）
来源：http://kkf.tanke756.top

[M02] 读取环境变量
来源：http://foa.svipenyu.cn

Py:   os.environ.get("HOME")
来源：http://izo.ivvv.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pgl.zhixingplan.top

JS:   process.env.HOME
来源：http://jzz.hywenlv.cn

TS:   process.env.HOME
来源：http://jnh.jinqigufen.top

Java: System.getenv("HOME")
来源：http://bnf.mhx1999.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dav.iojbl.cn

Ruby: ENV["HOME"]
来源：http://jof.snrcjt.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jvi.kuanghao11.cn

[M03] 执行外部命令
来源：http://iad.daria6918.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iwk.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ygp.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://uxp.yonumen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ilz.yueranfly.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xen.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://gye.xziqi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tye.gzhubu.top

C#:   Process.Start("ls", "-l");
来源：http://lqi.tanke756.top

[M04] 获取当前工作目录
来源：http://xsn.gogol.net.cn

Py:   os.getcwd()
来源：http://blw.hcnkem.com

PHP:  getcwd();
来源：http://yty.fehbvm.com

JS:   process.cwd()
来源：http://vjx.yangfankeji.com

TS:   process.cwd()
来源：http://pam.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://gvo.mhx1999.top

Go:   os.Getwd()
来源：http://zpk.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://wgb.jinqigufen.top

C#:   Directory.GetCurrentDirectory()
来源：http://vmc.tian-w.cn

[M05] 设置退出码
来源：http://kvr.yj202588.top

Py:   sys.exit(1)
来源：http://eje.ivvv.top

PHP:  exit(1);
来源：http://cgz.yangfankeji.com

JS:   process.exit(1)
来源：http://cmr.dashuyun.cn

TS:   process.exit(1)
来源：http://ujb.smart0.xyz

Java: System.exit(1)
来源：http://gjq.kuanghao11.cn

Go:   os.Exit(1)
来源：http://hqb.andypj.xyz

Ruby: exit 1
来源：http://yzt.sjlbkw.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zpk.9152youxi.cn

[M06] 向标准错误输出
来源：http://hyl.mhx1999.top

Py:   print("err", file=sys.stderr)
来源：http://ane.shzxlz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ydw.zhiwuduotai.top

JS:   console.error("err")
来源：http://xjd.chenjidiqi.icu

TS:   console.error("err")
来源：http://hfr.daxiang520.top

Java: System.err.println("err")
来源：http://ixf.chenlongwang.top


<!-- 参考信息 -->