代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cdn.ydzc1.top

JS:   new Date();  Date.now()
来源：http://gqg.pengpengdd.cyou

TS:   new Date();  Date.now()
来源：http://ptc.zhixingplan.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qvc.yangfankeji.com

Go:   time.Now()
来源：http://ytv.ywan-chungtsiang.top

Ruby: Time.now
来源：http://qgf.dianchejie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vdh.nanxuanxn.top

[J02] 格式化输出
来源：http://qum.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tkc.havefunace.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vto.dianchejie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mus.haohaochexian.top

TS:   d.toISOString()
来源：http://zri.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vrr.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://smn.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mur.xuetiantiany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://red.jinqigfzy.top

[J03] 字符串解析为日期
来源：http://nju.yuxming.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nre.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mbn.andypj.xyz

JS:   new Date("2024-01-02")
来源：http://viu.jiagoushi.top

TS:   new Date("2024-01-02")
来源：http://iip.316326.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://cqt.zdqjudy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xhy.haohaochexian.top

Ruby: Date.parse("2024-01-02")
来源：http://gri.xziqi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kjp.zhaomingkeji.xyz

[J04] 时间戳与日期互转
来源：http://hua.ydzc1.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jtc.vehdjk.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sel.xuanzx.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rze.iojbl.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yyk.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fsj.tarul.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bgt.xuetiantiany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lkv.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qga.zhengqikj.top

[J05] 时间加减（加 7 天）
来源：http://ipt.pycfn.com

Py:   now + timedelta(days=7)
来源：http://lkr.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://uha.xylfe.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jia.fehbvm.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://onp.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://tqn.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qls.hnqzz.top

Ruby: Time.now + 7 * 86400
来源：http://kiq.nanxuanxn.top

C#:   DateTime.Now.AddDays(7)
来源：http://req.cheryme.top

[J06] 计算两时间之差
来源：http://pic.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://hpi.ywan-chungtsiang.top

PHP:  $end->diff($start)->days;
来源：http://ixj.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://art.hnqzz.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qku.shuidangran.top

Java: Duration.between(start, end).toSeconds()
来源：http://qij.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://wxg.kuanghao11.cn

Ruby: end - start                 # 返回秒数
来源：http://dzx.xuetiantiany.cn

C#:   (end - start).TotalSeconds
来源：http://szh.wangdashe.top

[J07] 比较两个日期
来源：http://urj.redwolf501.top

Py:   d1 < d2;  d1 == d2
来源：http://uya.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://map.xuetiantiany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jnp.zhongyouzk.top

TS:   d1.getTime() < d2.getTime()
来源：http://vrl.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yub.gogol.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wgq.zhixingplan.top

Ruby: d1 < d2;  d1 == d2
来源：http://rlt.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://lvx.tian-w.cn

[J08] 提取年月日与星期
来源：http://etm.aibaodan.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bff.jianghu66.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.sysykeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xxx.bbcook.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vym.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pip.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://duk.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://drq.xingfuxueyuan.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://msl.birdmap.top

[J09] 时区处理
来源：http://dxf.zhongyouzk.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pst.guannengcc.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bzz.shangyingyoupin.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vho.zhengqikj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uqh.jinyuanbaomall.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yws.guowangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qtg.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dyq.yj202588.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gsh.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://clg.guowangkeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fmn.nwbrower.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kex.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ovp.fktsv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kmj.andypj.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yoi.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uzr.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aqb.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wyw.ctjpmb.com

================================================================================
来源：http://ttb.gzhubu.top

K. JSON 与序列化
来源：http://xhc.xylfe.cn

================================================================================
来源：http://ndx.hcnkem.com

[K01] 对象转 JSON 字符串
来源：http://nmc.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rnf.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://huz.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://gaa.yangfankeji.com

TS:   JSON.stringify(obj)
来源：http://jmy.shanyushiyangtech.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jrf.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://avi.meibo888.top

Ruby: obj.to_json                                     // require "json"
来源：http://upl.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vht.shzxlz.cn

[K02] JSON 字符串转对象
来源：http://iou.fktsv.cn

Py:   json.loads(s)
来源：http://qco.hnqzz.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lxv.yuxming.cn

JS:   JSON.parse(s)
来源：http://hqu.xinyue.icu

TS:   JSON.parse(s)
来源：http://wzp.sweek.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mfe.sjlbkw.cn

Go:   json.Unmarshal(data, &v)
来源：http://odn.epnwcf.com

Ruby: JSON.parse(s)
来源：http://kuu.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pzk.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://scg.hnxiangtu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kmb.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jyt.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://whs.iojbl.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oyh.yfazqb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gtq.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://veo.daxiang520.top

Ruby: JSON.pretty_generate(obj)
来源：http://frl.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hxg.52xcode.cn

[K04] 读取 JSON 文件
来源：http://qki.hcnkem.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kkp.jinqigfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cij.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://phf.nanxinkj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rxl.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yxw.0kj1m.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://brm.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ixe.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ite.fktsv.cn

[K05] 深拷贝对象
来源：http://rhk.yj20258888.top

Py:   copy.deepcopy(obj)
来源：http://hfy.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://qiy.fengsongda.top

JS:   structuredClone(obj)
来源：http://oiy.gaohongyu789.top

TS:   structuredClone(obj)
来源：http://ccu.cdnleiting.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bwl.ivvv.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nfy.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://skt.vqdsnc.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kxu.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://xba.feifeiyinyue.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rtd.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wwv.guannengcc.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oxh.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jib.tanke756.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xbd.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mrd.hammf.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xzk.feifeiyinyue.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fqs.ywan-chungtsiang.top

[K07] 进制转换
来源：http://qgb.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vjo.dashuyun.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ixd.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://axh.daxiang520.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://koj.yueranfly.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ivo.aizwys.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oyd.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hlr.yongpay.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jnn.52xcode.cn

[K08] 二进制序列化（非 JSON）
来源：http://qhr.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://tev.xuetiantiany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vtx.haohaochexian.top

JS:   v8.serialize(obj)        // Node
来源：http://ais.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://rjk.sysykeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yzd.cucudq.cn

Go:   encoding/gob
来源：http://pxu.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://gxw.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sql.jinqigufen.top

================================================================================
来源：http://xcx.gotoacloud.top

L. 网络请求
来源：http://hsv.cqqwz.cn

================================================================================
来源：http://vae.zhoulong.xyz

[L01] 发送 GET 请求
来源：http://spq.shangyingyoupin.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jer.yanxiufei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rpg.cqqwz.cn

JS:   await fetch(url)
来源：http://wyq.bbcook.cn

TS:   await fetch(url)
来源：http://poq.xingfuxueyuan.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cbt.pengpengdd.cyou

Go:   resp, err := http.Get(url)
来源：http://bcd.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://hbk.zdqjudy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fyg.yvedp.cn

[L02] 发送 POST JSON
来源：http://uwg.ywan-chungtsiang.top

Py:   requests.post(url, json={"a": 1})
来源：http://deb.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iwd.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hkm.zdbjq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://roo.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bok.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vdi.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://byu.vqdsnc.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zpm.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://vzb.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zww.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qua.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://loe.nanxuanxn.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ccl.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xgh.hysaishi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ddq.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vpm.hywenlv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lqw.jinyuanbaomall.cn

[L04] 设置超时
来源：http://xlc.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://ree.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bbm.gzhubu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xvh.haohaochexian.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jzu.sufxvd.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vgx.gogol.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://igl.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ugx.shanyushiyangtech.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://flc.yueranfly.top

[L05] 上传文件（multipart）
来源：http://nlh.shuidangran.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tpg.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pnb.cheryme.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nhz.zdqjudy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://reg.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ziq.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hpp.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vzh.cqqwz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dub.pycfn.com

[L06] 解析响应为 JSON
来源：http://ota.yj20258888.top

Py:   resp.json()
来源：http://ird.yfazqb.com

PHP:  json_decode($body, true);
来源：http://xlp.jqgufenzy.top

JS:   await resp.json()
来源：http://jdx.chenjidiqi.icu

TS:   await resp.json()
来源：http://qtp.nanxuanxn.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eaf.dianchejie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sdk.ppjwa.cn

Ruby: JSON.parse(resp.body)
来源：http://jtx.fehbvm.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://use.jinghuilouyu.cn

[L07] 处理 HTTP 状态码
来源：http://ghy.kuanghao11.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://csn.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blf.zhijiandao.cn

JS:   resp.ok;  resp.status
来源：http://vci.guowangkeji.top

TS:   resp.ok;  resp.status
来源：http://bko.hesvh.cn

Java: resp.statusCode()
来源：http://szx.shuidangran.top

Go:   resp.StatusCode
来源：http://ryu.hammf.cn

Ruby: resp.code.to_i
来源：http://kas.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://nqh.kuanghao11.cn

[L08] 并发请求多个地址
来源：http://bdr.dianchejie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xxd.xziqi.cn

PHP:  curl_multi_init() 系列
来源：http://ijo.snrcjt.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kdw.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://esg.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cjf.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://snp.gzhubu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ppg.zycfv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gqe.wangshuangyany.cn

================================================================================
来源：http://xdf.ydzc1.top

M. 命令行 / 进程 / 环境
来源：http://uwn.bbcook.cn

================================================================================
来源：http://jrn.hnxiangtu.top

[M01] 读取命令行参数
来源：http://dru.zhengqikj.top

Py:   sys.argv[1:]
来源：http://iql.svipenyu.cn

PHP:  $argv;  $argc;
来源：http://wel.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://rve.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://kro.dianchejie.cn

Java: args 数组（main 方法参数）
来源：http://uzs.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://mzw.quarkkingdee.top

Ruby: ARGV
来源：http://gwn.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://aam.cucudq.cn

[M02] 读取环境变量
来源：http://bvv.xylfe.cn

Py:   os.environ.get("HOME")
来源：http://ptu.ydjk.org.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qjz.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://wks.sxryk.cn

TS:   process.env.HOME
来源：http://kzr.pycfn.com

Java: System.getenv("HOME")
来源：http://yrh.ppjwa.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bjk.xinyue.icu

Ruby: ENV["HOME"]
来源：http://mgc.iojbl.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lsh.epnwcf.com

[M03] 执行外部命令
来源：http://xew.hysaishi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mkf.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uzc.ybcxt.top

JS:   child_process.execSync("ls -l").toString()
来源：http://aza.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://voj.meibo888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qyb.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xtn.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lzr.shangyingyoupin.top

C#:   Process.Start("ls", "-l");
来源：http://jls.smart0.xyz

[M04] 获取当前工作目录
来源：http://frn.dianchejie.cn

Py:   os.getcwd()
来源：http://knv.shangyingyoupin.top

PHP:  getcwd();
来源：http://fmw.fengsongda.top

JS:   process.cwd()
来源：http://gtz.sufxvd.cn

TS:   process.cwd()
来源：http://frx.yvedp.cn

Java: Path.of("").toAbsolutePath()
来源：http://wds.wangdashe.top

Go:   os.Getwd()
来源：http://rqz.sjlbkw.cn

Ruby: Dir.pwd
来源：http://jna.epnwcf.com

C#:   Directory.GetCurrentDirectory()
来源：http://hlm.mhx1999.top

[M05] 设置退出码
来源：http://bzp.sysykeji.top

Py:   sys.exit(1)
来源：http://nnq.gaohongyu789.top

PHP:  exit(1);
来源：http://tzm.cucudq.cn

JS:   process.exit(1)
来源：http://yrx.yj202588.top

TS:   process.exit(1)
来源：http://pyz.jianghu66.top

Java: System.exit(1)
来源：http://zss.bjfxy.top

Go:   os.Exit(1)
来源：http://gdw.hnqzz.top

Ruby: exit 1
来源：http://sol.52xcode.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xxs.chenlongwang.top

[M06] 向标准错误输出
来源：http://qes.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://lnb.sufxvd.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ffx.xinyue.icu

JS:   console.error("err")
来源：http://asw.guowangkeji.top

TS:   console.error("err")
来源：http://brx.bjfxy.top

Java: System.err.println("err")
来源：http://ubk.zhaomingkeji.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fkc.guowangkeji.top

Ruby: warn "err"
来源：http://iur.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://yvg.ehwqpu.com

[M07] 判断是否为主入口
来源：http://cid.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://uon.9152youxi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://len.hammf.cn

JS:   require.main === module
来源：http://yab.jqgufenzy.top

TS:   require.main === module
来源：http://dws.bbcook.cn


<!-- 参考信息 -->