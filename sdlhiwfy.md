代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://weh.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cms.pycfn.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zfd.gogol.net.cn

TS:   d.toISOString()
来源：http://wxj.jinghuilouyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kgw.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xdv.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kgj.ybcxt.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qrx.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://yho.yuxming.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jky.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xno.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://equ.yvedp.cn

TS:   new Date("2024-01-02")
来源：http://yer.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://vfr.zdbjq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://idg.iojbl.cn

Ruby: Date.parse("2024-01-02")
来源：http://nyi.yfazqb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zwl.yanxiufei.cn

[J04] 时间戳与日期互转
来源：http://zgf.yueranfly.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://who.wangdashe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yxu.yanxiufei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xlu.yj20258888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ote.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nmk.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cug.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://urp.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://azg.52xcode.cn

[J05] 时间加减（加 7 天）
来源：http://xgn.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://bjk.ppjwa.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tyj.nanxinkj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://czy.ydjk.org.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dlx.snrcjt.cn

Java: LocalDate.now().plusDays(7)
来源：http://jrb.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wvd.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://obm.zycfv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bos.cqqwz.cn

[J06] 计算两时间之差
来源：http://kon.fehbvm.com

Py:   (end - start).total_seconds()
来源：http://qjf.hcnkem.com

PHP:  $end->diff($start)->days;
来源：http://qhq.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nvq.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ntj.c1oappe.top

Java: Duration.between(start, end).toSeconds()
来源：http://pxw.hnxiangtu.top

Go:   end.Sub(start).Hours()
来源：http://otq.xinyue.icu

Ruby: end - start                 # 返回秒数
来源：http://nre.zhijiandao.cn

C#:   (end - start).TotalSeconds
来源：http://jns.ctjpmb.com

[J07] 比较两个日期
来源：http://bok.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://dze.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wis.zhaomingkeji.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://spt.redwolf501.top

TS:   d1.getTime() < d2.getTime()
来源：http://lri.jinghuilouyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zfq.xuanzx.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tjx.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://lgw.iojbl.cn

C#:   d1 < d2;  d1 == d2
来源：http://upc.hnxiangtu.top

[J08] 提取年月日与星期
来源：http://vfk.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xry.ydzc1.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qgc.zhijiandao.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tpi.daxiang520.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://css.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hoi.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pbe.fktsv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xkp.birdmap.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gux.ppjwa.cn

[J09] 时区处理
来源：http://mnq.jyoumei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ddt.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sbj.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://smp.vqdsnc.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rrs.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rxn.bbcook.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://odz.c1oappe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tuy.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uyl.gotoacloud.top

[J10] 取今天 / 本月第一天
来源：http://rzx.vehdjk.com

Py:   date.today();  date.today().replace(day=1)
来源：http://rdq.hcnkem.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aeq.fktsv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jeu.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sqt.ctjpmb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xgg.xziqi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://idv.fktsv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://apn.birdmap.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xzd.zycfv.cn

================================================================================
来源：http://air.snrcjt.cn

K. JSON 与序列化
来源：http://ntd.shangyingyoupin.top

================================================================================
来源：http://yaj.gogol.net.cn

[K01] 对象转 JSON 字符串
来源：http://pec.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eln.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ben.shanyushiyangkeji.top

JS:   JSON.stringify(obj)
来源：http://pkb.yvedp.cn

TS:   JSON.stringify(obj)
来源：http://asc.cqqwz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aux.bjfxy.top

Go:   json.Marshal(obj)
来源：http://hpp.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uee.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://amd.yj20258.top

[K02] JSON 字符串转对象
来源：http://sjg.shanyushiyangkeji.top

Py:   json.loads(s)
来源：http://ilt.0kj1m.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sxi.tianlin.xyz

JS:   JSON.parse(s)
来源：http://qzc.xuetiantiany.cn

TS:   JSON.parse(s)
来源：http://jap.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://drm.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://zkb.yongpay.top

Ruby: JSON.parse(s)
来源：http://cxa.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qkh.shanyushiyangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://pwj.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qiw.guannengcc.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ovc.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zro.xinyue.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://jpw.birdmap.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://axn.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ack.jiagoushi.top

Ruby: JSON.pretty_generate(obj)
来源：http://vlw.pycfn.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sif.hesvh.cn

[K04] 读取 JSON 文件
来源：http://lhn.aibaodan.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ozu.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pbf.meibo888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oit.xingfuxueyuan.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bak.shanyushiyangtech.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://esc.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tpw.tarul.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qvu.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yaq.9152youxi.cn

[K05] 深拷贝对象
来源：http://dno.yvedp.cn

Py:   copy.deepcopy(obj)
来源：http://zfy.yvedp.cn

PHP:  unserialize(serialize($obj));
来源：http://ull.zhijiandao.cn

JS:   structuredClone(obj)
来源：http://kqk.zdbjq.cn

TS:   structuredClone(obj)
来源：http://ppd.tanke756.top

Java: // 手写拷贝构造，或序列化往返
来源：http://syx.gotoacloud.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ohr.shanyushiyangtech.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pru.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://epe.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://bpo.jinyuanbaomall.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rvj.jianghu66.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lbh.xuetiantiany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lhs.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bao.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://csq.birdmap.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mni.ydzc1.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://prf.jiagoushi.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ylj.redwolf501.top

[K07] 进制转换
来源：http://otn.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yht.zycfv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qdn.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fgu.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ymy.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hat.tarul.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nmm.zdqjudy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dly.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cip.hcnkem.com

[K08] 二进制序列化（非 JSON）
来源：http://onb.fehbvm.com

Py:   pickle.dumps(obj)
来源：http://pxa.yonumen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://erk.cucudq.cn

JS:   v8.serialize(obj)        // Node
来源：http://kla.chenzaomai.com

TS:   v8.serialize(obj)        // Node
来源：http://lzy.shanyushiyangtech.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hze.hongshengwenyu.top

Go:   encoding/gob
来源：http://stm.gotoacloud.top

Ruby: Marshal.dump(obj)
来源：http://vqh.zhaomingkeji.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yhi.zhixingplan.top

================================================================================
来源：http://wiy.dianchejie.cn

L. 网络请求
来源：http://yxq.birdmap.top

================================================================================
来源：http://dcf.ivvv.top

[L01] 发送 GET 请求
来源：http://ujy.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eke.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://afh.shuidangran.top

JS:   await fetch(url)
来源：http://sub.cucudq.cn

TS:   await fetch(url)
来源：http://vwj.jqgfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ofm.c1oappe.top

Go:   resp, err := http.Get(url)
来源：http://bgs.yangfankeji.com

Ruby: Net::HTTP.get(URI(url))
来源：http://apy.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vap.guowangkeji.top

[L02] 发送 POST JSON
来源：http://nri.guowangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://cjt.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zey.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vuk.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://org.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ubs.jinghuilouyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kbs.daxiang520.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://msk.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vrp.cashguo.top

[L03] 设置自定义请求头
来源：http://anv.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nbm.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ubc.gzhubu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yqu.snrcjt.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mex.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fpj.zhixingplan.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wtg.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qog.zhoulong.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vqm.jinqigufen.top

[L04] 设置超时
来源：http://xyz.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://avz.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zre.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uug.jinqigfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://djd.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nbb.jlsjyb.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gxa.yfazqb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://imq.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mxn.ydjk.org.cn

[L05] 上传文件（multipart）
来源：http://rio.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cjh.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://psc.daria6918.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ady.redwolf501.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mwv.hfpthk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eif.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aer.chenzaomai.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tdn.daria6918.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dzn.guowangkeji.top

[L06] 解析响应为 JSON
来源：http://vgf.yfazqb.com

Py:   resp.json()
来源：http://ekq.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://lwd.yuanzhike.top

JS:   await resp.json()
来源：http://ndh.cucudq.cn

TS:   await resp.json()
来源：http://ebn.bjfxy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cpl.xuanzx.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ilh.sxryk.cn

Ruby: JSON.parse(resp.body)
来源：http://ope.aizwys.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ikn.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://mjd.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cuj.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kvg.bbcook.cn

JS:   resp.ok;  resp.status
来源：http://dia.zycfv.cn

TS:   resp.ok;  resp.status
来源：http://nff.yj20258.top

Java: resp.statusCode()
来源：http://wfx.sysykeji.top

Go:   resp.StatusCode
来源：http://vkh.gotoacloud.top

Ruby: resp.code.to_i
来源：http://gxt.52xcode.cn

C#:   (int)resp.StatusCode
来源：http://zdi.dianchejie.cn

[L08] 并发请求多个地址
来源：http://ott.shanyushiyangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://srl.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://csv.yonumen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mhd.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xpz.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hef.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hry.zhongyouzk.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jhm.jinqigfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kxv.jqgufenzy.top

================================================================================
来源：http://dzb.tian-w.cn

M. 命令行 / 进程 / 环境
来源：http://hal.pengpengdd.cyou

================================================================================
来源：http://kel.zhixingplan.top

[M01] 读取命令行参数
来源：http://ifh.andypj.xyz

Py:   sys.argv[1:]
来源：http://jkw.fktsv.cn

PHP:  $argv;  $argc;
来源：http://esk.zdqjudy.top

JS:   process.argv.slice(2)
来源：http://qaz.jiagoushi.top

TS:   process.argv.slice(2)
来源：http://dkf.tanke756.top

Java: args 数组（main 方法参数）
来源：http://pbv.vqdsnc.cn

Go:   os.Args[1:]
来源：http://pry.jinghuilouyu.cn

Ruby: ARGV
来源：http://rso.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://aex.hfpthk.cn

[M02] 读取环境变量
来源：http://mju.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://zty.zdqjudy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tmw.316326.xyz

JS:   process.env.HOME
来源：http://imz.ppjwa.cn

TS:   process.env.HOME
来源：http://bhz.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://fyb.fzhhl.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ykm.ppjwa.cn

Ruby: ENV["HOME"]
来源：http://dkj.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ubq.snrcjt.cn

[M03] 执行外部命令
来源：http://jzh.zhixingplan.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bgg.bbcook.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aln.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://scv.xylfe.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ghr.ctjpmb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pur.zhoulong.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://jgl.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ccn.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://ekw.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://dsq.sweek.top

Py:   os.getcwd()
来源：http://qzp.shanyushiyangtech.top

PHP:  getcwd();
来源：http://mvr.ppjwa.cn

JS:   process.cwd()
来源：http://hzs.zhongyouzk.top

TS:   process.cwd()
来源：http://kql.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://lsn.daria6918.cn

Go:   os.Getwd()
来源：http://yxb.fzhhl.top

Ruby: Dir.pwd
来源：http://rjh.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://hgi.zhijiandao.cn

[M05] 设置退出码
来源：http://qch.tian-w.cn

Py:   sys.exit(1)
来源：http://sny.sjlbkw.cn

PHP:  exit(1);
来源：http://eqn.fzhhl.top

JS:   process.exit(1)
来源：http://ljm.yongpay.top

TS:   process.exit(1)
来源：http://vle.jqgfzy.top

Java: System.exit(1)
来源：http://pnp.quarkkingdee.top

Go:   os.Exit(1)
来源：http://sbm.shanyushiyangtech.top

Ruby: exit 1
来源：http://jdr.hongshengwenyu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fsc.zdbjq.cn

[M06] 向标准错误输出
来源：http://zeh.fanxiaobao.xyz

Py:   print("err", file=sys.stderr)
来源：http://vad.xylfe.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dck.iojbl.cn

JS:   console.error("err")
来源：http://uut.redwolf501.top

TS:   console.error("err")
来源：http://upk.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://bgv.chenzaomai.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mtv.gaohongyu789.top

Ruby: warn "err"
来源：http://ids.yuxming.cn

C#:   Console.Error.WriteLine("err")
来源：http://mps.dashuyun.cn

[M07] 判断是否为主入口
来源：http://tcs.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://ddt.yj202588.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wfa.shanyushiyangkeji.top

JS:   require.main === module
来源：http://tss.zhoulong.xyz

TS:   require.main === module
来源：http://hyu.cdnleiting.top

Java: public static void main(String[] args)
来源：http://lai.jinghuilouyu.cn

Go:   func main()
来源：http://qnp.hnqzz.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qgj.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://avg.cucudq.cn

[M08] 获取系统与运行时信息
来源：http://lkv.epnwcf.com

Py:   platform.system();  platform.python_version()
来源：http://ffa.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://xey.pycfn.com

JS:   process.platform;  process.version
来源：http://ujl.fanxiaobao.xyz


<!-- 参考信息 -->