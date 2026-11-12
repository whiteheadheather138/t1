代发 wailian999

[J03] 字符串解析为日期
来源：http://rxu.jianghu66.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ruq.hesvh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kdh.nwbrower.top

JS:   new Date("2024-01-02")
来源：http://zxh.hcnkem.com

TS:   new Date("2024-01-02")
来源：http://qap.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://vuq.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bud.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://cgu.jiagoushi.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bof.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://qhl.nanxuanxn.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cxu.birdmap.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tyt.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://clc.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vcg.tarul.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qow.smart0.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jjm.0kj1m.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rgt.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://son.hammf.cn

[J05] 时间加减（加 7 天）
来源：http://hxm.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://wpi.jinghuilouyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nbj.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://loo.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zlw.aibaodan.cn

Java: LocalDate.now().plusDays(7)
来源：http://exb.jinqigfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sgw.yuxming.cn

Ruby: Time.now + 7 * 86400
来源：http://fnx.quarkkingdee.top

C#:   DateTime.Now.AddDays(7)
来源：http://oxe.yuanzhike.top

[J06] 计算两时间之差
来源：http://wie.meibo888.top

Py:   (end - start).total_seconds()
来源：http://ukk.xuetiantiany.cn

PHP:  $end->diff($start)->days;
来源：http://gmw.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kak.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ayq.xingfuxueyuan.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://nkw.redwolf501.top

Go:   end.Sub(start).Hours()
来源：http://bzb.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://kdt.hfpthk.cn

C#:   (end - start).TotalSeconds
来源：http://zcq.haohaochexian.top

[J07] 比较两个日期
来源：http://jzf.zdqjudy.top

Py:   d1 < d2;  d1 == d2
来源：http://wbs.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sft.fengsongda.top

JS:   d1.getTime() < d2.getTime()
来源：http://gll.bjfxy.top

TS:   d1.getTime() < d2.getTime()
来源：http://opk.vqdsnc.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ncd.yj20258.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yfb.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://qdc.hongshengwenyu.top

C#:   d1 < d2;  d1 == d2
来源：http://udp.cdnleiting.top

[J08] 提取年月日与星期
来源：http://yek.fzhhl.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://poz.ivvv.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cdo.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cah.sysykeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fqb.zhijiandao.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sjo.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wly.xingfuxueyuan.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gok.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rpv.shanyushiyangkeji.top

[J09] 时区处理
来源：http://aem.jianghu66.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jtj.tarul.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jkw.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aec.c1oappe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uky.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://krv.jqgfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gyq.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://plk.andypj.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tiv.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://fpu.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xav.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rfn.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pxr.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qef.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cem.ppjwa.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lcm.zhijiandao.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://obg.jianghu66.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bzs.bjfxy.top

================================================================================
来源：http://kxm.hcnkem.com

K. JSON 与序列化
来源：http://nxs.xinyue.icu

================================================================================
来源：http://ygb.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://mcd.yuxming.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mrs.shzxlz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oeu.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://doo.zhoulong.xyz

TS:   JSON.stringify(obj)
来源：http://raf.xuetiantiany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ayu.hammf.cn

Go:   json.Marshal(obj)
来源：http://ivn.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://idy.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://lss.zhoulong.xyz

[K02] JSON 字符串转对象
来源：http://mhx.iojbl.cn

Py:   json.loads(s)
来源：http://qun.ppjwa.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://air.bbcook.cn

JS:   JSON.parse(s)
来源：http://hrn.zhengqikj.top

TS:   JSON.parse(s)
来源：http://thu.tanke756.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zcd.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://ipe.hongshengwenyu.top

Ruby: JSON.parse(s)
来源：http://ayp.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ojx.zhixingplan.top

[K03] JSON 美化输出（带缩进）
来源：http://ooj.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ndo.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zot.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zna.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://jwp.shangyingyoupin.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://evi.vqdsnc.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gzd.birdmap.top

Ruby: JSON.pretty_generate(obj)
来源：http://rmw.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://req.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://esh.hywenlv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://olu.yangfankeji.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tlp.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rta.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nov.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uar.yj20258888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gqp.zhijiandao.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jht.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mhx.0kj1m.cn

[K05] 深拷贝对象
来源：http://bry.snrcjt.cn

Py:   copy.deepcopy(obj)
来源：http://euq.hfpthk.cn

PHP:  unserialize(serialize($obj));
来源：http://zgg.9152youxi.cn

JS:   structuredClone(obj)
来源：http://pyc.pycfn.com

TS:   structuredClone(obj)
来源：http://phv.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://sfi.316326.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pfx.52xcode.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ezl.epnwcf.com

C#:   // 序列化往返，或自定义 Clone
来源：http://jya.cashguo.top

[K06] 解析 URL 查询串
来源：http://nxz.nanxuanxn.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://omb.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://epo.bbcook.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cni.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fgl.tianlin.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gfg.fzhhl.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hhs.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pbd.bbcook.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gqy.chenzaomai.com

[K07] 进制转换
来源：http://gsx.ctjpmb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yxr.cashguo.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qfl.zdqjudy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ebh.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kbr.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hda.zhongyouzk.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fub.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yim.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mmo.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://ewj.ivvv.top

Py:   pickle.dumps(obj)
来源：http://vcn.c1oappe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ysg.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://xxm.ydzc1.top

TS:   v8.serialize(obj)        // Node
来源：http://xsx.zdqjudy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mee.zhengqikj.top

Go:   encoding/gob
来源：http://vif.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://qeu.9152youxi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fbq.feifeiyinyue.top

================================================================================
来源：http://ycf.daria6918.cn

L. 网络请求
来源：http://mol.hesvh.cn

================================================================================
来源：http://aoh.chenlongwang.top

[L01] 发送 GET 请求
来源：http://uon.gogol.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lml.ppjwa.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kfh.fehbvm.com

JS:   await fetch(url)
来源：http://rlz.hongshengwenyu.top

TS:   await fetch(url)
来源：http://tro.9152youxi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vkr.0kj1m.cn

Go:   resp, err := http.Get(url)
来源：http://xgf.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kvt.sufxvd.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pxs.daria6918.cn

[L02] 发送 POST JSON
来源：http://qlh.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wuf.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aja.xziqi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://amh.mhx1999.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://awd.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nzt.mhx1999.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xxq.dianchejie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xfx.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tdo.yangfankeji.com

[L03] 设置自定义请求头
来源：http://llt.fzhhl.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yca.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://puq.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jyt.ywan-chungtsiang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://irl.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jxk.uphjek.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://avd.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ewt.mhx1999.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oet.chenjidiqi.icu

[L04] 设置超时
来源：http://uar.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://ybt.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://srt.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mtp.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lvk.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://amw.jyoumei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://plg.shangyingyoupin.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ntj.tian-w.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lgv.svipenyu.cn

[L05] 上传文件（multipart）
来源：http://mxh.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gvz.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ikj.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gbe.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jqx.hongshengwenyu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wow.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yri.shzxlz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ehu.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eyc.nanxuanxn.top

[L06] 解析响应为 JSON
来源：http://wso.zdqjudy.top

Py:   resp.json()
来源：http://hic.hfpthk.cn

PHP:  json_decode($body, true);
来源：http://ikx.zdbjq.cn

JS:   await resp.json()
来源：http://wqf.gogol.net.cn

TS:   await resp.json()
来源：http://hon.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vlz.quarkkingdee.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mni.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://nzu.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pol.hcnkem.com

[L07] 处理 HTTP 状态码
来源：http://xrk.redwolf501.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hei.ydjk.org.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xyx.chenlongwang.top

JS:   resp.ok;  resp.status
来源：http://dej.yongpay.top

TS:   resp.ok;  resp.status
来源：http://wsl.jqgfzy.top

Java: resp.statusCode()
来源：http://osx.ydzc1.top

Go:   resp.StatusCode
来源：http://cka.hesvh.cn

Ruby: resp.code.to_i
来源：http://wrp.birdmap.top

C#:   (int)resp.StatusCode
来源：http://bxg.chenjidiqi.icu

[L08] 并发请求多个地址
来源：http://gdx.aizwys.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hhi.xingfuxueyuan.xyz

PHP:  curl_multi_init() 系列
来源：http://grr.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tti.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://muu.gotoacloud.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://czw.xziqi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hop.guowangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dpe.bbcook.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zwb.c1oappe.top

================================================================================
来源：http://dwy.gogol.net.cn

M. 命令行 / 进程 / 环境
来源：http://hcc.316326.xyz

================================================================================
来源：http://ywn.316326.xyz

[M01] 读取命令行参数
来源：http://ngs.yj20258.top

Py:   sys.argv[1:]
来源：http://als.jyoumei.cn

PHP:  $argv;  $argc;
来源：http://dfn.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://qho.epnwcf.com

TS:   process.argv.slice(2)
来源：http://wbv.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://yrz.birdmap.top

Go:   os.Args[1:]
来源：http://uhu.zhaomingkeji.xyz

Ruby: ARGV
来源：http://vzc.sxryk.cn

C#:   args 数组（Main 方法参数）
来源：http://gix.jiagoushi.top

[M02] 读取环境变量
来源：http://qsh.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://jab.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oyn.hcnkem.com

JS:   process.env.HOME
来源：http://pmt.hfpthk.cn

TS:   process.env.HOME
来源：http://fxx.mhx1999.top

Java: System.getenv("HOME")
来源：http://wfq.vehdjk.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ewa.smart0.xyz

Ruby: ENV["HOME"]
来源：http://rki.zhaomingkeji.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://asj.yanxiufei.cn

[M03] 执行外部命令
来源：http://bep.fktsv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sda.feifeiyinyue.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://imd.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ose.xuetiantiany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xfa.fengsongda.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xpm.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://agm.haohaochexian.top

Ruby: system("ls -l");  `ls -l`
来源：http://mzr.shanyushiyangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://wli.c1oappe.top

[M04] 获取当前工作目录
来源：http://cfj.jqgufenzy.top

Py:   os.getcwd()
来源：http://byi.ivvv.top

PHP:  getcwd();
来源：http://dss.quarkkingdee.top

JS:   process.cwd()
来源：http://rkl.fanxiaobao.xyz

TS:   process.cwd()
来源：http://sms.chenzaomai.com

Java: Path.of("").toAbsolutePath()
来源：http://hdc.ybcxt.top

Go:   os.Getwd()
来源：http://dip.cucudq.cn

Ruby: Dir.pwd
来源：http://ubd.gotoacloud.top

C#:   Directory.GetCurrentDirectory()
来源：http://rkr.ctjpmb.com

[M05] 设置退出码
来源：http://toi.nanxinkj.top

Py:   sys.exit(1)
来源：http://raj.yj20258.top

PHP:  exit(1);
来源：http://wae.smart0.xyz

JS:   process.exit(1)
来源：http://rqn.zhoulong.xyz

TS:   process.exit(1)
来源：http://odj.fzhhl.top

Java: System.exit(1)
来源：http://blx.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://wik.nanxuanxn.top

Ruby: exit 1
来源：http://uuy.tarul.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vuy.dashuyun.cn

[M06] 向标准错误输出
来源：http://ppi.chenzaomai.com

Py:   print("err", file=sys.stderr)
来源：http://cbm.chenzaomai.com

PHP:  fwrite(STDERR, "err\n");
来源：http://acm.iojbl.cn

JS:   console.error("err")
来源：http://rsy.sysykeji.top

TS:   console.error("err")
来源：http://vcf.gogol.net.cn

Java: System.err.println("err")
来源：http://wfw.shangyingyoupin.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pgz.ctjpmb.com

Ruby: warn "err"
来源：http://acp.zhiwuduotai.top

C#:   Console.Error.WriteLine("err")
来源：http://ktp.smart0.xyz

[M07] 判断是否为主入口
来源：http://ata.jqgfzy.top

Py:   if __name__ == "__main__":
来源：http://gcy.shangyingyoupin.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zaa.xinyue.icu

JS:   require.main === module
来源：http://tef.9152youxi.cn

TS:   require.main === module
来源：http://mcg.shangyingyoupin.top

Java: public static void main(String[] args)
来源：http://qek.yfazqb.com

Go:   func main()
来源：http://qfq.meibo888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wzt.yvedp.cn

C#:   static void Main(string[] args)
来源：http://yxt.tian-w.cn

[M08] 获取系统与运行时信息
来源：http://mln.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://dnb.hfpthk.cn

PHP:  PHP_OS;  phpversion();
来源：http://qdc.guowangkeji.top

JS:   process.platform;  process.version
来源：http://aao.nanxuanxn.top

TS:   process.platform;  process.version
来源：http://sko.jqgufenzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://buq.sysykeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jhc.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ftp.bjfxy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tvz.ehwqpu.com

================================================================================
来源：http://xgj.birdmap.top

N. 数据结构与算法
来源：http://crs.hammf.cn

================================================================================
来源：http://pxd.jinghuilouyu.cn


<!-- 参考信息 -->