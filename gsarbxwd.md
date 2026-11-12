代发 wailian999

TS:   new Date("2024-01-02")
来源：http://ygp.shzxlz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ibc.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yiu.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://prz.hnxiangtu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ypt.xziqi.cn

[J04] 时间戳与日期互转
来源：http://uhb.jianghu66.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lna.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lcf.fzhhl.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nkc.nwbrower.top

TS:   Math.floor(Date.now() / 1000)
来源：http://osv.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gjg.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://shv.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://inp.yj20258.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://odc.meibo888.top

[J05] 时间加减（加 7 天）
来源：http://ghn.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://jzp.guannengcc.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hje.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kue.hongshengwenyu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vgs.hywenlv.cn

Java: LocalDate.now().plusDays(7)
来源：http://wvd.hesvh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pzz.tanke756.top

Ruby: Time.now + 7 * 86400
来源：http://dpb.jinghuilouyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://aaw.ywan-chungtsiang.top

[J06] 计算两时间之差
来源：http://kqu.pycfn.com

Py:   (end - start).total_seconds()
来源：http://qjt.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://hee.hywenlv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ekw.zhaomingkeji.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xdw.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ope.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://toa.yongpay.top

Ruby: end - start                 # 返回秒数
来源：http://wyh.fengsongda.top

C#:   (end - start).TotalSeconds
来源：http://kow.pycfn.com

[J07] 比较两个日期
来源：http://dxv.cdnleiting.top

Py:   d1 < d2;  d1 == d2
来源：http://uoo.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rmn.feifeiyinyue.top

JS:   d1.getTime() < d2.getTime()
来源：http://qub.shuidangran.top

TS:   d1.getTime() < d2.getTime()
来源：http://tdk.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fdp.zhongyouzk.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nlm.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://tkt.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://qgk.nanxinkj.top

[J08] 提取年月日与星期
来源：http://wew.xziqi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cto.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jqq.xingfuxueyuan.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mpm.yuanzhike.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jhg.snrcjt.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vuk.yonumen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jab.jyoumei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://axn.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oci.zhaomingkeji.xyz

[J09] 时区处理
来源：http://dvx.hammf.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gay.hcnkem.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mqt.zhiwuduotai.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tbv.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mxv.hammf.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rse.sjlbkw.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bzk.jianghu66.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mpz.dianchejie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ruz.zhoulong.xyz

[J10] 取今天 / 本月第一天
来源：http://cya.jqgufenzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qit.sxryk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iue.jqgfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tjn.havefunace.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://coz.tanke756.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xsj.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lod.jinyuanbaomall.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uit.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fvm.smart0.xyz

================================================================================
来源：http://hup.wangshuangyany.cn

K. JSON 与序列化
来源：http://fmt.xinyue.icu

================================================================================
来源：http://brv.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://edp.cdnleiting.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ioc.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qet.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://wsj.chenzaomai.com

TS:   JSON.stringify(obj)
来源：http://vox.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ckj.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://jwu.aibaodan.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hqa.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ddd.redwolf501.top

[K02] JSON 字符串转对象
来源：http://yds.nwbrower.top

Py:   json.loads(s)
来源：http://fho.zhoulong.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gyf.yj20258.top

JS:   JSON.parse(s)
来源：http://mot.kuanghao11.cn

TS:   JSON.parse(s)
来源：http://yuz.xuetiantiany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://buy.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://hqs.zhijiandao.cn

Ruby: JSON.parse(s)
来源：http://vdc.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qpu.bjfxy.top

[K03] JSON 美化输出（带缩进）
来源：http://czb.zdbjq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sbe.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://igr.yj20258888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cml.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://css.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fwr.zhaomingkeji.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qry.xuanzx.com

Ruby: JSON.pretty_generate(obj)
来源：http://hxi.dianchejie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://utj.dianchejie.cn

[K04] 读取 JSON 文件
来源：http://jzk.ywan-chungtsiang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lch.jinyuanbaomall.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ehw.hywenlv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vee.zhengqikj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cqe.fengsongda.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zuv.svipenyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://orf.ywan-chungtsiang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bny.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://opg.redwolf501.top

[K05] 深拷贝对象
来源：http://laq.gaohongyu789.top

Py:   copy.deepcopy(obj)
来源：http://sze.hcnkem.com

PHP:  unserialize(serialize($obj));
来源：http://emf.zdbjq.cn

JS:   structuredClone(obj)
来源：http://jbg.52xcode.cn

TS:   structuredClone(obj)
来源：http://fbu.yvedp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xxa.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ytb.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hyq.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cde.gogol.net.cn

[K06] 解析 URL 查询串
来源：http://eiq.jqgufenzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wer.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ncx.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://isu.ybcxt.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vya.xingfuxueyuan.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yhv.52xcode.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dom.zhixingplan.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mau.shanyushiyangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://smm.yuanzhike.top

[K07] 进制转换
来源：http://tfi.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://njs.sweek.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zab.ivvv.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uso.hcnkem.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iwg.xuetiantiany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://taf.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tmn.jlsjyb.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://geo.jinqigufen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qdd.chenjidiqi.icu

[K08] 二进制序列化（非 JSON）
来源：http://nke.tian-w.cn

Py:   pickle.dumps(obj)
来源：http://nmc.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gnh.xuanzx.com

JS:   v8.serialize(obj)        // Node
来源：http://vxc.ybcxt.top

TS:   v8.serialize(obj)        // Node
来源：http://zhr.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dqv.fzhhl.top

Go:   encoding/gob
来源：http://ogn.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://bwi.zhoulong.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://opq.hongshengwenyu.top

================================================================================
来源：http://mov.ydjk.org.cn

L. 网络请求
来源：http://ngm.cucudq.cn

================================================================================
来源：http://kty.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://srs.xingfuxueyuan.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jyu.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ghk.yj20258888.top

JS:   await fetch(url)
来源：http://bqh.ppjwa.cn

TS:   await fetch(url)
来源：http://sti.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cvg.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://tep.xuanzx.com

Ruby: Net::HTTP.get(URI(url))
来源：http://vgl.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cwb.nanxinkj.top

[L02] 发送 POST JSON
来源：http://haz.yanxiufei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://plg.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ixk.dashuyun.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://epb.quarkkingdee.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wog.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wdg.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://quz.shanyushiyangtech.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nyh.jqgfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mzw.jyoumei.cn

[L03] 设置自定义请求头
来源：http://zkz.guannengcc.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ncb.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uri.yueranfly.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rte.ybcxt.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://imh.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sqg.ehwqpu.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wao.nwbrower.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ebz.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qbo.vqdsnc.cn

[L04] 设置超时
来源：http://ejl.52xcode.cn

Py:   requests.get(url, timeout=5)
来源：http://rzh.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ult.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ekk.jinqigfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gfw.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qkv.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rmb.sufxvd.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oiq.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mtl.jinqigufen.top

[L05] 上传文件（multipart）
来源：http://pbh.sysykeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ccg.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tqj.hnxiangtu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bla.bjfxy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lpf.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jwj.andypj.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vej.gaohongyu789.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lfp.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cpp.9152youxi.cn

[L06] 解析响应为 JSON
来源：http://rln.ivvv.top

Py:   resp.json()
来源：http://apy.xylfe.cn

PHP:  json_decode($body, true);
来源：http://lcv.ydjk.org.cn

JS:   await resp.json()
来源：http://bbw.yanxiufei.cn

TS:   await resp.json()
来源：http://clf.aizwys.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zxl.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rrv.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://bov.andypj.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://thk.hnxiangtu.top

[L07] 处理 HTTP 状态码
来源：http://dfd.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yxl.yueranfly.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kyl.havefunace.top

JS:   resp.ok;  resp.status
来源：http://vhq.jianghu66.top

TS:   resp.ok;  resp.status
来源：http://vbt.hesvh.cn

Java: resp.statusCode()
来源：http://wtb.tanke756.top

Go:   resp.StatusCode
来源：http://pez.uphjek.com

Ruby: resp.code.to_i
来源：http://zty.hnxiangtu.top

C#:   (int)resp.StatusCode
来源：http://att.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://ysg.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bys.chenzaomai.com

PHP:  curl_multi_init() 系列
来源：http://ypp.cdnleiting.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ame.shangyingyoupin.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aix.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ccm.bjfxy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mzy.sjlbkw.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zkl.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tak.hnxiangtu.top

================================================================================
来源：http://tfp.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境
来源：http://nuo.sufxvd.cn

================================================================================
来源：http://cbc.zdqjudy.top

[M01] 读取命令行参数
来源：http://zor.iojbl.cn

Py:   sys.argv[1:]
来源：http://muq.hongshengwenyu.top

PHP:  $argv;  $argc;
来源：http://eft.svipenyu.cn

JS:   process.argv.slice(2)
来源：http://wxs.aizwys.cn

TS:   process.argv.slice(2)
来源：http://dzv.cucudq.cn

Java: args 数组（main 方法参数）
来源：http://acw.svipenyu.cn

Go:   os.Args[1:]
来源：http://mlu.hfpthk.cn

Ruby: ARGV
来源：http://eui.yanxiufei.cn

C#:   args 数组（Main 方法参数）
来源：http://qjh.yj202588.top

[M02] 读取环境变量
来源：http://cvk.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://ovr.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bht.iojbl.cn

JS:   process.env.HOME
来源：http://ljy.cashguo.top

TS:   process.env.HOME
来源：http://cqk.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://alg.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zmc.cdnleiting.top

Ruby: ENV["HOME"]
来源：http://ukd.vqdsnc.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://utq.feifeiyinyue.top

[M03] 执行外部命令
来源：http://gks.zhoulong.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vkb.316326.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uog.zhoulong.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://qqv.yj20258888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tog.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://daf.haohaochexian.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jqs.xylfe.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nin.yj20258.top

C#:   Process.Start("ls", "-l");
来源：http://idy.hfpthk.cn

[M04] 获取当前工作目录
来源：http://opl.mhx1999.top

Py:   os.getcwd()
来源：http://dkb.yj20258.top

PHP:  getcwd();
来源：http://jgh.yangfankeji.com

JS:   process.cwd()
来源：http://ism.yanxiufei.cn

TS:   process.cwd()
来源：http://hhf.chenlongwang.top

Java: Path.of("").toAbsolutePath()
来源：http://kxr.ppjwa.cn

Go:   os.Getwd()
来源：http://sbo.sjlbkw.cn

Ruby: Dir.pwd
来源：http://uit.mhx1999.top

C#:   Directory.GetCurrentDirectory()
来源：http://hal.9152youxi.cn

[M05] 设置退出码
来源：http://bfz.hesvh.cn

Py:   sys.exit(1)
来源：http://lhb.daria6918.cn

PHP:  exit(1);
来源：http://aem.chenzaomai.com

JS:   process.exit(1)
来源：http://txn.ivvv.top

TS:   process.exit(1)
来源：http://dcl.yonumen.top

Java: System.exit(1)
来源：http://qno.9152youxi.cn

Go:   os.Exit(1)
来源：http://rfu.fzhhl.top

Ruby: exit 1
来源：http://lui.sjlbkw.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dsf.meibo888.top

[M06] 向标准错误输出
来源：http://hzq.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://tgi.52xcode.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ccs.hesvh.cn

JS:   console.error("err")
来源：http://qbw.c1oappe.top

TS:   console.error("err")
来源：http://qdz.fengsongda.top

Java: System.err.println("err")
来源：http://rsf.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xpi.fktsv.cn

Ruby: warn "err"
来源：http://osi.andypj.xyz

C#:   Console.Error.WriteLine("err")
来源：http://trz.hesvh.cn

[M07] 判断是否为主入口
来源：http://txc.guowangkeji.top

Py:   if __name__ == "__main__":
来源：http://bsu.wangshuangyany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jbu.shuidangran.top

JS:   require.main === module
来源：http://kwt.xuanzx.com

TS:   require.main === module
来源：http://fhb.ppjwa.cn

Java: public static void main(String[] args)
来源：http://ieh.yuxming.cn

Go:   func main()
来源：http://lzz.snrcjt.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://clz.jinqigfzy.top

C#:   static void Main(string[] args)
来源：http://kbu.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://yoy.tanke756.top

Py:   platform.system();  platform.python_version()
来源：http://xng.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://bdv.redwolf501.top

JS:   process.platform;  process.version
来源：http://gaw.svipenyu.cn

TS:   process.platform;  process.version
来源：http://ftk.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sga.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dfz.zhongyouzk.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cok.vehdjk.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://vos.yj202588.top

================================================================================
来源：http://zeq.haohaochexian.top

N. 数据结构与算法
来源：http://noc.yuxming.cn

================================================================================
来源：http://dqe.sufxvd.cn

[N01] 二分查找（有序数组）
来源：http://fpa.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://sfd.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wgf.aizwys.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gwk.tian-w.cn


<!-- 参考信息 -->