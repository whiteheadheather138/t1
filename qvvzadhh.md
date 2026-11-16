代发 wailian999

[J03] 字符串解析为日期
来源：http://skl.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cas.cdnleiting.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://itg.yj20258888.top

JS:   new Date("2024-01-02")
来源：http://uem.yonumen.top

TS:   new Date("2024-01-02")
来源：http://icl.sysykeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://qpu.daxiang520.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vao.xylfe.cn

Ruby: Date.parse("2024-01-02")
来源：http://nat.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://itd.xylfe.cn

[J04] 时间戳与日期互转
来源：http://hsy.hcnkem.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tug.yuanzhike.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fts.bjfxy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nca.jyoumei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://iat.shuidangran.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vlq.fzhhl.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ukj.gotoacloud.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tqd.snrcjt.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://byf.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://gyp.pycfn.com

Py:   now + timedelta(days=7)
来源：http://wnu.0kj1m.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mwh.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gdm.hesvh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fzu.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://uww.zhoulong.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fri.iojbl.cn

Ruby: Time.now + 7 * 86400
来源：http://cao.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://bxb.gogol.net.cn

[J06] 计算两时间之差
来源：http://dgk.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://chd.zycfv.cn

PHP:  $end->diff($start)->days;
来源：http://znb.gzhubu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qza.fehbvm.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sfz.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://fiq.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://sxs.gaohongyu789.top

Ruby: end - start                 # 返回秒数
来源：http://oww.mhx1999.top

C#:   (end - start).TotalSeconds
来源：http://ktj.xziqi.cn

[J07] 比较两个日期
来源：http://ksi.zdqjudy.top

Py:   d1 < d2;  d1 == d2
来源：http://toj.ywan-chungtsiang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tno.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://xzy.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://gdf.jinqigufen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qxd.shuidangran.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vgl.zhengqikj.top

Ruby: d1 < d2;  d1 == d2
来源：http://omt.fanxiaobao.xyz

C#:   d1 < d2;  d1 == d2
来源：http://pad.birdmap.top

[J08] 提取年月日与星期
来源：http://jit.shanyushiyangtech.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ynf.fengsongda.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dmq.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nlh.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eaq.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://say.yj20258888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jbn.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rvg.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nbp.yangfankeji.com

[J09] 时区处理
来源：http://ykk.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://edg.yfazqb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hdx.jinqigfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hic.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rim.sweek.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tif.shuidangran.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ebl.jyoumei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fow.uphjek.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blq.hcnkem.com

[J10] 取今天 / 本月第一天
来源：http://nwz.c1oappe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bpi.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lno.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rci.jyoumei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vxk.hnxiangtu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ife.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jxz.9152youxi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://naz.52xcode.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xlt.zhongyouzk.top

================================================================================
来源：http://wfa.ctjpmb.com

K. JSON 与序列化
来源：http://sdu.tarul.cn

================================================================================
来源：http://hoz.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://glb.hywenlv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tft.epnwcf.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nkz.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://tap.xuetiantiany.cn

TS:   JSON.stringify(obj)
来源：http://egk.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xwv.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://dow.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://mgl.xuanzx.com

C#:   JsonSerializer.Serialize(obj)
来源：http://stm.fanxiaobao.xyz

[K02] JSON 字符串转对象
来源：http://awm.jlsjyb.cn

Py:   json.loads(s)
来源：http://fkm.xuanzx.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xuh.xziqi.cn

JS:   JSON.parse(s)
来源：http://itd.yvedp.cn

TS:   JSON.parse(s)
来源：http://snx.epnwcf.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qre.daria6918.cn

Go:   json.Unmarshal(data, &v)
来源：http://gbv.cheryme.top

Ruby: JSON.parse(s)
来源：http://xsw.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nnt.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://amo.aizwys.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://orj.ppjwa.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yqe.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mdq.ivvv.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xbq.yvedp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iec.zdqjudy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oox.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bwd.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ajy.zhoulong.xyz

[K04] 读取 JSON 文件
来源：http://bhc.xuetiantiany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vgn.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tdr.nanxinkj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yuf.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qdl.vehdjk.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lyc.cucudq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wtw.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dpq.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ddw.xylfe.cn

[K05] 深拷贝对象
来源：http://cqv.hongshengwenyu.top

Py:   copy.deepcopy(obj)
来源：http://jyx.pycfn.com

PHP:  unserialize(serialize($obj));
来源：http://hfs.gogol.net.cn

JS:   structuredClone(obj)
来源：http://wnf.guowangkeji.top

TS:   structuredClone(obj)
来源：http://vcq.zhengqikj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tgl.redwolf501.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qet.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zay.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kxr.andypj.xyz

[K06] 解析 URL 查询串
来源：http://kcp.shzxlz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kkf.andypj.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tor.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uzk.yuanzhike.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lsc.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zkf.hfpthk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oee.guannengcc.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nyi.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kum.nanxuanxn.top

[K07] 进制转换
来源：http://ixu.epnwcf.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ncr.c1oappe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ond.hcnkem.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nju.gotoacloud.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tba.uphjek.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://glq.daria6918.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jom.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gxc.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://obn.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://ewo.fanxiaobao.xyz

Py:   pickle.dumps(obj)
来源：http://hus.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://afc.daxiang520.top

JS:   v8.serialize(obj)        // Node
来源：http://psf.fktsv.cn

TS:   v8.serialize(obj)        // Node
来源：http://otw.dashuyun.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dhg.yuxming.cn

Go:   encoding/gob
来源：http://vyh.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://zxs.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ltd.yfazqb.com

================================================================================
来源：http://jiu.gzhubu.top

L. 网络请求
来源：http://hmf.sweek.top

================================================================================
来源：http://fjf.ppjwa.cn

[L01] 发送 GET 请求
来源：http://gdn.yueranfly.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pey.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bam.sjlbkw.cn

JS:   await fetch(url)
来源：http://hvh.tianlin.xyz

TS:   await fetch(url)
来源：http://exq.tian-w.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aok.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://dht.yvedp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://edh.hfpthk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ivm.jianghu66.top

[L02] 发送 POST JSON
来源：http://qbb.jinqigufen.top

Py:   requests.post(url, json={"a": 1})
来源：http://tch.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pmn.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ejh.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mcf.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zhk.aibaodan.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wkj.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://juj.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nob.shzxlz.cn

[L03] 设置自定义请求头
来源：http://nfo.zhixingplan.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://idf.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gwh.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lmz.vqdsnc.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ayj.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dxc.yvedp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://csx.xingfuxueyuan.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vce.zycfv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ezh.9152youxi.cn

[L04] 设置超时
来源：http://jss.tian-w.cn

Py:   requests.get(url, timeout=5)
来源：http://xoa.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://isw.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ifu.hcnkem.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jbq.jinqigufen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xju.jiagoushi.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hhe.svipenyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://omo.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://neo.jqgufenzy.top

[L05] 上传文件（multipart）
来源：http://dut.fengsongda.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tvf.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pcu.yangfankeji.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iry.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ukx.chenlongwang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vfg.c1oappe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xbo.chenlongwang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ndv.gogol.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aja.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://ejf.hfpthk.cn

Py:   resp.json()
来源：http://ffh.gotoacloud.top

PHP:  json_decode($body, true);
来源：http://izn.sysykeji.top

JS:   await resp.json()
来源：http://dvh.zhoulong.xyz

TS:   await resp.json()
来源：http://zzw.shangyingyoupin.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eas.hywenlv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bne.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://oet.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zzn.snrcjt.cn

[L07] 处理 HTTP 状态码
来源：http://lux.yuxming.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tlo.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://afg.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://vdi.yuxming.cn

TS:   resp.ok;  resp.status
来源：http://nbf.hywenlv.cn

Java: resp.statusCode()
来源：http://fch.chenlongwang.top

Go:   resp.StatusCode
来源：http://cid.yj20258888.top

Ruby: resp.code.to_i
来源：http://oyk.fehbvm.com

C#:   (int)resp.StatusCode
来源：http://vmv.zdqjudy.top

[L08] 并发请求多个地址
来源：http://keo.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eye.shzxlz.cn

PHP:  curl_multi_init() 系列
来源：http://bou.hywenlv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fch.fengsongda.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zhy.vqdsnc.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lor.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://etu.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uvh.bjfxy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vws.9152youxi.cn

================================================================================
来源：http://tea.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://uxo.fktsv.cn

================================================================================
来源：http://cgm.fktsv.cn

[M01] 读取命令行参数
来源：http://dsk.shzxlz.cn

Py:   sys.argv[1:]
来源：http://qzy.zhongyouzk.top

PHP:  $argv;  $argc;
来源：http://hks.svipenyu.cn

JS:   process.argv.slice(2)
来源：http://qmr.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://xke.yonumen.top

Java: args 数组（main 方法参数）
来源：http://zxh.cashguo.top

Go:   os.Args[1:]
来源：http://sjv.uphjek.com

Ruby: ARGV
来源：http://zmc.ivvv.top

C#:   args 数组（Main 方法参数）
来源：http://fil.aizwys.cn

[M02] 读取环境变量
来源：http://tpa.nanxuanxn.top

Py:   os.environ.get("HOME")
来源：http://teu.cqqwz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rpx.nanxuanxn.top

JS:   process.env.HOME
来源：http://erj.ydjk.org.cn

TS:   process.env.HOME
来源：http://cay.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://lad.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://drs.nwbrower.top

Ruby: ENV["HOME"]
来源：http://xva.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hyo.hnxiangtu.top

[M03] 执行外部命令
来源：http://ihe.guannengcc.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jax.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jlz.yvedp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jds.hfpthk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://obm.hammf.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pmz.ehwqpu.com

Go:   exec.Command("ls", "-l").Output()
来源：http://tjj.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hdv.yueranfly.top

C#:   Process.Start("ls", "-l");
来源：http://mid.yj20258.top

[M04] 获取当前工作目录
来源：http://zjs.dianchejie.cn

Py:   os.getcwd()
来源：http://cla.vehdjk.com

PHP:  getcwd();
来源：http://abk.epnwcf.com

JS:   process.cwd()
来源：http://rqt.feifeiyinyue.top

TS:   process.cwd()
来源：http://ehq.yanxiufei.cn

Java: Path.of("").toAbsolutePath()
来源：http://emx.vehdjk.com

Go:   os.Getwd()
来源：http://zix.vqdsnc.cn

Ruby: Dir.pwd
来源：http://itp.zdqjudy.top

C#:   Directory.GetCurrentDirectory()
来源：http://aww.ehwqpu.com

[M05] 设置退出码
来源：http://agx.tianlin.xyz

Py:   sys.exit(1)
来源：http://nyc.aizwys.cn

PHP:  exit(1);
来源：http://qgz.chenlongwang.top

JS:   process.exit(1)
来源：http://rqx.chenlongwang.top

TS:   process.exit(1)
来源：http://lwk.daria6918.cn

Java: System.exit(1)
来源：http://pkv.bjfxy.top

Go:   os.Exit(1)
来源：http://daz.tanke756.top

Ruby: exit 1
来源：http://wrv.zhixingplan.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://geo.haohaochexian.top

[M06] 向标准错误输出
来源：http://sce.hysaishi.cn

Py:   print("err", file=sys.stderr)
来源：http://hwh.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rpy.hysaishi.cn

JS:   console.error("err")
来源：http://nya.316326.xyz

TS:   console.error("err")
来源：http://sry.cashguo.top

Java: System.err.println("err")
来源：http://odo.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://adh.daria6918.cn

Ruby: warn "err"
来源：http://ves.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://igv.tian-w.cn

[M07] 判断是否为主入口
来源：http://ahv.pycfn.com

Py:   if __name__ == "__main__":
来源：http://ubk.zhongyouzk.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://orc.wangshuangyany.cn

JS:   require.main === module
来源：http://gke.shanyushiyangkeji.top

TS:   require.main === module
来源：http://kpq.shanyushiyangtech.top

Java: public static void main(String[] args)
来源：http://ktz.9152youxi.cn

Go:   func main()
来源：http://ecf.meibo888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tbv.yj20258.top

C#:   static void Main(string[] args)
来源：http://jgw.xuetiantiany.cn

[M08] 获取系统与运行时信息
来源：http://iqa.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://ttn.zhijiandao.cn

PHP:  PHP_OS;  phpversion();
来源：http://sky.yj202588.top

JS:   process.platform;  process.version
来源：http://iya.gaohongyu789.top

TS:   process.platform;  process.version
来源：http://niy.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vfg.sxryk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gfg.xuanzx.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://doy.iojbl.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://brs.wangdashe.top

================================================================================
来源：http://lgy.zhoulong.xyz

N. 数据结构与算法
来源：http://siu.iojbl.cn

================================================================================
来源：http://nrv.bjfxy.top


<!-- 参考信息 -->