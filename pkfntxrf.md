代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://edx.guowangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://epw.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qpu.cdnleiting.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cda.wangshuangyany.cn

[J03] 字符串解析为日期
来源：http://vna.feifeiyinyue.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hbb.jinghuilouyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qsd.zhijiandao.cn

JS:   new Date("2024-01-02")
来源：http://ass.guowangkeji.top

TS:   new Date("2024-01-02")
来源：http://vcq.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://svx.sjlbkw.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://isy.ybcxt.top

Ruby: Date.parse("2024-01-02")
来源：http://lif.9152youxi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lgx.tanke756.top

[J04] 时间戳与日期互转
来源：http://eur.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fye.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xot.tanke756.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ybm.tarul.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jdk.dashuyun.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iot.nwbrower.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rgw.xziqi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://chs.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hca.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://kxj.wangshuangyany.cn

Py:   now + timedelta(days=7)
来源：http://vrb.hfpthk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yim.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://svf.zhiwuduotai.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gxf.aizwys.cn

Java: LocalDate.now().plusDays(7)
来源：http://zkc.sjlbkw.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dvl.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://bcn.bbcook.cn

C#:   DateTime.Now.AddDays(7)
来源：http://haw.xuanzx.com

[J06] 计算两时间之差
来源：http://luv.jiagoushi.top

Py:   (end - start).total_seconds()
来源：http://hcv.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://dkl.sufxvd.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fbs.jyoumei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://udr.daxiang520.top

Java: Duration.between(start, end).toSeconds()
来源：http://wgl.guowangkeji.top

Go:   end.Sub(start).Hours()
来源：http://urx.shanyushiyangtech.top

Ruby: end - start                 # 返回秒数
来源：http://fbe.havefunace.top

C#:   (end - start).TotalSeconds
来源：http://rrg.nanxuanxn.top

[J07] 比较两个日期
来源：http://lic.haohaochexian.top

Py:   d1 < d2;  d1 == d2
来源：http://rij.pengpengdd.cyou

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zxg.dianchejie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://whc.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://zbl.daria6918.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cxq.yuxming.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://saf.jinghuilouyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fne.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://xzd.shzxlz.cn

[J08] 提取年月日与星期
来源：http://ynx.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://avs.andypj.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://efz.dashuyun.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oju.hongshengwenyu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ilr.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lid.hongshengwenyu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uqa.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nud.xuanzx.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ktc.yvedp.cn

[J09] 时区处理
来源：http://mwm.epnwcf.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nmu.nwbrower.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ada.yongpay.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wye.zhijiandao.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hrl.yj20258.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gba.shangyingyoupin.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jez.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ntd.havefunace.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rdo.nanxuanxn.top

[J10] 取今天 / 本月第一天
来源：http://kfr.sufxvd.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://flp.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lgj.cdnleiting.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dxi.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ses.birdmap.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wbu.vehdjk.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pqz.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ygo.yanxiufei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ait.iojbl.cn

================================================================================
来源：http://nzs.nanxuanxn.top

K. JSON 与序列化
来源：http://bxd.jinghuilouyu.cn

================================================================================
来源：http://dom.dianchejie.cn

[K01] 对象转 JSON 字符串
来源：http://ive.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eyy.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fvf.hcnkem.com

JS:   JSON.stringify(obj)
来源：http://isn.ydjk.org.cn

TS:   JSON.stringify(obj)
来源：http://crk.zdqjudy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://poz.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://bea.zdqjudy.top

Ruby: obj.to_json                                     // require "json"
来源：http://liw.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yja.zdbjq.cn

[K02] JSON 字符串转对象
来源：http://pvu.cashguo.top

Py:   json.loads(s)
来源：http://vmy.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://frd.hcnkem.com

JS:   JSON.parse(s)
来源：http://qiw.dianchejie.cn

TS:   JSON.parse(s)
来源：http://dib.hfpthk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tgq.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://sfx.xziqi.cn

Ruby: JSON.parse(s)
来源：http://dpc.birdmap.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ytb.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://men.chenjidiqi.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qyh.jinqigufen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kkc.sxryk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gfm.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gvz.ywan-chungtsiang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tmh.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://njl.tanke756.top

Ruby: JSON.pretty_generate(obj)
来源：http://asn.gotoacloud.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kqc.hywenlv.cn

[K04] 读取 JSON 文件
来源：http://jqu.nanxinkj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bmb.ehwqpu.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dmt.fktsv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qxn.kuanghao11.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vmd.fengsongda.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oug.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tin.yj20258888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jkx.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://byq.xylfe.cn

[K05] 深拷贝对象
来源：http://lus.jiagoushi.top

Py:   copy.deepcopy(obj)
来源：http://uyp.ivvv.top

PHP:  unserialize(serialize($obj));
来源：http://fre.xingfuxueyuan.xyz

JS:   structuredClone(obj)
来源：http://ifz.meibo888.top

TS:   structuredClone(obj)
来源：http://fwp.tianlin.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://opt.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jnx.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ecn.jinyuanbaomall.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ylk.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://fff.sweek.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bzx.cqqwz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oms.hnqzz.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tff.aibaodan.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hjq.dashuyun.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uui.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://nbe.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xzi.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bpi.wangdashe.top

[K07] 进制转换
来源：http://pig.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ycr.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://szj.yonumen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mcr.jinqigufen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qnj.zhixingplan.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nfe.cashguo.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hpc.zhongyouzk.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wrr.cucudq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mme.hongshengwenyu.top

[K08] 二进制序列化（非 JSON）
来源：http://wsx.zdbjq.cn

Py:   pickle.dumps(obj)
来源：http://aho.yangfankeji.com

PHP:  serialize($obj);  unserialize($s);
来源：http://eqc.mhx1999.top

JS:   v8.serialize(obj)        // Node
来源：http://nsx.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://oef.hesvh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dci.yj20258.top

Go:   encoding/gob
来源：http://yjs.hnxiangtu.top

Ruby: Marshal.dump(obj)
来源：http://bwu.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://idn.guowangkeji.top

================================================================================
来源：http://zpn.cashguo.top

L. 网络请求
来源：http://ipj.cqqwz.cn

================================================================================
来源：http://hwi.sysykeji.top

[L01] 发送 GET 请求
来源：http://fmm.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mak.sweek.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kvh.shanyushiyangkeji.top

JS:   await fetch(url)
来源：http://gsf.tarul.cn

TS:   await fetch(url)
来源：http://rgl.sufxvd.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kix.bjfxy.top

Go:   resp, err := http.Get(url)
来源：http://zgt.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://udo.sufxvd.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jxp.0kj1m.cn

[L02] 发送 POST JSON
来源：http://geu.redwolf501.top

Py:   requests.post(url, json={"a": 1})
来源：http://tmy.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qdp.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zza.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gah.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xmg.fengsongda.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vkn.fzhhl.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ogl.chenjidiqi.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kzu.pycfn.com

[L03] 设置自定义请求头
来源：http://nhi.andypj.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vdp.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zfk.zhoulong.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nfc.yj202588.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bpu.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ocj.shuidangran.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yhr.sjlbkw.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ugf.ydjk.org.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fcw.jlsjyb.cn

[L04] 设置超时
来源：http://eyp.dashuyun.cn

Py:   requests.get(url, timeout=5)
来源：http://rhf.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ydo.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://siu.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ezc.cheryme.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kur.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dvi.yuanzhike.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pzj.nwbrower.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pdo.fzhhl.top

[L05] 上传文件（multipart）
来源：http://aap.316326.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kyk.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://erz.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cnr.yj202588.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://com.jianghu66.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nzz.c1oappe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eda.bbcook.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lwp.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ldn.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://zkp.yueranfly.top

Py:   resp.json()
来源：http://cvm.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://gdr.cheryme.top

JS:   await resp.json()
来源：http://txk.jqgfzy.top

TS:   await resp.json()
来源：http://wfo.tianlin.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sel.gotoacloud.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://civ.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://kxk.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jtt.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://edr.gogol.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pbb.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://prq.0kj1m.cn

JS:   resp.ok;  resp.status
来源：http://vvu.yj20258.top

TS:   resp.ok;  resp.status
来源：http://icx.ppjwa.cn

Java: resp.statusCode()
来源：http://pbd.jinqigufen.top

Go:   resp.StatusCode
来源：http://fne.shzxlz.cn

Ruby: resp.code.to_i
来源：http://koy.jqgufenzy.top

C#:   (int)resp.StatusCode
来源：http://kou.yj20258.top

[L08] 并发请求多个地址
来源：http://nby.fktsv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gkj.dianchejie.cn

PHP:  curl_multi_init() 系列
来源：http://nxu.tian-w.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jpk.yanxiufei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vcb.gogol.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mxg.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zmk.jianghu66.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vni.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hsc.dashuyun.cn

================================================================================
来源：http://aje.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境
来源：http://owc.jinqigfzy.top

================================================================================
来源：http://mka.cucudq.cn

[M01] 读取命令行参数
来源：http://yki.ehwqpu.com

Py:   sys.argv[1:]
来源：http://vfm.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://dip.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://fka.xziqi.cn

TS:   process.argv.slice(2)
来源：http://hvh.jinqigufen.top

Java: args 数组（main 方法参数）
来源：http://axi.xziqi.cn

Go:   os.Args[1:]
来源：http://ans.mhx1999.top

Ruby: ARGV
来源：http://fya.sjlbkw.cn

C#:   args 数组（Main 方法参数）
来源：http://dds.hnqzz.top

[M02] 读取环境变量
来源：http://kug.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://drc.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tbt.xuetiantiany.cn

JS:   process.env.HOME
来源：http://kbw.zhijiandao.cn

TS:   process.env.HOME
来源：http://czq.jyoumei.cn

Java: System.getenv("HOME")
来源：http://wzq.dianchejie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ghl.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://air.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fft.sjlbkw.cn

[M03] 执行外部命令
来源：http://jmf.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ybk.316326.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ihy.ppjwa.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ard.shzxlz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nuk.sjlbkw.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://veu.tianlin.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://yst.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://cqc.ehwqpu.com

C#:   Process.Start("ls", "-l");
来源：http://nqy.sufxvd.cn

[M04] 获取当前工作目录
来源：http://qer.mhx1999.top

Py:   os.getcwd()
来源：http://ymu.tianlin.xyz

PHP:  getcwd();
来源：http://zmc.ybcxt.top

JS:   process.cwd()
来源：http://vmk.zycfv.cn

TS:   process.cwd()
来源：http://xvf.yuanzhike.top

Java: Path.of("").toAbsolutePath()
来源：http://miv.jinqigfzy.top

Go:   os.Getwd()
来源：http://fyp.fehbvm.com

Ruby: Dir.pwd
来源：http://vvk.jyoumei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://myi.hywenlv.cn

[M05] 设置退出码
来源：http://hob.yongpay.top

Py:   sys.exit(1)
来源：http://jiq.gogol.net.cn

PHP:  exit(1);
来源：http://nmi.yfazqb.com

JS:   process.exit(1)
来源：http://mix.zycfv.cn

TS:   process.exit(1)
来源：http://hlc.sxryk.cn

Java: System.exit(1)
来源：http://oud.ivvv.top

Go:   os.Exit(1)
来源：http://som.sufxvd.cn

Ruby: exit 1
来源：http://wvu.pycfn.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://prg.epnwcf.com

[M06] 向标准错误输出
来源：http://fat.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://ogn.shangyingyoupin.top

PHP:  fwrite(STDERR, "err\n");
来源：http://igo.zhaomingkeji.xyz

JS:   console.error("err")
来源：http://uyl.bjfxy.top

TS:   console.error("err")
来源：http://pmi.iojbl.cn

Java: System.err.println("err")
来源：http://adq.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rtg.tanke756.top

Ruby: warn "err"
来源：http://jvu.tian-w.cn

C#:   Console.Error.WriteLine("err")
来源：http://nnw.sxryk.cn

[M07] 判断是否为主入口
来源：http://pbe.yuxming.cn

Py:   if __name__ == "__main__":
来源：http://jub.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dex.shanyushiyangtech.top

JS:   require.main === module
来源：http://qji.iojbl.cn

TS:   require.main === module
来源：http://ksf.snrcjt.cn

Java: public static void main(String[] args)
来源：http://dwj.sjlbkw.cn

Go:   func main()
来源：http://zhi.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hbc.shzxlz.cn

C#:   static void Main(string[] args)
来源：http://qcv.quarkkingdee.top

[M08] 获取系统与运行时信息
来源：http://vck.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://iah.c1oappe.top

PHP:  PHP_OS;  phpversion();
来源：http://bne.316326.xyz

JS:   process.platform;  process.version
来源：http://wzg.fktsv.cn

TS:   process.platform;  process.version
来源：http://otp.vqdsnc.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jnc.zhixingplan.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wbr.haohaochexian.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wwg.hesvh.cn


<!-- 参考信息 -->