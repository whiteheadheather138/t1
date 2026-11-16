代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kzb.cheryme.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jjb.ywan-chungtsiang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iji.bbcook.cn

TS:   d.toISOString()
来源：http://sgp.hongshengwenyu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://epv.yangfankeji.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pqx.chenlongwang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ort.316326.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ioc.birdmap.top

[J03] 字符串解析为日期
来源：http://msj.316326.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://guw.gzhubu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ppd.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://dpn.chenzaomai.com

TS:   new Date("2024-01-02")
来源：http://zxg.zhengqikj.top

Java: LocalDate.parse("2024-01-02")
来源：http://njm.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://edq.jlsjyb.cn

Ruby: Date.parse("2024-01-02")
来源：http://hnr.yj202588.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hnx.jlsjyb.cn

[J04] 时间戳与日期互转
来源：http://xlh.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sus.yueranfly.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bvz.xuanzx.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sca.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://eya.pycfn.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lyg.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fvr.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pwf.ctjpmb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lyp.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://eyq.tarul.cn

Py:   now + timedelta(days=7)
来源：http://kwb.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://flr.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xnb.zhaomingkeji.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gsl.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://fxu.xuanzx.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mae.cqqwz.cn

Ruby: Time.now + 7 * 86400
来源：http://ops.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mya.bbcook.cn

[J06] 计算两时间之差
来源：http://skw.sweek.top

Py:   (end - start).total_seconds()
来源：http://dne.redwolf501.top

PHP:  $end->diff($start)->days;
来源：http://tfl.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vuu.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qzf.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qzz.zdqjudy.top

Go:   end.Sub(start).Hours()
来源：http://vbb.xingfuxueyuan.xyz

Ruby: end - start                 # 返回秒数
来源：http://ohi.andypj.xyz

C#:   (end - start).TotalSeconds
来源：http://hyn.bbcook.cn

[J07] 比较两个日期
来源：http://xug.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ogl.sxryk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fiz.wangdashe.top

JS:   d1.getTime() < d2.getTime()
来源：http://dje.yonumen.top

TS:   d1.getTime() < d2.getTime()
来源：http://qpw.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://waq.yj20258888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aur.yj20258888.top

Ruby: d1 < d2;  d1 == d2
来源：http://tgf.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://cyq.feifeiyinyue.top

[J08] 提取年月日与星期
来源：http://juk.gaohongyu789.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://urf.smart0.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://czz.hywenlv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kkb.pengpengdd.cyou

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aka.shanyushiyangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gvm.gaohongyu789.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fkz.xinyue.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://npp.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jmf.chenlongwang.top

[J09] 时区处理
来源：http://dxr.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mqx.cucudq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://skv.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jnx.jyoumei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://awz.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eov.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hao.fzhhl.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ops.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vdc.cqqwz.cn

[J10] 取今天 / 本月第一天
来源：http://eay.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://atq.shuidangran.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://buh.xuetiantiany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hij.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jjl.smart0.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mau.fanxiaobao.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cqq.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uyb.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ypi.xingfuxueyuan.xyz

================================================================================
来源：http://pjg.jianghu66.top

K. JSON 与序列化
来源：http://xok.svipenyu.cn

================================================================================
来源：http://dpa.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://rve.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wnl.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kxb.zdqjudy.top

JS:   JSON.stringify(obj)
来源：http://hsq.smart0.xyz

TS:   JSON.stringify(obj)
来源：http://chu.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://guc.yj202588.top

Go:   json.Marshal(obj)
来源：http://tvm.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://uca.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ahc.tarul.cn

[K02] JSON 字符串转对象
来源：http://mnj.hnxiangtu.top

Py:   json.loads(s)
来源：http://lww.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hpt.zycfv.cn

JS:   JSON.parse(s)
来源：http://whb.hfpthk.cn

TS:   JSON.parse(s)
来源：http://ugs.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://plj.dianchejie.cn

Go:   json.Unmarshal(data, &v)
来源：http://vlp.316326.xyz

Ruby: JSON.parse(s)
来源：http://xph.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hiu.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://aak.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fkw.yonumen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fnz.bbcook.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fir.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://geg.cdnleiting.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qqx.fengsongda.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hbu.jinqigfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://vqu.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://szw.wangshuangyany.cn

[K04] 读取 JSON 文件
来源：http://jux.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://biz.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://won.jyoumei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://itd.nanxuanxn.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ynq.yuanzhike.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bpj.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oeo.316326.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://bwx.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jtr.0kj1m.cn

[K05] 深拷贝对象
来源：http://qex.sjlbkw.cn

Py:   copy.deepcopy(obj)
来源：http://djw.sysykeji.top

PHP:  unserialize(serialize($obj));
来源：http://zkd.guowangkeji.top

JS:   structuredClone(obj)
来源：http://zxt.mhx1999.top

TS:   structuredClone(obj)
来源：http://evq.hcnkem.com

Java: // 手写拷贝构造，或序列化往返
来源：http://tzp.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tev.cheryme.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yvy.jyoumei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://luv.jinqigfzy.top

[K06] 解析 URL 查询串
来源：http://yuw.zhixingplan.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ghf.dianchejie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hcz.vqdsnc.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ddp.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kjj.nwbrower.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://moj.jqgufenzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oao.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iws.snrcjt.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cfn.gogol.net.cn

[K07] 进制转换
来源：http://sck.tarul.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tvl.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zmn.zhiwuduotai.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ssl.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://njt.jqgufenzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bvz.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xjm.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kqr.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zbs.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://sii.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://zmm.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jyb.shanyushiyangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://rvu.jinyuanbaomall.cn

TS:   v8.serialize(obj)        // Node
来源：http://blk.epnwcf.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pbm.shangyingyoupin.top

Go:   encoding/gob
来源：http://bfg.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://ang.xylfe.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bef.jinghuilouyu.cn

================================================================================
来源：http://aoa.sjlbkw.cn

L. 网络请求
来源：http://lqk.birdmap.top

================================================================================
来源：http://wpk.yuanzhike.top

[L01] 发送 GET 请求
来源：http://cvf.havefunace.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dvo.zdqjudy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zkb.hcnkem.com

JS:   await fetch(url)
来源：http://qey.yueranfly.top

TS:   await fetch(url)
来源：http://vhr.zycfv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iil.aizwys.cn

Go:   resp, err := http.Get(url)
来源：http://kzi.chenjidiqi.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://dxn.meibo888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hem.bjfxy.top

[L02] 发送 POST JSON
来源：http://fst.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ebw.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rra.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cch.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://phr.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iup.daxiang520.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aup.9152youxi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jhs.yongpay.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://knz.nanxinkj.top

[L03] 设置自定义请求头
来源：http://ryx.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ssn.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ksm.xziqi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://emz.fengsongda.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ndl.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tqr.sjlbkw.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://def.yvedp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rjh.cqqwz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nei.fzhhl.top

[L04] 设置超时
来源：http://qcx.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://glj.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://idj.ybcxt.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wxf.vqdsnc.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ywo.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wul.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gpl.cdnleiting.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ynh.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mxc.epnwcf.com

[L05] 上传文件（multipart）
来源：http://fhe.iojbl.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wlg.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eae.hywenlv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sbj.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gvw.jiagoushi.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ytq.iojbl.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rxi.xuanzx.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qhs.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://get.bbcook.cn

[L06] 解析响应为 JSON
来源：http://cuv.cheryme.top

Py:   resp.json()
来源：http://joo.xuanzx.com

PHP:  json_decode($body, true);
来源：http://scc.nwbrower.top

JS:   await resp.json()
来源：http://mgu.tianlin.xyz

TS:   await resp.json()
来源：http://qaz.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oks.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wcb.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://jdc.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tqw.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://crx.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uec.hywenlv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sgu.316326.xyz

JS:   resp.ok;  resp.status
来源：http://ezx.gaohongyu789.top

TS:   resp.ok;  resp.status
来源：http://lgo.sweek.top

Java: resp.statusCode()
来源：http://erb.yongpay.top

Go:   resp.StatusCode
来源：http://xfe.shzxlz.cn

Ruby: resp.code.to_i
来源：http://epk.guowangkeji.top

C#:   (int)resp.StatusCode
来源：http://zph.52xcode.cn

[L08] 并发请求多个地址
来源：http://zto.jinyuanbaomall.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eqv.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://vqi.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vds.jqgfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lkd.tianlin.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hzx.jianghu66.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iub.tian-w.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lxt.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xwe.xziqi.cn

================================================================================
来源：http://sse.jqgfzy.top

M. 命令行 / 进程 / 环境
来源：http://owj.hfpthk.cn

================================================================================
来源：http://ydz.epnwcf.com

[M01] 读取命令行参数
来源：http://ile.jiagoushi.top

Py:   sys.argv[1:]
来源：http://nhr.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://mmo.pycfn.com

JS:   process.argv.slice(2)
来源：http://xpa.jinghuilouyu.cn

TS:   process.argv.slice(2)
来源：http://cxf.yfazqb.com

Java: args 数组（main 方法参数）
来源：http://kyu.gotoacloud.top

Go:   os.Args[1:]
来源：http://kbx.52xcode.cn

Ruby: ARGV
来源：http://nhc.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://kym.yj202588.top

[M02] 读取环境变量
来源：http://die.gogol.net.cn

Py:   os.environ.get("HOME")
来源：http://fvq.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aab.cheryme.top

JS:   process.env.HOME
来源：http://ied.hammf.cn

TS:   process.env.HOME
来源：http://wha.mhx1999.top

Java: System.getenv("HOME")
来源：http://tmg.zhengqikj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ghk.shangyingyoupin.top

Ruby: ENV["HOME"]
来源：http://otj.shanyushiyangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oam.vqdsnc.cn

[M03] 执行外部命令
来源：http://ivx.zhaomingkeji.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xfb.yanxiufei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wwu.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://aqd.yj20258888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gxi.shzxlz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://otm.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zbo.yj202588.top

Ruby: system("ls -l");  `ls -l`
来源：http://vzu.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://zio.hnqzz.top

[M04] 获取当前工作目录
来源：http://zmz.bjfxy.top

Py:   os.getcwd()
来源：http://dft.gaohongyu789.top

PHP:  getcwd();
来源：http://awe.iojbl.cn

JS:   process.cwd()
来源：http://kmm.tanke756.top

TS:   process.cwd()
来源：http://ahr.ydjk.org.cn

Java: Path.of("").toAbsolutePath()
来源：http://wcz.aibaodan.cn

Go:   os.Getwd()
来源：http://dzy.ehwqpu.com

Ruby: Dir.pwd
来源：http://oqi.yongpay.top

C#:   Directory.GetCurrentDirectory()
来源：http://pkh.smart0.xyz

[M05] 设置退出码
来源：http://zdf.guannengcc.top

Py:   sys.exit(1)
来源：http://fmh.cashguo.top

PHP:  exit(1);
来源：http://mtw.9152youxi.cn

JS:   process.exit(1)
来源：http://ftj.9152youxi.cn

TS:   process.exit(1)
来源：http://ntk.pengpengdd.cyou

Java: System.exit(1)
来源：http://krr.havefunace.top

Go:   os.Exit(1)
来源：http://enk.bbcook.cn

Ruby: exit 1
来源：http://vlv.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xtj.smart0.xyz

[M06] 向标准错误输出
来源：http://yka.hysaishi.cn

Py:   print("err", file=sys.stderr)
来源：http://dqy.gogol.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://men.jyoumei.cn

JS:   console.error("err")
来源：http://mfd.vehdjk.com

TS:   console.error("err")
来源：http://qcm.hcnkem.com

Java: System.err.println("err")
来源：http://vmz.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rlt.tian-w.cn

Ruby: warn "err"
来源：http://swt.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://jdb.haohaochexian.top

[M07] 判断是否为主入口
来源：http://beq.pycfn.com

Py:   if __name__ == "__main__":
来源：http://nqq.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://url.guowangkeji.top

JS:   require.main === module
来源：http://ltk.kuanghao11.cn

TS:   require.main === module
来源：http://fha.yueranfly.top

Java: public static void main(String[] args)
来源：http://drw.haohaochexian.top

Go:   func main()
来源：http://lej.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cfl.sxryk.cn

C#:   static void Main(string[] args)
来源：http://nfl.chenzaomai.com

[M08] 获取系统与运行时信息
来源：http://gxb.nwbrower.top

Py:   platform.system();  platform.python_version()
来源：http://mdk.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://kwy.tanke756.top

JS:   process.platform;  process.version
来源：http://wzb.shanyushiyangkeji.top


<!-- 参考信息 -->