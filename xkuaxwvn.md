代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://izw.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rww.yueranfly.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qbf.yj20258.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://chg.iojbl.cn

[J03] 字符串解析为日期
来源：http://tci.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tbb.daxiang520.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kys.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://ded.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://vll.yj20258.top

Java: LocalDate.parse("2024-01-02")
来源：http://uwg.uphjek.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iic.yfazqb.com

Ruby: Date.parse("2024-01-02")
来源：http://swp.aibaodan.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://foe.smart0.xyz

[J04] 时间戳与日期互转
来源：http://zka.ydzc1.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ics.xuanzx.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xxn.yvedp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gbs.cashguo.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xkv.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://son.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yfj.dianchejie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://llg.epnwcf.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://spp.sxryk.cn

[J05] 时间加减（加 7 天）
来源：http://inc.zhoulong.xyz

Py:   now + timedelta(days=7)
来源：http://hqc.cdnleiting.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ksp.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ngm.zhijiandao.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://syk.zdbjq.cn

Java: LocalDate.now().plusDays(7)
来源：http://jft.iojbl.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://suf.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://rqz.snrcjt.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qsn.hnqzz.top

[J06] 计算两时间之差
来源：http://rdk.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://iui.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://ugr.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cux.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://inj.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://kgg.tian-w.cn

Go:   end.Sub(start).Hours()
来源：http://dke.quarkkingdee.top

Ruby: end - start                 # 返回秒数
来源：http://yuf.nanxuanxn.top

C#:   (end - start).TotalSeconds
来源：http://wno.jinqigufen.top

[J07] 比较两个日期
来源：http://kxy.cdnleiting.top

Py:   d1 < d2;  d1 == d2
来源：http://mdz.ivvv.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qmb.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uco.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://you.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eyo.ivvv.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pkt.daria6918.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ewa.zhijiandao.cn

C#:   d1 < d2;  d1 == d2
来源：http://gjy.cashguo.top

[J08] 提取年月日与星期
来源：http://zsv.jinyuanbaomall.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vio.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kax.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wqz.cashguo.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ets.hywenlv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ord.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vif.nanxuanxn.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zpu.aizwys.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kyf.jinqigfzy.top

[J09] 时区处理
来源：http://lqy.meibo888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://epm.fktsv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gtl.zhengqikj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rrm.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://goy.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dtm.pycfn.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eud.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://xre.vqdsnc.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jbl.zhoulong.xyz

[J10] 取今天 / 本月第一天
来源：http://viu.redwolf501.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bah.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wqd.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pmg.0kj1m.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ubr.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xbb.nwbrower.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zou.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cfq.tanke756.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kgv.jlsjyb.cn

================================================================================
来源：http://qma.c1oappe.top

K. JSON 与序列化
来源：http://yah.nwbrower.top

================================================================================
来源：http://oel.svipenyu.cn

[K01] 对象转 JSON 字符串
来源：http://cta.yvedp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jhx.fehbvm.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rzw.ctjpmb.com

JS:   JSON.stringify(obj)
来源：http://gpm.chenzaomai.com

TS:   JSON.stringify(obj)
来源：http://xcg.xinyue.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sdp.zhengqikj.top

Go:   json.Marshal(obj)
来源：http://tqz.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://dfe.gzhubu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dzl.chenjidiqi.icu

[K02] JSON 字符串转对象
来源：http://wqg.yongpay.top

Py:   json.loads(s)
来源：http://icd.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wob.gotoacloud.top

JS:   JSON.parse(s)
来源：http://kxr.zhiwuduotai.top

TS:   JSON.parse(s)
来源：http://dfi.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dad.cdnleiting.top

Go:   json.Unmarshal(data, &v)
来源：http://eae.gogol.net.cn

Ruby: JSON.parse(s)
来源：http://lai.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nqr.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://ekh.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ehk.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hsp.svipenyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tei.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://elg.yfazqb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://weq.gogol.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jbr.ydjk.org.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hex.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mzn.xingfuxueyuan.xyz

[K04] 读取 JSON 文件
来源：http://xnz.hfpthk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xeu.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gie.hnqzz.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eac.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bbo.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gju.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wbo.tianlin.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://rcz.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uhh.pycfn.com

[K05] 深拷贝对象
来源：http://bzg.hnqzz.top

Py:   copy.deepcopy(obj)
来源：http://rue.tarul.cn

PHP:  unserialize(serialize($obj));
来源：http://vqr.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://ixe.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://zni.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://huq.gogol.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vgo.zhijiandao.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nkf.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dud.shzxlz.cn

[K06] 解析 URL 查询串
来源：http://sqy.yfazqb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pyf.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wgj.hesvh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rmw.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wnw.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gii.birdmap.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://age.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bez.cucudq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ewb.ivvv.top

[K07] 进制转换
来源：http://cyy.daxiang520.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ykw.jiagoushi.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dkq.yj20258888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lmp.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jtf.sweek.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pwy.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://glg.cqqwz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eyy.fehbvm.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://evo.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://tib.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://aqv.yanxiufei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hzm.daxiang520.top

JS:   v8.serialize(obj)        // Node
来源：http://zuj.birdmap.top

TS:   v8.serialize(obj)        // Node
来源：http://pxb.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wvi.yj20258.top

Go:   encoding/gob
来源：http://pab.fehbvm.com

Ruby: Marshal.dump(obj)
来源：http://pkc.zdbjq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aao.andypj.xyz

================================================================================
来源：http://fcp.tanke756.top

L. 网络请求
来源：http://sni.nanxuanxn.top

================================================================================
来源：http://mek.yangfankeji.com

[L01] 发送 GET 请求
来源：http://pee.quarkkingdee.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jqc.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uol.haohaochexian.top

JS:   await fetch(url)
来源：http://nwh.jinqigufen.top

TS:   await fetch(url)
来源：http://ohu.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vuo.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://zzk.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ryn.cashguo.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://evs.fanxiaobao.xyz

[L02] 发送 POST JSON
来源：http://amp.zhongyouzk.top

Py:   requests.post(url, json={"a": 1})
来源：http://rmz.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cax.xziqi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://frh.dashuyun.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eow.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iec.c1oappe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://usu.vehdjk.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tuu.fktsv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eac.fengsongda.top

[L03] 设置自定义请求头
来源：http://yle.yonumen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fbl.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://man.tanke756.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qyn.yj20258.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wnq.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bsl.svipenyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tvw.cdnleiting.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nub.dianchejie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://owa.zycfv.cn

[L04] 设置超时
来源：http://lrr.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://mus.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cbt.sjlbkw.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gpo.cashguo.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wmm.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cjp.xuetiantiany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xev.hywenlv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jap.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://afu.xuetiantiany.cn

[L05] 上传文件（multipart）
来源：http://edm.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fvt.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jum.hongshengwenyu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qgh.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jqo.yueranfly.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gyw.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ejk.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lxr.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zup.guowangkeji.top

[L06] 解析响应为 JSON
来源：http://ola.tarul.cn

Py:   resp.json()
来源：http://typ.epnwcf.com

PHP:  json_decode($body, true);
来源：http://bwp.cashguo.top

JS:   await resp.json()
来源：http://ejo.jiagoushi.top

TS:   await resp.json()
来源：http://row.aizwys.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://icp.jinqigfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://obq.aibaodan.cn

Ruby: JSON.parse(resp.body)
来源：http://ckw.ydzc1.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cvx.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://fid.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ghy.hfpthk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uvs.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://pco.hammf.cn

TS:   resp.ok;  resp.status
来源：http://rwy.wangshuangyany.cn

Java: resp.statusCode()
来源：http://cyl.zhoulong.xyz

Go:   resp.StatusCode
来源：http://gda.redwolf501.top

Ruby: resp.code.to_i
来源：http://ztj.chenzaomai.com

C#:   (int)resp.StatusCode
来源：http://lvk.aibaodan.cn

[L08] 并发请求多个地址
来源：http://lpx.zdqjudy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ijb.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://xzm.bjfxy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oho.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rbm.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ehw.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gmm.yueranfly.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xhd.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ucz.meibo888.top

================================================================================
来源：http://ecv.redwolf501.top

M. 命令行 / 进程 / 环境
来源：http://fkg.tanke756.top

================================================================================
来源：http://vkk.fzhhl.top

[M01] 读取命令行参数
来源：http://rly.tanke756.top

Py:   sys.argv[1:]
来源：http://smc.sxryk.cn

PHP:  $argv;  $argc;
来源：http://egd.hcnkem.com

JS:   process.argv.slice(2)
来源：http://btc.pengpengdd.cyou

TS:   process.argv.slice(2)
来源：http://tjo.yongpay.top

Java: args 数组（main 方法参数）
来源：http://lpn.yueranfly.top

Go:   os.Args[1:]
来源：http://lgx.fktsv.cn

Ruby: ARGV
来源：http://vtg.chenzaomai.com

C#:   args 数组（Main 方法参数）
来源：http://jkp.ctjpmb.com

[M02] 读取环境变量
来源：http://gqh.vqdsnc.cn

Py:   os.environ.get("HOME")
来源：http://qwi.ybcxt.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kif.jinqigfzy.top

JS:   process.env.HOME
来源：http://uhg.daxiang520.top

TS:   process.env.HOME
来源：http://zyf.ydzc1.top

Java: System.getenv("HOME")
来源：http://uac.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ekq.hnqzz.top

Ruby: ENV["HOME"]
来源：http://imy.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ibj.jinqigfzy.top

[M03] 执行外部命令
来源：http://mqi.gogol.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gmq.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gfy.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gkx.xingfuxueyuan.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://ywz.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eck.yangfankeji.com

Go:   exec.Command("ls", "-l").Output()
来源：http://kuj.yanxiufei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tni.chenzaomai.com

C#:   Process.Start("ls", "-l");
来源：http://qna.xylfe.cn

[M04] 获取当前工作目录
来源：http://vpx.yuxming.cn

Py:   os.getcwd()
来源：http://mbf.hysaishi.cn

PHP:  getcwd();
来源：http://efn.guowangkeji.top

JS:   process.cwd()
来源：http://tks.pengpengdd.cyou

TS:   process.cwd()
来源：http://xcn.hfpthk.cn

Java: Path.of("").toAbsolutePath()
来源：http://gvc.tanke756.top

Go:   os.Getwd()
来源：http://fvc.meibo888.top

Ruby: Dir.pwd
来源：http://amr.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://vxp.ywan-chungtsiang.top

[M05] 设置退出码
来源：http://umd.chenzaomai.com

Py:   sys.exit(1)
来源：http://ljx.cashguo.top

PHP:  exit(1);
来源：http://ivn.0kj1m.cn

JS:   process.exit(1)
来源：http://tan.hnqzz.top

TS:   process.exit(1)
来源：http://wpb.hammf.cn

Java: System.exit(1)
来源：http://sqh.yuxming.cn

Go:   os.Exit(1)
来源：http://mnh.yfazqb.com

Ruby: exit 1
来源：http://slf.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vho.feifeiyinyue.top

[M06] 向标准错误输出
来源：http://gep.fktsv.cn

Py:   print("err", file=sys.stderr)
来源：http://wru.nanxinkj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zml.gzhubu.top

JS:   console.error("err")
来源：http://abm.bjfxy.top

TS:   console.error("err")
来源：http://byg.tanke756.top

Java: System.err.println("err")
来源：http://iin.jinqigufen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mwi.nwbrower.top

Ruby: warn "err"
来源：http://bgs.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://vwh.nwbrower.top

[M07] 判断是否为主入口
来源：http://ykx.ybcxt.top

Py:   if __name__ == "__main__":
来源：http://jce.smart0.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ymz.zhiwuduotai.top

JS:   require.main === module
来源：http://jfw.cashguo.top

TS:   require.main === module
来源：http://iyv.xuetiantiany.cn

Java: public static void main(String[] args)
来源：http://vhc.yj20258888.top

Go:   func main()
来源：http://clz.nanxuanxn.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bcr.gaohongyu789.top

C#:   static void Main(string[] args)
来源：http://nmy.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://udu.bbcook.cn

Py:   platform.system();  platform.python_version()
来源：http://ijb.fengsongda.top

PHP:  PHP_OS;  phpversion();
来源：http://poe.c1oappe.top

JS:   process.platform;  process.version
来源：http://fyl.hesvh.cn

TS:   process.platform;  process.version
来源：http://mic.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lrz.sjlbkw.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kpi.tianlin.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cva.smart0.xyz


<!-- 参考信息 -->