代发 wailian999

TS:   new Date("2024-01-02")
来源：http://eib.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://fkh.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qun.aibaodan.cn

Ruby: Date.parse("2024-01-02")
来源：http://vyf.zycfv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cpg.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://kjl.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wmt.sufxvd.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zux.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tbp.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bvo.xuanzx.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wxw.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jei.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hce.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qxy.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://iwd.feifeiyinyue.top

Py:   now + timedelta(days=7)
来源：http://olp.bjfxy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://oba.fengsongda.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://npy.guowangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yly.jqgufenzy.top

Java: LocalDate.now().plusDays(7)
来源：http://hob.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mvv.hysaishi.cn

Ruby: Time.now + 7 * 86400
来源：http://vkx.zhixingplan.top

C#:   DateTime.Now.AddDays(7)
来源：http://lag.meibo888.top

[J06] 计算两时间之差
来源：http://wkv.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://rcc.xylfe.cn

PHP:  $end->diff($start)->days;
来源：http://jzj.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://diq.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nur.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dac.daria6918.cn

Go:   end.Sub(start).Hours()
来源：http://lyf.tanke756.top

Ruby: end - start                 # 返回秒数
来源：http://pwb.shanyushiyangtech.top

C#:   (end - start).TotalSeconds
来源：http://tgw.sxryk.cn

[J07] 比较两个日期
来源：http://bwt.dianchejie.cn

Py:   d1 < d2;  d1 == d2
来源：http://kuv.iojbl.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vxc.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://joy.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://rii.xuetiantiany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xzh.cheryme.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://osg.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://mbm.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://wre.jqgfzy.top

[J08] 提取年月日与星期
来源：http://jww.havefunace.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eay.jinqigufen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nfi.xziqi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sir.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://buw.cucudq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hkm.gogol.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ylz.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ncy.jqgfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wfh.zhijiandao.cn

[J09] 时区处理
来源：http://dax.havefunace.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uck.hnxiangtu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bfl.zdbjq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xgu.quarkkingdee.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bcj.guannengcc.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xie.shuidangran.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fse.xziqi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gyd.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aiu.tanke756.top

[J10] 取今天 / 本月第一天
来源：http://zek.jlsjyb.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hlg.pycfn.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rnf.fengsongda.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pjk.wangdashe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://euk.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hhk.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kmp.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wjf.pycfn.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xqe.jinghuilouyu.cn

================================================================================
来源：http://qpe.zhongyouzk.top

K. JSON 与序列化
来源：http://cbv.jlsjyb.cn

================================================================================
来源：http://mdm.zhaomingkeji.xyz

[K01] 对象转 JSON 字符串
来源：http://aon.feifeiyinyue.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bsf.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lcg.0kj1m.cn

JS:   JSON.stringify(obj)
来源：http://qew.aizwys.cn

TS:   JSON.stringify(obj)
来源：http://wcn.zhixingplan.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nia.guannengcc.top

Go:   json.Marshal(obj)
来源：http://kqu.guowangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://knq.xylfe.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dsh.fktsv.cn

[K02] JSON 字符串转对象
来源：http://zoj.jinyuanbaomall.cn

Py:   json.loads(s)
来源：http://qxz.chenjidiqi.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hah.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://fnq.jqgfzy.top

TS:   JSON.parse(s)
来源：http://yrk.fanxiaobao.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qxl.cqqwz.cn

Go:   json.Unmarshal(data, &v)
来源：http://lln.hnqzz.top

Ruby: JSON.parse(s)
来源：http://rbd.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xek.nwbrower.top

[K03] JSON 美化输出（带缩进）
来源：http://oav.cashguo.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ttp.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ejm.shanyushiyangtech.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uuk.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mky.shzxlz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hmf.kuanghao11.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tii.yj202588.top

Ruby: JSON.pretty_generate(obj)
来源：http://kai.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ppr.sysykeji.top

[K04] 读取 JSON 文件
来源：http://qrl.hywenlv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ker.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://utk.xylfe.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mcr.zdqjudy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hpr.zdqjudy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qvq.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://msk.hnqzz.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://opm.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://udi.chenjidiqi.icu

[K05] 深拷贝对象
来源：http://bsr.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://wwi.9152youxi.cn

PHP:  unserialize(serialize($obj));
来源：http://jwn.zhijiandao.cn

JS:   structuredClone(obj)
来源：http://nzm.zhixingplan.top

TS:   structuredClone(obj)
来源：http://zmm.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kag.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sxo.yonumen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mbl.52xcode.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ykn.cqqwz.cn

[K06] 解析 URL 查询串
来源：http://due.gogol.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hnu.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dor.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qev.fehbvm.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://abm.fzhhl.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hrl.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bhu.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://thl.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sab.9152youxi.cn

[K07] 进制转换
来源：http://dha.ybcxt.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dni.andypj.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aei.jinqigfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bks.yj20258888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bxc.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bbj.xinyue.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pau.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bcc.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lmi.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://fkx.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://leg.wangshuangyany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://odi.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://jnd.andypj.xyz

TS:   v8.serialize(obj)        // Node
来源：http://hya.hfpthk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://smf.yuanzhike.top

Go:   encoding/gob
来源：http://mgv.gaohongyu789.top

Ruby: Marshal.dump(obj)
来源：http://ijo.yuanzhike.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ist.yongpay.top

================================================================================
来源：http://xax.chenlongwang.top

L. 网络请求
来源：http://vni.ydzc1.top

================================================================================
来源：http://nxd.yfazqb.com

[L01] 发送 GET 请求
来源：http://qta.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qiq.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pbb.shangyingyoupin.top

JS:   await fetch(url)
来源：http://txr.shanyushiyangtech.top

TS:   await fetch(url)
来源：http://zdt.havefunace.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vcp.chenlongwang.top

Go:   resp, err := http.Get(url)
来源：http://cso.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jkd.hfpthk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://amw.fehbvm.com

[L02] 发送 POST JSON
来源：http://itm.cheryme.top

Py:   requests.post(url, json={"a": 1})
来源：http://bkl.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rjw.hywenlv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hhy.feifeiyinyue.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cal.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dzc.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ugt.yangfankeji.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xhy.shuidangran.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://euw.hnqzz.top

[L03] 设置自定义请求头
来源：http://kis.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aoz.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://azj.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oub.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://coz.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mha.shangyingyoupin.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zuy.9152youxi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mjo.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vpo.quarkkingdee.top

[L04] 设置超时
来源：http://nmf.iojbl.cn

Py:   requests.get(url, timeout=5)
来源：http://kic.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yhm.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://skc.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wip.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ulj.hammf.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ilv.chenlongwang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://amq.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xsj.cqqwz.cn

[L05] 上传文件（multipart）
来源：http://zyr.zhengqikj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blq.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://apc.wangdashe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dxg.zhaomingkeji.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kvx.pengpengdd.cyou

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qky.yj202588.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cdw.0kj1m.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://njb.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fcx.daria6918.cn

[L06] 解析响应为 JSON
来源：http://eho.jqgfzy.top

Py:   resp.json()
来源：http://nhh.shanyushiyangkeji.top

PHP:  json_decode($body, true);
来源：http://jmo.epnwcf.com

JS:   await resp.json()
来源：http://zhf.chenjidiqi.icu

TS:   await resp.json()
来源：http://zrg.sxryk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ges.xingfuxueyuan.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zzc.ehwqpu.com

Ruby: JSON.parse(resp.body)
来源：http://buy.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fmx.xylfe.cn

[L07] 处理 HTTP 状态码
来源：http://qub.quarkkingdee.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qnk.0kj1m.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lbw.xuetiantiany.cn

JS:   resp.ok;  resp.status
来源：http://evz.cucudq.cn

TS:   resp.ok;  resp.status
来源：http://xqs.iojbl.cn

Java: resp.statusCode()
来源：http://kvm.yuanzhike.top

Go:   resp.StatusCode
来源：http://prx.cucudq.cn

Ruby: resp.code.to_i
来源：http://iev.sysykeji.top

C#:   (int)resp.StatusCode
来源：http://deh.xziqi.cn

[L08] 并发请求多个地址
来源：http://snj.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qor.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://caz.hnqzz.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dxw.snrcjt.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yev.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://isq.meibo888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yqy.sjlbkw.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zgt.pengpengdd.cyou

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://exa.ywan-chungtsiang.top

================================================================================
来源：http://wqq.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://jxk.yanxiufei.cn

================================================================================
来源：http://wne.fehbvm.com

[M01] 读取命令行参数
来源：http://lhq.jlsjyb.cn

Py:   sys.argv[1:]
来源：http://ybn.shangyingyoupin.top

PHP:  $argv;  $argc;
来源：http://soc.sufxvd.cn

JS:   process.argv.slice(2)
来源：http://dqk.316326.xyz

TS:   process.argv.slice(2)
来源：http://cpp.chenjidiqi.icu

Java: args 数组（main 方法参数）
来源：http://xwd.daxiang520.top

Go:   os.Args[1:]
来源：http://gal.chenjidiqi.icu

Ruby: ARGV
来源：http://eov.hywenlv.cn

C#:   args 数组（Main 方法参数）
来源：http://wvd.gzhubu.top

[M02] 读取环境变量
来源：http://lxg.ivvv.top

Py:   os.environ.get("HOME")
来源：http://tqv.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hgl.zhixingplan.top

JS:   process.env.HOME
来源：http://mnc.jianghu66.top

TS:   process.env.HOME
来源：http://plf.gotoacloud.top

Java: System.getenv("HOME")
来源：http://nru.aizwys.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ybk.jlsjyb.cn

Ruby: ENV["HOME"]
来源：http://qad.ybcxt.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://low.316326.xyz

[M03] 执行外部命令
来源：http://fnb.nanxuanxn.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nhm.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ivq.tanke756.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tcu.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://fdh.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eul.sjlbkw.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://acb.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ozj.nanxinkj.top

C#:   Process.Start("ls", "-l");
来源：http://ioq.daria6918.cn

[M04] 获取当前工作目录
来源：http://xlr.cdnleiting.top

Py:   os.getcwd()
来源：http://lpr.sxryk.cn

PHP:  getcwd();
来源：http://aoc.ydjk.org.cn

JS:   process.cwd()
来源：http://eae.birdmap.top

TS:   process.cwd()
来源：http://ehc.uphjek.com

Java: Path.of("").toAbsolutePath()
来源：http://wib.yj20258888.top

Go:   os.Getwd()
来源：http://ggw.fengsongda.top

Ruby: Dir.pwd
来源：http://vfp.jinqigufen.top

C#:   Directory.GetCurrentDirectory()
来源：http://col.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://maq.jinghuilouyu.cn

Py:   sys.exit(1)
来源：http://qlf.shanyushiyangkeji.top

PHP:  exit(1);
来源：http://yml.sjlbkw.cn

JS:   process.exit(1)
来源：http://brj.hysaishi.cn

TS:   process.exit(1)
来源：http://pod.pengpengdd.cyou

Java: System.exit(1)
来源：http://qcx.dianchejie.cn

Go:   os.Exit(1)
来源：http://nlb.shzxlz.cn

Ruby: exit 1
来源：http://cmy.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xdv.xuetiantiany.cn

[M06] 向标准错误输出
来源：http://kce.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://yvv.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wne.shuidangran.top

JS:   console.error("err")
来源：http://ndd.shuidangran.top

TS:   console.error("err")
来源：http://ctl.yanxiufei.cn

Java: System.err.println("err")
来源：http://hsq.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dij.zycfv.cn

Ruby: warn "err"
来源：http://vle.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://qkd.yanxiufei.cn

[M07] 判断是否为主入口
来源：http://vnr.andypj.xyz

Py:   if __name__ == "__main__":
来源：http://ilj.xylfe.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nla.yonumen.top

JS:   require.main === module
来源：http://znv.jinqigufen.top

TS:   require.main === module
来源：http://rjx.yfazqb.com

Java: public static void main(String[] args)
来源：http://uld.chenlongwang.top

Go:   func main()
来源：http://txe.zhixingplan.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cwz.sjlbkw.cn

C#:   static void Main(string[] args)
来源：http://ewh.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://eyd.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://jlo.316326.xyz

PHP:  PHP_OS;  phpversion();
来源：http://dhq.yfazqb.com

JS:   process.platform;  process.version
来源：http://wnl.zhijiandao.cn

TS:   process.platform;  process.version
来源：http://osp.zhiwuduotai.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fbt.yj20258888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://biw.redwolf501.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://osg.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://zug.xinyue.icu

================================================================================
来源：http://qxp.aizwys.cn

N. 数据结构与算法
来源：http://tel.quarkkingdee.top

================================================================================
来源：http://ltb.vehdjk.com

[N01] 二分查找（有序数组）
来源：http://dav.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://qjz.gogol.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wed.jyoumei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oue.aizwys.cn


<!-- 参考信息 -->