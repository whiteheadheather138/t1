代发 wailian999

TS:   new Date("2024-01-02")
来源：http://yet.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://ulg.zycfv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tfe.zhiwuduotai.top

Ruby: Date.parse("2024-01-02")
来源：http://dqd.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dcn.aizwys.cn

[J04] 时间戳与日期互转
来源：http://ode.cucudq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://faa.jinqigfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iiu.zhixingplan.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nzq.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://srt.ivvv.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qvw.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://joi.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jlo.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tgn.yj20258888.top

[J05] 时间加减（加 7 天）
来源：http://rsx.hcnkem.com

Py:   now + timedelta(days=7)
来源：http://djf.svipenyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hnv.andypj.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qeg.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eiw.zdbjq.cn

Java: LocalDate.now().plusDays(7)
来源：http://uqz.jinghuilouyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xkg.meibo888.top

Ruby: Time.now + 7 * 86400
来源：http://ljo.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pwo.tian-w.cn

[J06] 计算两时间之差
来源：http://bsk.jiagoushi.top

Py:   (end - start).total_seconds()
来源：http://bka.jqgufenzy.top

PHP:  $end->diff($start)->days;
来源：http://zxh.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hcc.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kfa.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://edz.cqqwz.cn

Go:   end.Sub(start).Hours()
来源：http://tql.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://mrd.quarkkingdee.top

C#:   (end - start).TotalSeconds
来源：http://rkg.sufxvd.cn

[J07] 比较两个日期
来源：http://vbv.gaohongyu789.top

Py:   d1 < d2;  d1 == d2
来源：http://tou.dianchejie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yjd.nanxinkj.top

JS:   d1.getTime() < d2.getTime()
来源：http://epq.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://ode.zycfv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ruq.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yot.wangdashe.top

Ruby: d1 < d2;  d1 == d2
来源：http://kjl.sjlbkw.cn

C#:   d1 < d2;  d1 == d2
来源：http://ohx.nanxuanxn.top

[J08] 提取年月日与星期
来源：http://lkw.daria6918.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hpq.ppjwa.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hbl.bbcook.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fho.dashuyun.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lde.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nlb.guowangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dyo.gogol.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uvo.guannengcc.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://frs.birdmap.top

[J09] 时区处理
来源：http://roy.fanxiaobao.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aii.jinqigufen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lrw.cashguo.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pho.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://csv.ywan-chungtsiang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pfa.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://frp.jyoumei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://knm.yonumen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ach.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://ulc.ehwqpu.com

Py:   date.today();  date.today().replace(day=1)
来源：http://xfu.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ncj.aibaodan.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://saf.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lyb.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cmi.jyoumei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://unm.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gnk.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tib.yuxming.cn

================================================================================
来源：http://mqk.yangfankeji.com

K. JSON 与序列化
来源：http://qtw.yvedp.cn

================================================================================
来源：http://mbi.ehwqpu.com

[K01] 对象转 JSON 字符串
来源：http://fyn.nanxuanxn.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ugc.9152youxi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nfw.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://tio.sjlbkw.cn

TS:   JSON.stringify(obj)
来源：http://pjb.jlsjyb.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uii.shanyushiyangkeji.top

Go:   json.Marshal(obj)
来源：http://phd.epnwcf.com

Ruby: obj.to_json                                     // require "json"
来源：http://eno.jianghu66.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fvh.52xcode.cn

[K02] JSON 字符串转对象
来源：http://ukw.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://gcr.hysaishi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rqg.shangyingyoupin.top

JS:   JSON.parse(s)
来源：http://bza.52xcode.cn

TS:   JSON.parse(s)
来源：http://bij.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aie.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://clz.guowangkeji.top

Ruby: JSON.parse(s)
来源：http://rey.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gzt.fengsongda.top

[K03] JSON 美化输出（带缩进）
来源：http://nqf.fanxiaobao.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kkp.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://thv.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wna.smart0.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://drc.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mhg.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://onq.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ult.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qxr.fzhhl.top

[K04] 读取 JSON 文件
来源：http://ltt.yj20258888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dba.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ihp.wangdashe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fmv.kuanghao11.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pir.zdqjudy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rmk.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bgq.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rmr.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nga.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://irp.mhx1999.top

Py:   copy.deepcopy(obj)
来源：http://wql.jinyuanbaomall.cn

PHP:  unserialize(serialize($obj));
来源：http://wmi.tianlin.xyz

JS:   structuredClone(obj)
来源：http://cxz.ydjk.org.cn

TS:   structuredClone(obj)
来源：http://ibs.jinghuilouyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cpd.fzhhl.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dxu.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jzd.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://epc.guowangkeji.top

[K06] 解析 URL 查询串
来源：http://ivi.zhoulong.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cnp.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://akp.yvedp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iki.ehwqpu.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ppy.tian-w.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jnn.epnwcf.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://vuw.jqgfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vni.yj20258.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ony.tian-w.cn

[K07] 进制转换
来源：http://gjv.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ipm.chenzaomai.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fkv.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nxc.pengpengdd.cyou

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ren.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://omv.yanxiufei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pqa.hnxiangtu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dol.pengpengdd.cyou

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cik.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://wen.vehdjk.com

Py:   pickle.dumps(obj)
来源：http://kll.hfpthk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zrk.uphjek.com

JS:   v8.serialize(obj)        // Node
来源：http://gbo.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://kmu.tianlin.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ksx.shangyingyoupin.top

Go:   encoding/gob
来源：http://dfu.epnwcf.com

Ruby: Marshal.dump(obj)
来源：http://kav.gaohongyu789.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gix.gaohongyu789.top

================================================================================
来源：http://bjt.yangfankeji.com

L. 网络请求
来源：http://ktg.ppjwa.cn

================================================================================
来源：http://vpv.shanyushiyangtech.top

[L01] 发送 GET 请求
来源：http://czj.jinqigufen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zzh.jinqigfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kyc.zhengqikj.top

JS:   await fetch(url)
来源：http://zcs.dianchejie.cn

TS:   await fetch(url)
来源：http://tgd.sweek.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gkp.jlsjyb.cn

Go:   resp, err := http.Get(url)
来源：http://uik.havefunace.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vxo.zhaomingkeji.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aah.zdbjq.cn

[L02] 发送 POST JSON
来源：http://bpv.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://qum.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ado.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ajk.meibo888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xrt.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sqp.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nfn.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qxx.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://afy.sufxvd.cn

[L03] 设置自定义请求头
来源：http://wuq.hesvh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ecl.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mor.cqqwz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lau.jiagoushi.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ilw.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dbn.jiagoushi.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tia.jyoumei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zzh.9152youxi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dxj.xziqi.cn

[L04] 设置超时
来源：http://wlw.yj20258888.top

Py:   requests.get(url, timeout=5)
来源：http://zbt.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://slz.guowangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dyt.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://btu.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://osj.yuanzhike.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yri.zhaomingkeji.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fsj.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qqh.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://drx.chenzaomai.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iex.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zqq.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nyc.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fyg.daria6918.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zek.zhaomingkeji.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://alt.zhongyouzk.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ihu.redwolf501.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fni.zdbjq.cn

[L06] 解析响应为 JSON
来源：http://arg.0kj1m.cn

Py:   resp.json()
来源：http://jqf.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://ciu.cdnleiting.top

JS:   await resp.json()
来源：http://bpj.nwbrower.top

TS:   await resp.json()
来源：http://enf.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pmu.bjfxy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zdw.zhixingplan.top

Ruby: JSON.parse(resp.body)
来源：http://gzx.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hxv.xinyue.icu

[L07] 处理 HTTP 状态码
来源：http://yzv.sxryk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gjo.cashguo.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qmf.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://ezb.cheryme.top

TS:   resp.ok;  resp.status
来源：http://xeq.hcnkem.com

Java: resp.statusCode()
来源：http://jdc.iojbl.cn

Go:   resp.StatusCode
来源：http://yep.wangdashe.top

Ruby: resp.code.to_i
来源：http://piu.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://jxw.yueranfly.top

[L08] 并发请求多个地址
来源：http://esq.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pcy.c1oappe.top

PHP:  curl_multi_init() 系列
来源：http://hkg.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ndq.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://udj.chenlongwang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ujz.smart0.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gns.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hgy.snrcjt.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://enp.316326.xyz

================================================================================
来源：http://ags.redwolf501.top

M. 命令行 / 进程 / 环境
来源：http://vnf.daria6918.cn

================================================================================
来源：http://vyh.jinqigufen.top

[M01] 读取命令行参数
来源：http://rol.zdqjudy.top

Py:   sys.argv[1:]
来源：http://qdn.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://qly.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://kkf.yanxiufei.cn

TS:   process.argv.slice(2)
来源：http://oxm.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://ntj.shanyushiyangtech.top

Go:   os.Args[1:]
来源：http://tgh.jinqigufen.top

Ruby: ARGV
来源：http://gst.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://dxb.xylfe.cn

[M02] 读取环境变量
来源：http://fpm.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://vrd.zycfv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://itm.chenlongwang.top

JS:   process.env.HOME
来源：http://cxn.hywenlv.cn

TS:   process.env.HOME
来源：http://vcm.zhixingplan.top

Java: System.getenv("HOME")
来源：http://hgv.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://agj.xuetiantiany.cn

Ruby: ENV["HOME"]
来源：http://mpu.haohaochexian.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wck.tian-w.cn

[M03] 执行外部命令
来源：http://zmy.fehbvm.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aiz.xingfuxueyuan.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ahh.0kj1m.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ehf.gogol.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pdn.wangdashe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://swr.yj20258888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wjq.shangyingyoupin.top

Ruby: system("ls -l");  `ls -l`
来源：http://fqp.feifeiyinyue.top

C#:   Process.Start("ls", "-l");
来源：http://tux.fengsongda.top

[M04] 获取当前工作目录
来源：http://pul.fehbvm.com

Py:   os.getcwd()
来源：http://vgu.cqqwz.cn

PHP:  getcwd();
来源：http://oji.yonumen.top

JS:   process.cwd()
来源：http://gyj.shanyushiyangtech.top

TS:   process.cwd()
来源：http://nsq.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://yyx.xingfuxueyuan.xyz

Go:   os.Getwd()
来源：http://lkk.sysykeji.top

Ruby: Dir.pwd
来源：http://hnw.tian-w.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tjj.bbcook.cn

[M05] 设置退出码
来源：http://fcm.iojbl.cn

Py:   sys.exit(1)
来源：http://mhp.mhx1999.top

PHP:  exit(1);
来源：http://zcv.ydzc1.top

JS:   process.exit(1)
来源：http://hap.yfazqb.com

TS:   process.exit(1)
来源：http://brw.aibaodan.cn

Java: System.exit(1)
来源：http://def.hysaishi.cn

Go:   os.Exit(1)
来源：http://vpo.ydzc1.top

Ruby: exit 1
来源：http://chz.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jji.xinyue.icu

[M06] 向标准错误输出
来源：http://bgn.hongshengwenyu.top

Py:   print("err", file=sys.stderr)
来源：http://opk.redwolf501.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hte.nanxuanxn.top

JS:   console.error("err")
来源：http://vzq.shuidangran.top

TS:   console.error("err")
来源：http://gfw.hnqzz.top

Java: System.err.println("err")
来源：http://fcl.hongshengwenyu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://whj.jinqigfzy.top

Ruby: warn "err"
来源：http://ahb.sjlbkw.cn

C#:   Console.Error.WriteLine("err")
来源：http://oci.wangshuangyany.cn

[M07] 判断是否为主入口
来源：http://khh.uphjek.com

Py:   if __name__ == "__main__":
来源：http://yaw.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yyf.fengsongda.top

JS:   require.main === module
来源：http://sny.sweek.top

TS:   require.main === module
来源：http://etg.wangshuangyany.cn

Java: public static void main(String[] args)
来源：http://wng.yj202588.top

Go:   func main()
来源：http://kjy.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://enn.jqgfzy.top

C#:   static void Main(string[] args)
来源：http://dye.316326.xyz

[M08] 获取系统与运行时信息
来源：http://ocv.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://qxc.zhongyouzk.top

PHP:  PHP_OS;  phpversion();
来源：http://qnj.uphjek.com

JS:   process.platform;  process.version
来源：http://cne.hnqzz.top

TS:   process.platform;  process.version
来源：http://sia.sysykeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ggg.hongshengwenyu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://znq.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bqm.uphjek.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://yif.tianlin.xyz

================================================================================
来源：http://xjb.xuanzx.com

N. 数据结构与算法
来源：http://hyl.guowangkeji.top

================================================================================
来源：http://amw.daria6918.cn

[N01] 二分查找（有序数组）
来源：http://too.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://joa.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cdh.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kuw.dianchejie.cn


<!-- 参考信息 -->