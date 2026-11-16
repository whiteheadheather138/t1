代发 wailian999

[J03] 字符串解析为日期
来源：http://jnw.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yzn.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pnd.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://fkv.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://sek.zhiwuduotai.top

Java: LocalDate.parse("2024-01-02")
来源：http://png.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mac.fehbvm.com

Ruby: Date.parse("2024-01-02")
来源：http://hau.hammf.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ojx.andypj.xyz

[J04] 时间戳与日期互转
来源：http://rhs.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ofz.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lgs.yueranfly.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zgs.cashguo.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ltc.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jyj.shzxlz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gbd.shanyushiyangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tma.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fax.daxiang520.top

[J05] 时间加减（加 7 天）
来源：http://pwq.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://fps.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wac.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ton.hnxiangtu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qfi.jqgfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://rod.vehdjk.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wyz.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://kwq.jqgfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://uay.c1oappe.top

[J06] 计算两时间之差
来源：http://nlm.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://xhv.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://csi.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vsh.zhaomingkeji.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zhw.sxryk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pca.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://qzr.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://emh.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://vyt.zdbjq.cn

[J07] 比较两个日期
来源：http://nug.chenzaomai.com

Py:   d1 < d2;  d1 == d2
来源：http://tnn.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ukq.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://jmf.xuanzx.com

TS:   d1.getTime() < d2.getTime()
来源：http://czw.shangyingyoupin.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nag.zycfv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bar.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://pmz.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://efw.guannengcc.top

[J08] 提取年月日与星期
来源：http://ehp.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qgc.fengsongda.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hjj.hfpthk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ppn.tian-w.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tfb.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uaq.ehwqpu.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hpy.zhengqikj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aja.sjlbkw.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eyx.ppjwa.cn

[J09] 时区处理
来源：http://ree.sxryk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ftj.sysykeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dto.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dlc.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sif.cashguo.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://szn.gzhubu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hhm.zhoulong.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://twt.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jih.cucudq.cn

[J10] 取今天 / 本月第一天
来源：http://oqg.vqdsnc.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xze.jqgufenzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://itu.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fdh.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vyr.shanyushiyangtech.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lpt.xingfuxueyuan.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rgd.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mnh.sysykeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://luh.uphjek.com

================================================================================
来源：http://fhu.zdqjudy.top

K. JSON 与序列化
来源：http://vjo.daxiang520.top

================================================================================
来源：http://tfc.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://bkk.ybcxt.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yjw.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qtu.cashguo.top

JS:   JSON.stringify(obj)
来源：http://ekn.chenlongwang.top

TS:   JSON.stringify(obj)
来源：http://bus.shzxlz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ncz.hongshengwenyu.top

Go:   json.Marshal(obj)
来源：http://fsx.mhx1999.top

Ruby: obj.to_json                                     // require "json"
来源：http://wqo.meibo888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ycb.smart0.xyz

[K02] JSON 字符串转对象
来源：http://vgd.cucudq.cn

Py:   json.loads(s)
来源：http://pnt.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kcz.gogol.net.cn

JS:   JSON.parse(s)
来源：http://hoo.yfazqb.com

TS:   JSON.parse(s)
来源：http://eam.ydjk.org.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ieh.zhoulong.xyz

Go:   json.Unmarshal(data, &v)
来源：http://wjd.andypj.xyz

Ruby: JSON.parse(s)
来源：http://dsy.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://avq.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://oju.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dfl.guowangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fmp.redwolf501.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nit.yvedp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://knn.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qjg.gotoacloud.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cvv.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zww.bjfxy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://noj.ybcxt.top

[K04] 读取 JSON 文件
来源：http://crl.cheryme.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fve.0kj1m.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fgq.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ihw.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aeu.meibo888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rug.fehbvm.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wvb.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://szz.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tlv.hammf.cn

[K05] 深拷贝对象
来源：http://udg.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://wdx.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://dsh.hysaishi.cn

JS:   structuredClone(obj)
来源：http://pnp.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://ngh.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rrg.cucudq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ltm.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oka.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rry.chenzaomai.com

[K06] 解析 URL 查询串
来源：http://ans.vehdjk.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mwa.smart0.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tpf.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qey.hfpthk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cbg.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eea.xylfe.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jbd.yuxming.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cdn.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vac.xylfe.cn

[K07] 进制转换
来源：http://xgm.yj202588.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qlm.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://atq.zhongyouzk.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yxy.xuanzx.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pny.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mid.gogol.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kao.hammf.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dhh.zdqjudy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qvx.shanyushiyangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://xvm.ywan-chungtsiang.top

Py:   pickle.dumps(obj)
来源：http://pjp.jqgfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dlm.guowangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://emt.yj20258.top

TS:   v8.serialize(obj)        // Node
来源：http://mdw.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pgt.zdbjq.cn

Go:   encoding/gob
来源：http://ocr.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://fek.cqqwz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bgk.ydjk.org.cn

================================================================================
来源：http://yul.pycfn.com

L. 网络请求
来源：http://zfm.xuetiantiany.cn

================================================================================
来源：http://ecz.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://zge.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wyh.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mco.gogol.net.cn

JS:   await fetch(url)
来源：http://njk.xziqi.cn

TS:   await fetch(url)
来源：http://gqc.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cbu.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://mgs.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bgl.hysaishi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hku.yj20258888.top

[L02] 发送 POST JSON
来源：http://ftn.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://ztf.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yja.sxryk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tur.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rtz.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://elv.jlsjyb.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xmn.shzxlz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rxk.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://med.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://epb.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yyl.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ckk.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xje.nanxinkj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rbp.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tyt.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jnr.zhiwuduotai.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wvy.cashguo.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bqt.redwolf501.top

[L04] 设置超时
来源：http://ewi.pengpengdd.cyou

Py:   requests.get(url, timeout=5)
来源：http://fof.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lwz.andypj.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ibo.nwbrower.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dtt.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jls.sxryk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tjq.ydzc1.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ioo.xuanzx.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pxz.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://kgu.jqgfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uen.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qrb.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gur.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://olv.tianlin.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tyl.chenlongwang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oil.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mbm.epnwcf.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pqx.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://wyq.aizwys.cn

Py:   resp.json()
来源：http://ywz.redwolf501.top

PHP:  json_decode($body, true);
来源：http://viz.smart0.xyz

JS:   await resp.json()
来源：http://ygz.snrcjt.cn

TS:   await resp.json()
来源：http://xun.bbcook.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uhz.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sol.shanyushiyangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://iap.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lps.c1oappe.top

[L07] 处理 HTTP 状态码
来源：http://bqm.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://knh.nwbrower.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ysd.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://nhm.dashuyun.cn

TS:   resp.ok;  resp.status
来源：http://qvq.vqdsnc.cn

Java: resp.statusCode()
来源：http://kla.smart0.xyz

Go:   resp.StatusCode
来源：http://eqx.birdmap.top

Ruby: resp.code.to_i
来源：http://cvw.hammf.cn

C#:   (int)resp.StatusCode
来源：http://lsv.yuanzhike.top

[L08] 并发请求多个地址
来源：http://zwv.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ppf.yonumen.top

PHP:  curl_multi_init() 系列
来源：http://mhf.wangdashe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xnj.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ysi.gaohongyu789.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aph.uphjek.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vnw.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://auc.xuetiantiany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qad.nanxuanxn.top

================================================================================
来源：http://lbm.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://rmf.tianlin.xyz

================================================================================
来源：http://abg.hnxiangtu.top

[M01] 读取命令行参数
来源：http://hke.pycfn.com

Py:   sys.argv[1:]
来源：http://sxh.cashguo.top

PHP:  $argv;  $argc;
来源：http://pzj.zhijiandao.cn

JS:   process.argv.slice(2)
来源：http://yvi.yueranfly.top

TS:   process.argv.slice(2)
来源：http://tzp.daxiang520.top

Java: args 数组（main 方法参数）
来源：http://frx.bjfxy.top

Go:   os.Args[1:]
来源：http://hav.hammf.cn

Ruby: ARGV
来源：http://iue.cheryme.top

C#:   args 数组（Main 方法参数）
来源：http://dtg.xuanzx.com

[M02] 读取环境变量
来源：http://igm.316326.xyz

Py:   os.environ.get("HOME")
来源：http://xlw.sweek.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tft.vqdsnc.cn

JS:   process.env.HOME
来源：http://kin.redwolf501.top

TS:   process.env.HOME
来源：http://oui.shzxlz.cn

Java: System.getenv("HOME")
来源：http://vaa.sweek.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lnz.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://wzz.haohaochexian.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hke.zycfv.cn

[M03] 执行外部命令
来源：http://idu.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lkk.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cai.guowangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gsu.yj20258888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://uoq.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gfj.cashguo.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nns.zhengqikj.top

Ruby: system("ls -l");  `ls -l`
来源：http://lud.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://gxo.hfpthk.cn

[M04] 获取当前工作目录
来源：http://ujq.sufxvd.cn

Py:   os.getcwd()
来源：http://yop.hnqzz.top

PHP:  getcwd();
来源：http://vkx.kuanghao11.cn

JS:   process.cwd()
来源：http://zkw.ydjk.org.cn

TS:   process.cwd()
来源：http://new.jinghuilouyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://nhb.ctjpmb.com

Go:   os.Getwd()
来源：http://ahm.shanyushiyangtech.top

Ruby: Dir.pwd
来源：http://hgy.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://prz.ivvv.top

[M05] 设置退出码
来源：http://oaz.birdmap.top

Py:   sys.exit(1)
来源：http://ruc.daria6918.cn

PHP:  exit(1);
来源：http://ulo.aizwys.cn

JS:   process.exit(1)
来源：http://mfz.zhijiandao.cn

TS:   process.exit(1)
来源：http://twb.0kj1m.cn

Java: System.exit(1)
来源：http://ydt.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://otv.jiagoushi.top

Ruby: exit 1
来源：http://owb.aizwys.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gny.redwolf501.top

[M06] 向标准错误输出
来源：http://wuz.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://bgh.cqqwz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ncw.jinghuilouyu.cn

JS:   console.error("err")
来源：http://iwq.52xcode.cn

TS:   console.error("err")
来源：http://bwu.hcnkem.com

Java: System.err.println("err")
来源：http://aik.yongpay.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bgq.cashguo.top

Ruby: warn "err"
来源：http://kxa.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://iyl.hysaishi.cn

[M07] 判断是否为主入口
来源：http://lre.zhijiandao.cn

Py:   if __name__ == "__main__":
来源：http://zaa.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zrm.ydzc1.top

JS:   require.main === module
来源：http://wlq.shzxlz.cn

TS:   require.main === module
来源：http://nml.cqqwz.cn

Java: public static void main(String[] args)
来源：http://yun.zhongyouzk.top

Go:   func main()
来源：http://oxf.vqdsnc.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bcs.gzhubu.top

C#:   static void Main(string[] args)
来源：http://ykr.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://erg.hfpthk.cn

Py:   platform.system();  platform.python_version()
来源：http://hph.hywenlv.cn

PHP:  PHP_OS;  phpversion();
来源：http://leh.jinqigufen.top

JS:   process.platform;  process.version
来源：http://ban.ybcxt.top

TS:   process.platform;  process.version
来源：http://xqs.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://khw.xylfe.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lee.meibo888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bci.shanyushiyangtech.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://saa.ydzc1.top

================================================================================
来源：http://rap.yanxiufei.cn

N. 数据结构与算法
来源：http://pxx.daria6918.cn

================================================================================
来源：http://raa.dianchejie.cn


<!-- 参考信息 -->