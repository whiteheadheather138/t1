代发 wailian999

TS:   new Date("2024-01-02")
来源：http://cpd.zdqjudy.top

Java: LocalDate.parse("2024-01-02")
来源：http://ryv.yvedp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://org.quarkkingdee.top

Ruby: Date.parse("2024-01-02")
来源：http://ram.hesvh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://knz.zhixingplan.top

[J04] 时间戳与日期互转
来源：http://sks.guannengcc.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bvy.sysykeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iqd.chenjidiqi.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rcb.aibaodan.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qdv.zhixingplan.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vcj.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://odf.xuetiantiany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tyn.zdbjq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gho.zhongyouzk.top

[J05] 时间加减（加 7 天）
来源：http://ukk.xinyue.icu

Py:   now + timedelta(days=7)
来源：http://rdw.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://flm.xinyue.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rgp.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ywa.mhx1999.top

Java: LocalDate.now().plusDays(7)
来源：http://dre.bbcook.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://svc.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://egh.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://orb.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://mgh.gzhubu.top

Py:   (end - start).total_seconds()
来源：http://tbn.yuanzhike.top

PHP:  $end->diff($start)->days;
来源：http://zly.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sar.hfpthk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mty.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://vvd.nanxuanxn.top

Go:   end.Sub(start).Hours()
来源：http://rxm.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://yck.haohaochexian.top

C#:   (end - start).TotalSeconds
来源：http://ezy.ctjpmb.com

[J07] 比较两个日期
来源：http://etr.yj202588.top

Py:   d1 < d2;  d1 == d2
来源：http://nsz.ywan-chungtsiang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://phd.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://oze.hnqzz.top

TS:   d1.getTime() < d2.getTime()
来源：http://hki.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ndx.yangfankeji.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://drz.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nld.yfazqb.com

C#:   d1 < d2;  d1 == d2
来源：http://gjz.zycfv.cn

[J08] 提取年月日与星期
来源：http://plk.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bls.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fpn.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nxt.cheryme.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bnk.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lhe.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rtw.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cxf.hnqzz.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ief.zhixingplan.top

[J09] 时区处理
来源：http://uvo.guowangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wdt.pycfn.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hqg.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zwv.shuidangran.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kbb.yueranfly.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hji.jqgufenzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mgs.xylfe.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://loe.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://euv.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://omy.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://joq.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bfd.xziqi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kmn.chenlongwang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ork.nanxinkj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iwk.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wjr.jianghu66.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://foo.zhixingplan.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qnf.chenlongwang.top

================================================================================
来源：http://ikv.shuidangran.top

K. JSON 与序列化
来源：http://ncb.ywan-chungtsiang.top

================================================================================
来源：http://kzq.zdqjudy.top

[K01] 对象转 JSON 字符串
来源：http://ozc.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hvi.fktsv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gng.shzxlz.cn

JS:   JSON.stringify(obj)
来源：http://czp.mhx1999.top

TS:   JSON.stringify(obj)
来源：http://baf.jinqigfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ivj.iojbl.cn

Go:   json.Marshal(obj)
来源：http://ogj.gotoacloud.top

Ruby: obj.to_json                                     // require "json"
来源：http://whx.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vbk.yonumen.top

[K02] JSON 字符串转对象
来源：http://iyl.guowangkeji.top

Py:   json.loads(s)
来源：http://lex.shangyingyoupin.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://drv.tarul.cn

JS:   JSON.parse(s)
来源：http://dyt.yfazqb.com

TS:   JSON.parse(s)
来源：http://exv.bjfxy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://spt.jinghuilouyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://qjg.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://pfl.yonumen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vez.yj202588.top

[K03] JSON 美化输出（带缩进）
来源：http://bqh.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oei.yj20258888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lvi.aibaodan.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pyg.jlsjyb.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ywv.c1oappe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vjw.jinghuilouyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pcx.hfpthk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bky.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://inm.zdbjq.cn

[K04] 读取 JSON 文件
来源：http://kqf.ivvv.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ffn.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yyo.shanyushiyangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yga.xingfuxueyuan.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://znv.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ktp.hnqzz.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://znl.yj202588.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jcu.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ywp.yonumen.top

[K05] 深拷贝对象
来源：http://cvr.chenjidiqi.icu

Py:   copy.deepcopy(obj)
来源：http://ltj.sweek.top

PHP:  unserialize(serialize($obj));
来源：http://ttk.xuanzx.com

JS:   structuredClone(obj)
来源：http://czd.sxryk.cn

TS:   structuredClone(obj)
来源：http://lrc.daxiang520.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ntk.ydzc1.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cdq.epnwcf.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rco.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vym.shuidangran.top

[K06] 解析 URL 查询串
来源：http://nae.cashguo.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hqh.xziqi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zfl.zhixingplan.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xuz.zhijiandao.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://trm.yj202588.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bnx.hesvh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ver.zdqjudy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ihg.cdnleiting.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fvy.zycfv.cn

[K07] 进制转换
来源：http://kut.zhixingplan.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dlq.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://obh.hywenlv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xbe.bjfxy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uon.aizwys.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cfi.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dyi.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jhi.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mkd.shanyushiyangtech.top

[K08] 二进制序列化（非 JSON）
来源：http://uvw.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://wpd.yj20258888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jie.jinyuanbaomall.cn

JS:   v8.serialize(obj)        // Node
来源：http://cak.jqgufenzy.top

TS:   v8.serialize(obj)        // Node
来源：http://oyc.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ood.yj20258888.top

Go:   encoding/gob
来源：http://cdl.jinqigfzy.top

Ruby: Marshal.dump(obj)
来源：http://mgl.daria6918.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xyf.shangyingyoupin.top

================================================================================
来源：http://nzx.yangfankeji.com

L. 网络请求
来源：http://iwd.jiagoushi.top

================================================================================
来源：http://mjk.smart0.xyz

[L01] 发送 GET 请求
来源：http://tuc.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dsn.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uvi.bbcook.cn

JS:   await fetch(url)
来源：http://off.zdqjudy.top

TS:   await fetch(url)
来源：http://yxv.jqgufenzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kmm.fengsongda.top

Go:   resp, err := http.Get(url)
来源：http://mub.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://elq.ehwqpu.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wfc.dianchejie.cn

[L02] 发送 POST JSON
来源：http://tug.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xwk.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://avv.shzxlz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yvd.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kax.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qus.yfazqb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rzg.daxiang520.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uze.pengpengdd.cyou

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rtb.hcnkem.com

[L03] 设置自定义请求头
来源：http://rlu.ywan-chungtsiang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ram.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tjd.shuidangran.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sve.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wci.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wqm.aibaodan.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pav.fzhhl.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ylc.hcnkem.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://deg.pengpengdd.cyou

[L04] 设置超时
来源：http://tku.birdmap.top

Py:   requests.get(url, timeout=5)
来源：http://zyf.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gbb.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xeq.gogol.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://plw.quarkkingdee.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xwk.kuanghao11.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yfq.hongshengwenyu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pvt.daria6918.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://piu.yongpay.top

[L05] 上传文件（multipart）
来源：http://jsc.dianchejie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lck.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://agp.uphjek.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iku.yuanzhike.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cfc.9152youxi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nam.yfazqb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hae.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://phy.ydjk.org.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bjf.hfpthk.cn

[L06] 解析响应为 JSON
来源：http://umq.quarkkingdee.top

Py:   resp.json()
来源：http://flw.tarul.cn

PHP:  json_decode($body, true);
来源：http://cwr.sxryk.cn

JS:   await resp.json()
来源：http://mak.fktsv.cn

TS:   await resp.json()
来源：http://eub.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://euc.tian-w.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cjd.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://tif.jinqigfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ghy.fktsv.cn

[L07] 处理 HTTP 状态码
来源：http://jek.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://njm.svipenyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ebn.hfpthk.cn

JS:   resp.ok;  resp.status
来源：http://oim.xylfe.cn

TS:   resp.ok;  resp.status
来源：http://raa.shzxlz.cn

Java: resp.statusCode()
来源：http://jss.tianlin.xyz

Go:   resp.StatusCode
来源：http://cba.jianghu66.top

Ruby: resp.code.to_i
来源：http://gkk.jinqigufen.top

C#:   (int)resp.StatusCode
来源：http://mom.0kj1m.cn

[L08] 并发请求多个地址
来源：http://xxy.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wln.daxiang520.top

PHP:  curl_multi_init() 系列
来源：http://naj.yanxiufei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hlh.fzhhl.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sdm.shzxlz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pdn.yanxiufei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://foh.yj20258888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uym.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nib.vqdsnc.cn

================================================================================
来源：http://pkb.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://lfv.zhongyouzk.top

================================================================================
来源：http://vdq.gzhubu.top

[M01] 读取命令行参数
来源：http://fns.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://whr.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://laf.xuetiantiany.cn

JS:   process.argv.slice(2)
来源：http://ucq.andypj.xyz

TS:   process.argv.slice(2)
来源：http://ven.316326.xyz

Java: args 数组（main 方法参数）
来源：http://ofr.guowangkeji.top

Go:   os.Args[1:]
来源：http://ulo.fengsongda.top

Ruby: ARGV
来源：http://pzq.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://inf.hywenlv.cn

[M02] 读取环境变量
来源：http://srk.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://wih.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://obf.smart0.xyz

JS:   process.env.HOME
来源：http://qvz.guannengcc.top

TS:   process.env.HOME
来源：http://pmd.epnwcf.com

Java: System.getenv("HOME")
来源：http://mps.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uxt.ydzc1.top

Ruby: ENV["HOME"]
来源：http://smf.sufxvd.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pcf.jinqigufen.top

[M03] 执行外部命令
来源：http://klj.tian-w.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ejq.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ldd.ctjpmb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://rhp.aibaodan.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oet.wangdashe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mym.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rwl.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://hud.hfpthk.cn

C#:   Process.Start("ls", "-l");
来源：http://gns.jiagoushi.top

[M04] 获取当前工作目录
来源：http://caj.chenlongwang.top

Py:   os.getcwd()
来源：http://sti.dashuyun.cn

PHP:  getcwd();
来源：http://gxa.mhx1999.top

JS:   process.cwd()
来源：http://aee.shuidangran.top

TS:   process.cwd()
来源：http://kbw.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://lyw.smart0.xyz

Go:   os.Getwd()
来源：http://tdo.cqqwz.cn

Ruby: Dir.pwd
来源：http://vvw.sysykeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://wkp.gotoacloud.top

[M05] 设置退出码
来源：http://rcn.c1oappe.top

Py:   sys.exit(1)
来源：http://tyy.hesvh.cn

PHP:  exit(1);
来源：http://iba.gogol.net.cn

JS:   process.exit(1)
来源：http://naq.zycfv.cn

TS:   process.exit(1)
来源：http://wtt.c1oappe.top

Java: System.exit(1)
来源：http://cdw.xuanzx.com

Go:   os.Exit(1)
来源：http://yuv.fengsongda.top

Ruby: exit 1
来源：http://npq.cdnleiting.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bvf.yfazqb.com

[M06] 向标准错误输出
来源：http://ojf.redwolf501.top

Py:   print("err", file=sys.stderr)
来源：http://rhm.jinyuanbaomall.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vkw.jqgfzy.top

JS:   console.error("err")
来源：http://lea.316326.xyz

TS:   console.error("err")
来源：http://bhx.aibaodan.cn

Java: System.err.println("err")
来源：http://knr.fehbvm.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wrx.hongshengwenyu.top

Ruby: warn "err"
来源：http://pjz.haohaochexian.top

C#:   Console.Error.WriteLine("err")
来源：http://haf.c1oappe.top

[M07] 判断是否为主入口
来源：http://jrh.ehwqpu.com

Py:   if __name__ == "__main__":
来源：http://mkg.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rry.yongpay.top

JS:   require.main === module
来源：http://yzk.quarkkingdee.top

TS:   require.main === module
来源：http://nbg.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://nsr.kuanghao11.cn

Go:   func main()
来源：http://xto.hnqzz.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jul.yueranfly.top

C#:   static void Main(string[] args)
来源：http://uhb.jinqigfzy.top

[M08] 获取系统与运行时信息
来源：http://zqx.yanxiufei.cn

Py:   platform.system();  platform.python_version()
来源：http://cyi.ybcxt.top

PHP:  PHP_OS;  phpversion();
来源：http://ipx.gaohongyu789.top

JS:   process.platform;  process.version
来源：http://puh.xziqi.cn

TS:   process.platform;  process.version
来源：http://tyf.redwolf501.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ccn.yangfankeji.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://fru.yj20258888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zyk.xuetiantiany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fqq.daria6918.cn

================================================================================
来源：http://igs.chenzaomai.com

N. 数据结构与算法
来源：http://pjf.xuanzx.com

================================================================================
来源：http://gwb.jianghu66.top

[N01] 二分查找（有序数组）
来源：http://ral.yueranfly.top

Py:   bisect.bisect_left(arr, x)
来源：http://onj.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zfn.tarul.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pdf.vehdjk.com


<!-- 参考信息 -->