代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cld.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://rtj.yueranfly.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dqt.sjlbkw.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mfk.zhoulong.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://duo.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://qql.ydjk.org.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zbw.smart0.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nvk.hnqzz.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xcm.xziqi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ngn.iojbl.cn

[J05] 时间加减（加 7 天）
来源：http://szg.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://ygc.hnxiangtu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fze.cucudq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cbf.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lnd.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://tzm.jiagoushi.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ikg.wangshuangyany.cn

Ruby: Time.now + 7 * 86400
来源：http://mcb.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://rvh.guowangkeji.top

[J06] 计算两时间之差
来源：http://zkk.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://iub.ppjwa.cn

PHP:  $end->diff($start)->days;
来源：http://jps.nwbrower.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://htv.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://toj.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://lib.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://egu.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://pok.ybcxt.top

C#:   (end - start).TotalSeconds
来源：http://dvv.c1oappe.top

[J07] 比较两个日期
来源：http://fwm.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://jwj.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bci.ydjk.org.cn

JS:   d1.getTime() < d2.getTime()
来源：http://flk.aizwys.cn

TS:   d1.getTime() < d2.getTime()
来源：http://loy.chenlongwang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xwi.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bxy.sweek.top

Ruby: d1 < d2;  d1 == d2
来源：http://tmb.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://kbj.aizwys.cn

[J08] 提取年月日与星期
来源：http://wst.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mrc.fanxiaobao.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tab.zdbjq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://azf.yvedp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xtp.hnqzz.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ppn.bbcook.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rly.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jed.ywan-chungtsiang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ruw.svipenyu.cn

[J09] 时区处理
来源：http://wna.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ygv.pycfn.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vxl.yj20258888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://buw.yongpay.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ogu.shzxlz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ncn.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ktj.yuxming.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lcy.zhoulong.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://khs.ywan-chungtsiang.top

[J10] 取今天 / 本月第一天
来源：http://utn.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nod.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wgh.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tpe.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rfw.hesvh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://myc.gogol.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zce.fanxiaobao.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vyo.gogol.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nzh.cheryme.top

================================================================================
来源：http://lim.cdnleiting.top

K. JSON 与序列化
来源：http://tfa.ctjpmb.com

================================================================================
来源：http://zid.havefunace.top

[K01] 对象转 JSON 字符串
来源：http://fve.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wla.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://owk.316326.xyz

JS:   JSON.stringify(obj)
来源：http://bjw.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://ryg.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hqw.fzhhl.top

Go:   json.Marshal(obj)
来源：http://ixn.shuidangran.top

Ruby: obj.to_json                                     // require "json"
来源：http://pxp.tianlin.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://ogc.jianghu66.top

[K02] JSON 字符串转对象
来源：http://vld.jianghu66.top

Py:   json.loads(s)
来源：http://lhg.birdmap.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ppq.havefunace.top

JS:   JSON.parse(s)
来源：http://hex.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://zbg.zhongyouzk.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cvc.redwolf501.top

Go:   json.Unmarshal(data, &v)
来源：http://faf.guannengcc.top

Ruby: JSON.parse(s)
来源：http://kwn.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mgd.yonumen.top

[K03] JSON 美化输出（带缩进）
来源：http://ppp.quarkkingdee.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jts.hnxiangtu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aoh.yanxiufei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pnn.zdqjudy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://sjd.52xcode.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fzr.xinyue.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wpg.hnqzz.top

Ruby: JSON.pretty_generate(obj)
来源：http://qwd.andypj.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ncj.gotoacloud.top

[K04] 读取 JSON 文件
来源：http://hab.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jry.jyoumei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uvj.yfazqb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dwm.yanxiufei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ebv.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ecv.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zxu.daria6918.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://akf.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ztn.smart0.xyz

[K05] 深拷贝对象
来源：http://xpi.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://kva.zhengqikj.top

PHP:  unserialize(serialize($obj));
来源：http://mzb.yj202588.top

JS:   structuredClone(obj)
来源：http://roe.dianchejie.cn

TS:   structuredClone(obj)
来源：http://dzm.ydjk.org.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nlj.gogol.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://omj.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vwe.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yzn.sxryk.cn

[K06] 解析 URL 查询串
来源：http://gad.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pga.52xcode.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://upq.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ude.ywan-chungtsiang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oer.tarul.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://umt.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pwh.fengsongda.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gaj.feifeiyinyue.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qpg.uphjek.com

[K07] 进制转换
来源：http://elg.guannengcc.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ojw.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bjr.jinyuanbaomall.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cgz.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://suj.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://exb.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://out.haohaochexian.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zvm.yvedp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ziz.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://rac.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://uqt.jyoumei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://iuy.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://zpo.yongpay.top

TS:   v8.serialize(obj)        // Node
来源：http://nti.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mck.shzxlz.cn

Go:   encoding/gob
来源：http://uzg.yuanzhike.top

Ruby: Marshal.dump(obj)
来源：http://ujp.hongshengwenyu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ety.sjlbkw.cn

================================================================================
来源：http://cny.yongpay.top

L. 网络请求
来源：http://hfg.xylfe.cn

================================================================================
来源：http://eab.tianlin.xyz

[L01] 发送 GET 请求
来源：http://fvr.feifeiyinyue.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hiq.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zds.hesvh.cn

JS:   await fetch(url)
来源：http://gew.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://rde.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bmy.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://uzk.fengsongda.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gzf.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hxu.tianlin.xyz

[L02] 发送 POST JSON
来源：http://kdj.jyoumei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://chi.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qxd.hnxiangtu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://myx.nanxinkj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ezb.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wry.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://osg.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ixf.pycfn.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nae.0kj1m.cn

[L03] 设置自定义请求头
来源：http://qzw.snrcjt.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zxq.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fxf.cucudq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dxw.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nig.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mqr.ehwqpu.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ukl.sufxvd.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cdn.cqqwz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jll.yonumen.top

[L04] 设置超时
来源：http://awx.epnwcf.com

Py:   requests.get(url, timeout=5)
来源：http://jnp.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bpx.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yxt.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fsv.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wkq.aizwys.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yto.sufxvd.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vzx.fzhhl.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sxj.kuanghao11.cn

[L05] 上传文件（multipart）
来源：http://dba.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jtk.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mrj.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rqp.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nuk.kuanghao11.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ckm.xingfuxueyuan.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dag.nwbrower.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rze.sweek.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cmm.iojbl.cn

[L06] 解析响应为 JSON
来源：http://ubn.ywan-chungtsiang.top

Py:   resp.json()
来源：http://zks.tarul.cn

PHP:  json_decode($body, true);
来源：http://bsv.xuetiantiany.cn

JS:   await resp.json()
来源：http://maz.zhiwuduotai.top

TS:   await resp.json()
来源：http://fxc.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uqh.ivvv.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ept.sjlbkw.cn

Ruby: JSON.parse(resp.body)
来源：http://cgp.birdmap.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://axy.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://vpu.hongshengwenyu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yxl.xinyue.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jok.tanke756.top

JS:   resp.ok;  resp.status
来源：http://bvt.yongpay.top

TS:   resp.ok;  resp.status
来源：http://abu.smart0.xyz

Java: resp.statusCode()
来源：http://crh.fengsongda.top

Go:   resp.StatusCode
来源：http://qju.yj20258.top

Ruby: resp.code.to_i
来源：http://pcd.bjfxy.top

C#:   (int)resp.StatusCode
来源：http://tdp.zhiwuduotai.top

[L08] 并发请求多个地址
来源：http://gtp.aibaodan.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xet.ehwqpu.com

PHP:  curl_multi_init() 系列
来源：http://tgx.yongpay.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pjt.fktsv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ttx.nwbrower.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vyh.gaohongyu789.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://esl.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pst.snrcjt.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lts.shzxlz.cn

================================================================================
来源：http://trz.yueranfly.top

M. 命令行 / 进程 / 环境
来源：http://gjr.ybcxt.top

================================================================================
来源：http://cek.nanxinkj.top

[M01] 读取命令行参数
来源：http://abn.xuetiantiany.cn

Py:   sys.argv[1:]
来源：http://sdz.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://wjx.daxiang520.top

JS:   process.argv.slice(2)
来源：http://zqw.guowangkeji.top

TS:   process.argv.slice(2)
来源：http://hpu.meibo888.top

Java: args 数组（main 方法参数）
来源：http://bmb.daria6918.cn

Go:   os.Args[1:]
来源：http://zya.xziqi.cn

Ruby: ARGV
来源：http://lcw.jlsjyb.cn

C#:   args 数组（Main 方法参数）
来源：http://zml.smart0.xyz

[M02] 读取环境变量
来源：http://vlw.yongpay.top

Py:   os.environ.get("HOME")
来源：http://lgo.tanke756.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vdk.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://moq.xziqi.cn

TS:   process.env.HOME
来源：http://vfh.zhiwuduotai.top

Java: System.getenv("HOME")
来源：http://gvz.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eks.ydjk.org.cn

Ruby: ENV["HOME"]
来源：http://rlj.cqqwz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ozq.pengpengdd.cyou

[M03] 执行外部命令
来源：http://jza.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gic.cqqwz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dux.hesvh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zls.aizwys.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://auu.pycfn.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hol.cucudq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cfd.hcnkem.com

Ruby: system("ls -l");  `ls -l`
来源：http://vxt.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://zuo.wangdashe.top

[M04] 获取当前工作目录
来源：http://kay.0kj1m.cn

Py:   os.getcwd()
来源：http://kwa.gzhubu.top

PHP:  getcwd();
来源：http://qnw.yj20258888.top

JS:   process.cwd()
来源：http://zhr.nanxuanxn.top

TS:   process.cwd()
来源：http://ggx.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://ziy.fzhhl.top

Go:   os.Getwd()
来源：http://vaa.yj20258888.top

Ruby: Dir.pwd
来源：http://omw.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://svb.tanke756.top

[M05] 设置退出码
来源：http://dxa.guannengcc.top

Py:   sys.exit(1)
来源：http://ahb.fanxiaobao.xyz

PHP:  exit(1);
来源：http://jkn.sweek.top

JS:   process.exit(1)
来源：http://fdf.gzhubu.top

TS:   process.exit(1)
来源：http://ixy.sjlbkw.cn

Java: System.exit(1)
来源：http://bbw.xylfe.cn

Go:   os.Exit(1)
来源：http://zuw.jqgfzy.top

Ruby: exit 1
来源：http://ddu.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://osk.0kj1m.cn

[M06] 向标准错误输出
来源：http://iyk.aizwys.cn

Py:   print("err", file=sys.stderr)
来源：http://uaz.smart0.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://kno.316326.xyz

JS:   console.error("err")
来源：http://bar.yangfankeji.com

TS:   console.error("err")
来源：http://mea.wangshuangyany.cn

Java: System.err.println("err")
来源：http://cjn.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pyd.jianghu66.top

Ruby: warn "err"
来源：http://pck.zdbjq.cn

C#:   Console.Error.WriteLine("err")
来源：http://yjq.yanxiufei.cn

[M07] 判断是否为主入口
来源：http://ebi.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://squ.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uyt.shangyingyoupin.top

JS:   require.main === module
来源：http://fzm.mhx1999.top

TS:   require.main === module
来源：http://oez.mhx1999.top

Java: public static void main(String[] args)
来源：http://dkh.zhaomingkeji.xyz

Go:   func main()
来源：http://bfy.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cpt.zhijiandao.cn

C#:   static void Main(string[] args)
来源：http://hfk.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://iaf.snrcjt.cn

Py:   platform.system();  platform.python_version()
来源：http://rua.tarul.cn

PHP:  PHP_OS;  phpversion();
来源：http://caq.yj202588.top

JS:   process.platform;  process.version
来源：http://uao.c1oappe.top

TS:   process.platform;  process.version
来源：http://mog.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yxi.jlsjyb.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vsd.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ejd.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://pbe.pengpengdd.cyou

================================================================================
来源：http://dmy.yongpay.top

N. 数据结构与算法
来源：http://byj.sweek.top

================================================================================
来源：http://jax.nanxinkj.top

[N01] 二分查找（有序数组）
来源：http://stj.xziqi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fem.fanxiaobao.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kjy.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nfm.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kzi.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://efx.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://rps.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://sqv.feifeiyinyue.top


<!-- 参考信息 -->