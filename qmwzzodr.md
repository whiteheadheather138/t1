代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zhh.mhx1999.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pwn.vehdjk.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rvs.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qar.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://omk.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nqs.zdqjudy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nub.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://jpd.bjfxy.top

TS:   new Date("2024-01-02")
来源：http://wph.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qsy.zhongyouzk.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ais.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://jub.tanke756.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yxc.yongpay.top

[J04] 时间戳与日期互转
来源：http://kpq.yj20258888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ahd.xylfe.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cbe.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nwy.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dlc.tanke756.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hkf.tianlin.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sru.ehwqpu.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ldn.zhaomingkeji.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fng.jinqigufen.top

[J05] 时间加减（加 7 天）
来源：http://sep.redwolf501.top

Py:   now + timedelta(days=7)
来源：http://wti.xuetiantiany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lml.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qxx.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wzk.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://eux.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wzo.hnqzz.top

Ruby: Time.now + 7 * 86400
来源：http://hjz.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://poz.yongpay.top

[J06] 计算两时间之差
来源：http://csb.hammf.cn

Py:   (end - start).total_seconds()
来源：http://zfg.birdmap.top

PHP:  $end->diff($start)->days;
来源：http://fjz.xingfuxueyuan.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tdc.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://udb.birdmap.top

Java: Duration.between(start, end).toSeconds()
来源：http://pyz.c1oappe.top

Go:   end.Sub(start).Hours()
来源：http://fne.gogol.net.cn

Ruby: end - start                 # 返回秒数
来源：http://bgo.ywan-chungtsiang.top

C#:   (end - start).TotalSeconds
来源：http://nxm.daxiang520.top

[J07] 比较两个日期
来源：http://bum.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://sef.aibaodan.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xyh.ywan-chungtsiang.top

JS:   d1.getTime() < d2.getTime()
来源：http://vrp.hnxiangtu.top

TS:   d1.getTime() < d2.getTime()
来源：http://ozp.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gar.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gpe.xinyue.icu

Ruby: d1 < d2;  d1 == d2
来源：http://fvl.aibaodan.cn

C#:   d1 < d2;  d1 == d2
来源：http://lqa.ehwqpu.com

[J08] 提取年月日与星期
来源：http://dcz.hnxiangtu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bgi.wangshuangyany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kkx.epnwcf.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wou.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zro.xziqi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fpm.chenjidiqi.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ktt.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eiw.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gdf.hysaishi.cn

[J09] 时区处理
来源：http://rob.fehbvm.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hlv.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bng.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sih.jinyuanbaomall.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bok.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mib.mhx1999.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dyt.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://cei.cheryme.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fwn.xuetiantiany.cn

[J10] 取今天 / 本月第一天
来源：http://hjd.xziqi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bwe.aibaodan.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xxc.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jbk.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oip.xingfuxueyuan.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yzs.fktsv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mww.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ojt.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vvq.daria6918.cn

================================================================================
来源：http://txu.c1oappe.top

K. JSON 与序列化
来源：http://tjd.wangshuangyany.cn

================================================================================
来源：http://guo.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://nho.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://otq.redwolf501.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cwg.yongpay.top

JS:   JSON.stringify(obj)
来源：http://qkg.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://cnu.nanxinkj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://arh.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://zgj.yj202588.top

Ruby: obj.to_json                                     // require "json"
来源：http://wqx.chenlongwang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dfh.jinyuanbaomall.cn

[K02] JSON 字符串转对象
来源：http://ikn.hcnkem.com

Py:   json.loads(s)
来源：http://wmg.tanke756.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://btj.xylfe.cn

JS:   JSON.parse(s)
来源：http://vmo.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://iic.xziqi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qqy.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://nyp.sufxvd.cn

Ruby: JSON.parse(s)
来源：http://dtl.fzhhl.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oyu.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://wvc.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dof.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rmq.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fce.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://amo.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qpg.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nti.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://oii.gogol.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://khx.fktsv.cn

[K04] 读取 JSON 文件
来源：http://cvg.aibaodan.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cld.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nee.shanyushiyangtech.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qvd.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://quj.zycfv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mqm.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jna.fanxiaobao.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://xew.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nyp.guowangkeji.top

[K05] 深拷贝对象
来源：http://rhg.shuidangran.top

Py:   copy.deepcopy(obj)
来源：http://dow.jinyuanbaomall.cn

PHP:  unserialize(serialize($obj));
来源：http://smg.ehwqpu.com

JS:   structuredClone(obj)
来源：http://axz.ydjk.org.cn

TS:   structuredClone(obj)
来源：http://ozx.daria6918.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ppd.jinghuilouyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fkk.sxryk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cub.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://say.wangshuangyany.cn

[K06] 解析 URL 查询串
来源：http://ayw.cashguo.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yxy.ehwqpu.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dix.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tys.ywan-chungtsiang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cvw.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://luz.pycfn.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ocy.daria6918.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kqf.hysaishi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dxf.jinqigufen.top

[K07] 进制转换
来源：http://mpp.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bji.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cha.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fbk.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zxw.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zvp.haohaochexian.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xxt.gotoacloud.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://btc.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xam.0kj1m.cn

[K08] 二进制序列化（非 JSON）
来源：http://xqp.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://dzo.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sgy.yangfankeji.com

JS:   v8.serialize(obj)        // Node
来源：http://ukq.yj202588.top

TS:   v8.serialize(obj)        // Node
来源：http://yky.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uon.haohaochexian.top

Go:   encoding/gob
来源：http://cbd.shanyushiyangtech.top

Ruby: Marshal.dump(obj)
来源：http://xna.gogol.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cir.zhengqikj.top

================================================================================
来源：http://xfc.jyoumei.cn

L. 网络请求
来源：http://ffr.xuanzx.com

================================================================================
来源：http://pxu.chenzaomai.com

[L01] 发送 GET 请求
来源：http://vrb.shangyingyoupin.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pio.xinyue.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://urd.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://hcx.cqqwz.cn

TS:   await fetch(url)
来源：http://ida.birdmap.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://efw.zhijiandao.cn

Go:   resp, err := http.Get(url)
来源：http://ajp.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://usi.hysaishi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wrx.zycfv.cn

[L02] 发送 POST JSON
来源：http://bem.xingfuxueyuan.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://xhd.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://twk.hywenlv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ywk.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nve.yj20258.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://clv.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dkr.9152youxi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zvp.jianghu66.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wbj.shzxlz.cn

[L03] 设置自定义请求头
来源：http://myc.daria6918.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bmk.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://psg.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aae.nanxinkj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dxv.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hqp.yonumen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ebj.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fdu.bjfxy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cso.hongshengwenyu.top

[L04] 设置超时
来源：http://erz.hammf.cn

Py:   requests.get(url, timeout=5)
来源：http://gkg.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zal.quarkkingdee.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ohh.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xlt.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cjb.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://knd.xinyue.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://krj.smart0.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gfq.sweek.top

[L05] 上传文件（multipart）
来源：http://pij.aizwys.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ahe.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dfq.tianlin.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://beq.yfazqb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://usm.cqqwz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gut.smart0.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gdr.snrcjt.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://euz.daxiang520.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gpx.vqdsnc.cn

[L06] 解析响应为 JSON
来源：http://swt.hywenlv.cn

Py:   resp.json()
来源：http://gmf.fengsongda.top

PHP:  json_decode($body, true);
来源：http://sgc.0kj1m.cn

JS:   await resp.json()
来源：http://lir.yangfankeji.com

TS:   await resp.json()
来源：http://usm.yongpay.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zbm.shuidangran.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lof.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://jbf.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bzb.cqqwz.cn

[L07] 处理 HTTP 状态码
来源：http://mqi.tianlin.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://roa.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yrx.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://lwu.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://zoj.fanxiaobao.xyz

Java: resp.statusCode()
来源：http://ykr.cucudq.cn

Go:   resp.StatusCode
来源：http://ujk.zycfv.cn

Ruby: resp.code.to_i
来源：http://wfm.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://tto.sweek.top

[L08] 并发请求多个地址
来源：http://xnt.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ixn.hongshengwenyu.top

PHP:  curl_multi_init() 系列
来源：http://wsh.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vqi.yanxiufei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gnp.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qec.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qvb.cqqwz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://war.shuidangran.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hqp.nanxinkj.top

================================================================================
来源：http://zza.andypj.xyz

M. 命令行 / 进程 / 环境
来源：http://dzl.yanxiufei.cn

================================================================================
来源：http://nga.aibaodan.cn

[M01] 读取命令行参数
来源：http://ywu.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://van.cheryme.top

PHP:  $argv;  $argc;
来源：http://vzf.yongpay.top

JS:   process.argv.slice(2)
来源：http://lmv.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://tfm.jlsjyb.cn

Java: args 数组（main 方法参数）
来源：http://uwe.yueranfly.top

Go:   os.Args[1:]
来源：http://svx.andypj.xyz

Ruby: ARGV
来源：http://pfp.dianchejie.cn

C#:   args 数组（Main 方法参数）
来源：http://lll.xingfuxueyuan.xyz

[M02] 读取环境变量
来源：http://lor.nanxuanxn.top

Py:   os.environ.get("HOME")
来源：http://fza.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jno.fktsv.cn

JS:   process.env.HOME
来源：http://ems.cucudq.cn

TS:   process.env.HOME
来源：http://rly.jianghu66.top

Java: System.getenv("HOME")
来源：http://jzg.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ixb.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://sbi.vehdjk.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dej.sxryk.cn

[M03] 执行外部命令
来源：http://thd.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jnx.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bcs.aibaodan.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ymv.jianghu66.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hmt.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://saz.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://mup.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://vcd.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://myd.kuanghao11.cn

[M04] 获取当前工作目录
来源：http://jkd.havefunace.top

Py:   os.getcwd()
来源：http://xzo.jiagoushi.top

PHP:  getcwd();
来源：http://ext.xuetiantiany.cn

JS:   process.cwd()
来源：http://wyo.svipenyu.cn

TS:   process.cwd()
来源：http://zcs.cdnleiting.top

Java: Path.of("").toAbsolutePath()
来源：http://oyv.birdmap.top

Go:   os.Getwd()
来源：http://fxn.yueranfly.top

Ruby: Dir.pwd
来源：http://uwl.xylfe.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vmz.kuanghao11.cn

[M05] 设置退出码
来源：http://fii.aizwys.cn

Py:   sys.exit(1)
来源：http://qwv.ppjwa.cn

PHP:  exit(1);
来源：http://lnq.gotoacloud.top

JS:   process.exit(1)
来源：http://sam.chenjidiqi.icu

TS:   process.exit(1)
来源：http://wcn.smart0.xyz

Java: System.exit(1)
来源：http://xfh.dashuyun.cn

Go:   os.Exit(1)
来源：http://wda.wangshuangyany.cn

Ruby: exit 1
来源：http://tpe.yonumen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://htj.cashguo.top

[M06] 向标准错误输出
来源：http://pui.snrcjt.cn

Py:   print("err", file=sys.stderr)
来源：http://xwz.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fuj.c1oappe.top

JS:   console.error("err")
来源：http://xxl.fzhhl.top

TS:   console.error("err")
来源：http://dlz.pycfn.com

Java: System.err.println("err")
来源：http://ybx.tian-w.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gyx.jiagoushi.top

Ruby: warn "err"
来源：http://cup.andypj.xyz

C#:   Console.Error.WriteLine("err")
来源：http://dka.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://pgk.birdmap.top

Py:   if __name__ == "__main__":
来源：http://vkx.zhengqikj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zid.0kj1m.cn

JS:   require.main === module
来源：http://mhl.kuanghao11.cn

TS:   require.main === module
来源：http://wbd.cucudq.cn

Java: public static void main(String[] args)
来源：http://auc.zdbjq.cn

Go:   func main()
来源：http://cog.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qes.fehbvm.com

C#:   static void Main(string[] args)
来源：http://boh.jinqigufen.top

[M08] 获取系统与运行时信息
来源：http://uch.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://fwb.hywenlv.cn

PHP:  PHP_OS;  phpversion();
来源：http://vlu.yj20258.top

JS:   process.platform;  process.version
来源：http://grt.gaohongyu789.top

TS:   process.platform;  process.version
来源：http://ybu.fehbvm.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qlk.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://iup.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gch.ydjk.org.cn


<!-- 参考信息 -->