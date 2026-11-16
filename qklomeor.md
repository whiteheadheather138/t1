代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jcu.shanyushiyangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hve.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nna.xinyue.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nrl.zhengqikj.top

[J03] 字符串解析为日期
来源：http://qfd.epnwcf.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://djc.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xzt.hnxiangtu.top

JS:   new Date("2024-01-02")
来源：http://iqk.tianlin.xyz

TS:   new Date("2024-01-02")
来源：http://eqm.zycfv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://omz.ybcxt.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zqn.sufxvd.cn

Ruby: Date.parse("2024-01-02")
来源：http://qqp.zhoulong.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dnr.tian-w.cn

[J04] 时间戳与日期互转
来源：http://rgr.jqgfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://axc.xingfuxueyuan.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pwk.yanxiufei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pst.nwbrower.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nyt.yj20258.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://opi.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vkm.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tyb.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gnm.daria6918.cn

[J05] 时间加减（加 7 天）
来源：http://skc.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://syt.mhx1999.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qtw.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wgs.yonumen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iab.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://nwf.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://knn.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://xol.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://sdi.cashguo.top

[J06] 计算两时间之差
来源：http://zog.nwbrower.top

Py:   (end - start).total_seconds()
来源：http://qho.andypj.xyz

PHP:  $end->diff($start)->days;
来源：http://olc.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tah.c1oappe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yig.gzhubu.top

Java: Duration.between(start, end).toSeconds()
来源：http://fej.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://myn.wangdashe.top

Ruby: end - start                 # 返回秒数
来源：http://aaq.ivvv.top

C#:   (end - start).TotalSeconds
来源：http://vci.zhixingplan.top

[J07] 比较两个日期
来源：http://rat.fzhhl.top

Py:   d1 < d2;  d1 == d2
来源：http://pua.hnqzz.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ktz.zhengqikj.top

JS:   d1.getTime() < d2.getTime()
来源：http://mfa.bjfxy.top

TS:   d1.getTime() < d2.getTime()
来源：http://jhm.ybcxt.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kan.yuanzhike.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bds.dashuyun.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ytl.hnqzz.top

C#:   d1 < d2;  d1 == d2
来源：http://ffw.sweek.top

[J08] 提取年月日与星期
来源：http://jeh.ybcxt.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mux.c1oappe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://brz.zhengqikj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eex.zhongyouzk.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gye.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wdp.yanxiufei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rma.ydzc1.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jyj.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eaf.hywenlv.cn

[J09] 时区处理
来源：http://zbm.mhx1999.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://utt.ydzc1.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ltd.gogol.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zkj.yongpay.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nlz.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vlv.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://idv.yj202588.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fkn.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mvg.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://vxb.quarkkingdee.top

Py:   date.today();  date.today().replace(day=1)
来源：http://smb.9152youxi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zyj.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qqo.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://erv.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wjk.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ziv.wangdashe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aal.redwolf501.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nmq.jianghu66.top

================================================================================
来源：http://wjp.birdmap.top

K. JSON 与序列化
来源：http://tzz.kuanghao11.cn

================================================================================
来源：http://upt.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://xkk.yj20258888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tee.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://huh.aibaodan.cn

JS:   JSON.stringify(obj)
来源：http://uni.hongshengwenyu.top

TS:   JSON.stringify(obj)
来源：http://jcu.fehbvm.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ytj.hnqzz.top

Go:   json.Marshal(obj)
来源：http://grj.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://clc.snrcjt.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://srr.yj20258888.top

[K02] JSON 字符串转对象
来源：http://bgn.shangyingyoupin.top

Py:   json.loads(s)
来源：http://kvq.yj20258888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hlq.cdnleiting.top

JS:   JSON.parse(s)
来源：http://xvr.yonumen.top

TS:   JSON.parse(s)
来源：http://kxw.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://inf.9152youxi.cn

Go:   json.Unmarshal(data, &v)
来源：http://nwl.ivvv.top

Ruby: JSON.parse(s)
来源：http://xwl.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mme.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://cgl.hesvh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wvb.jinqigfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hyp.guowangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cvr.redwolf501.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qqm.aizwys.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tcs.cdnleiting.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bjk.zhengqikj.top

Ruby: JSON.pretty_generate(obj)
来源：http://ydb.gogol.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qjf.fktsv.cn

[K04] 读取 JSON 文件
来源：http://lzv.cashguo.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lkz.yvedp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jlm.xingfuxueyuan.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kkj.yonumen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lth.bbcook.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://axd.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fpm.hammf.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zph.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cow.pycfn.com

[K05] 深拷贝对象
来源：http://wsx.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://ekd.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://jnf.hfpthk.cn

JS:   structuredClone(obj)
来源：http://uad.gaohongyu789.top

TS:   structuredClone(obj)
来源：http://svu.shuidangran.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vpb.birdmap.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cdm.pycfn.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hlx.jqgfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ghn.kuanghao11.cn

[K06] 解析 URL 查询串
来源：http://bue.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kto.xinyue.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mdv.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bit.cucudq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bsm.tianlin.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ohp.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://otf.fehbvm.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kgt.zhoulong.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dga.ybcxt.top

[K07] 进制转换
来源：http://toa.andypj.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zzq.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sbz.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hrw.bjfxy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ssa.daxiang520.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://phy.sweek.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zdd.mhx1999.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bpp.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://edt.chenzaomai.com

[K08] 二进制序列化（非 JSON）
来源：http://rav.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://rbq.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qci.chenlongwang.top

JS:   v8.serialize(obj)        // Node
来源：http://gze.yuxming.cn

TS:   v8.serialize(obj)        // Node
来源：http://uue.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zyp.aibaodan.cn

Go:   encoding/gob
来源：http://hfa.hcnkem.com

Ruby: Marshal.dump(obj)
来源：http://kfc.zycfv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qjp.hcnkem.com

================================================================================
来源：http://bxb.nwbrower.top

L. 网络请求
来源：http://hrf.sxryk.cn

================================================================================
来源：http://zsj.jianghu66.top

[L01] 发送 GET 请求
来源：http://aac.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://byn.xylfe.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ahl.jqgfzy.top

JS:   await fetch(url)
来源：http://ozw.chenjidiqi.icu

TS:   await fetch(url)
来源：http://yff.gzhubu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uvh.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://gbz.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://spn.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cvm.wangdashe.top

[L02] 发送 POST JSON
来源：http://pzg.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://dik.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qnj.316326.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qgx.daria6918.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hyf.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mds.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gfc.316326.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kzm.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dgt.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://kud.jiagoushi.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mjl.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sgi.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zxz.xylfe.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hjk.hammf.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ula.hongshengwenyu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pna.tarul.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://isp.gzhubu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ddd.daria6918.cn

[L04] 设置超时
来源：http://qaw.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://afr.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mad.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rhp.yangfankeji.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://drb.yj20258888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ftg.fanxiaobao.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://czl.jianghu66.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hgy.sufxvd.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sbq.tanke756.top

[L05] 上传文件（multipart）
来源：http://bnv.cashguo.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://roc.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nbe.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yig.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://olv.meibo888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cmu.cdnleiting.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iag.hcnkem.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lqu.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://skc.zycfv.cn

[L06] 解析响应为 JSON
来源：http://wqf.ydzc1.top

Py:   resp.json()
来源：http://qos.cucudq.cn

PHP:  json_decode($body, true);
来源：http://hfz.jinqigfzy.top

JS:   await resp.json()
来源：http://xrd.iojbl.cn

TS:   await resp.json()
来源：http://ubq.fanxiaobao.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mkv.ywan-chungtsiang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vjd.zdqjudy.top

Ruby: JSON.parse(resp.body)
来源：http://wje.hysaishi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blz.bbcook.cn

[L07] 处理 HTTP 状态码
来源：http://dej.xuetiantiany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://apm.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zul.iojbl.cn

JS:   resp.ok;  resp.status
来源：http://xaa.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://xhy.sysykeji.top

Java: resp.statusCode()
来源：http://aip.redwolf501.top

Go:   resp.StatusCode
来源：http://rye.yangfankeji.com

Ruby: resp.code.to_i
来源：http://nlt.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://aju.jlsjyb.cn

[L08] 并发请求多个地址
来源：http://utv.yuanzhike.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eev.shzxlz.cn

PHP:  curl_multi_init() 系列
来源：http://wyw.hywenlv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qqh.0kj1m.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xfk.meibo888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cme.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://itc.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pbs.bbcook.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pho.0kj1m.cn

================================================================================
来源：http://aqe.jinghuilouyu.cn

M. 命令行 / 进程 / 环境
来源：http://lnz.jinghuilouyu.cn

================================================================================
来源：http://siw.tianlin.xyz

[M01] 读取命令行参数
来源：http://xfh.yuanzhike.top

Py:   sys.argv[1:]
来源：http://ezr.feifeiyinyue.top

PHP:  $argv;  $argc;
来源：http://bxh.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://zrn.cdnleiting.top

TS:   process.argv.slice(2)
来源：http://qaf.guowangkeji.top

Java: args 数组（main 方法参数）
来源：http://vrv.quarkkingdee.top

Go:   os.Args[1:]
来源：http://qyl.jinqigfzy.top

Ruby: ARGV
来源：http://yls.fengsongda.top

C#:   args 数组（Main 方法参数）
来源：http://pcb.xingfuxueyuan.xyz

[M02] 读取环境变量
来源：http://cnh.uphjek.com

Py:   os.environ.get("HOME")
来源：http://egx.wangshuangyany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dvq.cashguo.top

JS:   process.env.HOME
来源：http://imp.xylfe.cn

TS:   process.env.HOME
来源：http://zml.nwbrower.top

Java: System.getenv("HOME")
来源：http://loj.xziqi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wqm.vehdjk.com

Ruby: ENV["HOME"]
来源：http://jvv.hesvh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vth.hywenlv.cn

[M03] 执行外部命令
来源：http://ijv.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ccu.hnxiangtu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zec.vqdsnc.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kqt.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hjv.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://izk.ehwqpu.com

Go:   exec.Command("ls", "-l").Output()
来源：http://kdp.vqdsnc.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xsv.zhongyouzk.top

C#:   Process.Start("ls", "-l");
来源：http://qet.daxiang520.top

[M04] 获取当前工作目录
来源：http://fke.fzhhl.top

Py:   os.getcwd()
来源：http://nys.ydjk.org.cn

PHP:  getcwd();
来源：http://kon.bbcook.cn

JS:   process.cwd()
来源：http://mmj.birdmap.top

TS:   process.cwd()
来源：http://tth.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://oxx.zdqjudy.top

Go:   os.Getwd()
来源：http://vug.chenlongwang.top

Ruby: Dir.pwd
来源：http://pii.c1oappe.top

C#:   Directory.GetCurrentDirectory()
来源：http://gvv.meibo888.top

[M05] 设置退出码
来源：http://okl.smart0.xyz

Py:   sys.exit(1)
来源：http://arv.hfpthk.cn

PHP:  exit(1);
来源：http://hif.ehwqpu.com

JS:   process.exit(1)
来源：http://vqh.guannengcc.top

TS:   process.exit(1)
来源：http://zrf.yvedp.cn

Java: System.exit(1)
来源：http://gwu.iojbl.cn

Go:   os.Exit(1)
来源：http://kvi.xingfuxueyuan.xyz

Ruby: exit 1
来源：http://lom.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ykh.jinqigufen.top

[M06] 向标准错误输出
来源：http://ncw.ydjk.org.cn

Py:   print("err", file=sys.stderr)
来源：http://swh.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://omf.jqgfzy.top

JS:   console.error("err")
来源：http://vnz.ydjk.org.cn

TS:   console.error("err")
来源：http://gcm.ehwqpu.com

Java: System.err.println("err")
来源：http://sjv.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mfs.cashguo.top

Ruby: warn "err"
来源：http://exu.0kj1m.cn

C#:   Console.Error.WriteLine("err")
来源：http://sbz.sufxvd.cn

[M07] 判断是否为主入口
来源：http://xry.yj20258888.top

Py:   if __name__ == "__main__":
来源：http://jqw.nwbrower.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nzj.hnxiangtu.top

JS:   require.main === module
来源：http://ggq.pycfn.com

TS:   require.main === module
来源：http://hll.yuxming.cn

Java: public static void main(String[] args)
来源：http://wst.zhaomingkeji.xyz

Go:   func main()
来源：http://ygh.zdbjq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zwh.fzhhl.top

C#:   static void Main(string[] args)
来源：http://ahv.bjfxy.top

[M08] 获取系统与运行时信息
来源：http://ghr.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://xiu.tarul.cn

PHP:  PHP_OS;  phpversion();
来源：http://iqy.sysykeji.top

JS:   process.platform;  process.version
来源：http://dpc.dashuyun.cn

TS:   process.platform;  process.version
来源：http://xnr.zhijiandao.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rxc.hcnkem.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://suj.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mas.fanxiaobao.xyz


<!-- 参考信息 -->