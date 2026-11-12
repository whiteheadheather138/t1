代发 wailian999

[J03] 字符串解析为日期
来源：http://nvx.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qgx.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cjs.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://bmg.aizwys.cn

TS:   new Date("2024-01-02")
来源：http://afg.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://jkz.aizwys.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ocg.chenzaomai.com

Ruby: Date.parse("2024-01-02")
来源：http://tao.cqqwz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tlm.smart0.xyz

[J04] 时间戳与日期互转
来源：http://fyb.tianlin.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dpa.jlsjyb.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rkj.hongshengwenyu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://twz.ybcxt.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qxo.9152youxi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ndj.zdqjudy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://elb.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ttl.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iqa.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://hcy.shanyushiyangtech.top

Py:   now + timedelta(days=7)
来源：http://egg.nanxuanxn.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qqp.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ypu.smart0.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://syq.jinghuilouyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://spe.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ycc.andypj.xyz

Ruby: Time.now + 7 * 86400
来源：http://fkm.52xcode.cn

C#:   DateTime.Now.AddDays(7)
来源：http://exv.kuanghao11.cn

[J06] 计算两时间之差
来源：http://urt.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://xzi.zycfv.cn

PHP:  $end->diff($start)->days;
来源：http://sqt.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ycx.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wjp.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://dfl.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://tcc.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://pbx.hongshengwenyu.top

C#:   (end - start).TotalSeconds
来源：http://kip.chenjidiqi.icu

[J07] 比较两个日期
来源：http://lla.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://jdy.feifeiyinyue.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pve.shanyushiyangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://nop.yanxiufei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gfc.yuanzhike.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zkr.jinqigufen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://log.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://tis.ehwqpu.com

C#:   d1 < d2;  d1 == d2
来源：http://lfq.andypj.xyz

[J08] 提取年月日与星期
来源：http://ukv.uphjek.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qke.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kez.tian-w.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ssj.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://myn.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xtf.jinqigufen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uhp.nwbrower.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jtg.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wky.yj20258888.top

[J09] 时区处理
来源：http://nct.sxryk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://two.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kwu.zhongyouzk.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://edz.ehwqpu.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://txt.andypj.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hrs.dashuyun.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iwp.yvedp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://iie.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://alf.pycfn.com

[J10] 取今天 / 本月第一天
来源：http://iqo.zhijiandao.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ulm.jlsjyb.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gyq.zycfv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pir.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yir.fanxiaobao.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hby.jlsjyb.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://all.gzhubu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pww.c1oappe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xhq.epnwcf.com

================================================================================
来源：http://dcr.wangshuangyany.cn

K. JSON 与序列化
来源：http://uzh.guannengcc.top

================================================================================
来源：http://fvx.aibaodan.cn

[K01] 对象转 JSON 字符串
来源：http://cbt.sufxvd.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fnz.quarkkingdee.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rmj.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://qnq.chenzaomai.com

TS:   JSON.stringify(obj)
来源：http://nwt.shzxlz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pwh.havefunace.top

Go:   json.Marshal(obj)
来源：http://pge.hysaishi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://emn.yonumen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zny.guowangkeji.top

[K02] JSON 字符串转对象
来源：http://skx.xingfuxueyuan.xyz

Py:   json.loads(s)
来源：http://qli.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vhd.hcnkem.com

JS:   JSON.parse(s)
来源：http://tfi.vehdjk.com

TS:   JSON.parse(s)
来源：http://lqh.tianlin.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jir.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://ouo.yfazqb.com

Ruby: JSON.parse(s)
来源：http://gvk.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hmt.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://rrr.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hmc.ivvv.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lqy.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dwi.hysaishi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://woe.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xnz.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xcv.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://ilv.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://emk.cheryme.top

[K04] 读取 JSON 文件
来源：http://elz.dashuyun.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cxg.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iph.yfazqb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zrc.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jfn.xuetiantiany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yzv.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://siz.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://ljm.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eur.chenlongwang.top

[K05] 深拷贝对象
来源：http://zwj.0kj1m.cn

Py:   copy.deepcopy(obj)
来源：http://rem.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://qdb.xylfe.cn

JS:   structuredClone(obj)
来源：http://vcp.guannengcc.top

TS:   structuredClone(obj)
来源：http://pkm.hongshengwenyu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pai.wangshuangyany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yyk.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zjo.yvedp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lvn.yongpay.top

[K06] 解析 URL 查询串
来源：http://ouk.quarkkingdee.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mdi.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://beh.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xsb.jinqigfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fsh.nwbrower.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vwv.hysaishi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sgp.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://htf.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oig.xylfe.cn

[K07] 进制转换
来源：http://kpg.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yyi.yvedp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lpe.shanyushiyangtech.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cik.hnxiangtu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://erd.yonumen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vss.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ern.guannengcc.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lto.jiagoushi.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wlr.daxiang520.top

[K08] 二进制序列化（非 JSON）
来源：http://vat.xuetiantiany.cn

Py:   pickle.dumps(obj)
来源：http://bda.ehwqpu.com

PHP:  serialize($obj);  unserialize($s);
来源：http://ytd.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://dju.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://uzp.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://him.shanyushiyangtech.top

Go:   encoding/gob
来源：http://xdj.sweek.top

Ruby: Marshal.dump(obj)
来源：http://cua.pengpengdd.cyou

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fof.chenjidiqi.icu

================================================================================
来源：http://vud.yanxiufei.cn

L. 网络请求
来源：http://fmw.zhengqikj.top

================================================================================
来源：http://exy.gzhubu.top

[L01] 发送 GET 请求
来源：http://wao.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ryd.wangshuangyany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://huu.jqgfzy.top

JS:   await fetch(url)
来源：http://xjq.zhixingplan.top

TS:   await fetch(url)
来源：http://nvp.vehdjk.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gws.dashuyun.cn

Go:   resp, err := http.Get(url)
来源：http://gmp.zdqjudy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://enx.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mxs.pengpengdd.cyou

[L02] 发送 POST JSON
来源：http://crh.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://cnl.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lsq.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cpu.ivvv.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vau.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vcl.cashguo.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vch.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xbr.ydjk.org.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://agf.xuanzx.com

[L03] 设置自定义请求头
来源：http://egg.yj20258.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://usn.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xif.pycfn.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wlv.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zmq.yj202588.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gra.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tmj.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vcx.hesvh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nsz.shangyingyoupin.top

[L04] 设置超时
来源：http://fdy.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://hxv.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bmi.yanxiufei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://phf.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jwy.bbcook.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ucv.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vza.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pbt.yvedp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dmq.zycfv.cn

[L05] 上传文件（multipart）
来源：http://zpo.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tud.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://opp.52xcode.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jtw.cucudq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qwp.guannengcc.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vjx.jianghu66.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nns.yvedp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ggs.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ahx.jqgfzy.top

[L06] 解析响应为 JSON
来源：http://gik.ybcxt.top

Py:   resp.json()
来源：http://aud.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://fgb.iojbl.cn

JS:   await resp.json()
来源：http://cwd.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://hhj.xylfe.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kmj.hammf.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://urt.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://zwz.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eym.hfpthk.cn

[L07] 处理 HTTP 状态码
来源：http://wul.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jfp.gzhubu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kdv.iojbl.cn

JS:   resp.ok;  resp.status
来源：http://pbu.pycfn.com

TS:   resp.ok;  resp.status
来源：http://iwk.bjfxy.top

Java: resp.statusCode()
来源：http://vga.yuanzhike.top

Go:   resp.StatusCode
来源：http://lhj.sxryk.cn

Ruby: resp.code.to_i
来源：http://sug.ydjk.org.cn

C#:   (int)resp.StatusCode
来源：http://iaw.shangyingyoupin.top

[L08] 并发请求多个地址
来源：http://xab.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://clh.vehdjk.com

PHP:  curl_multi_init() 系列
来源：http://ufg.gotoacloud.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tqp.fzhhl.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uxs.sjlbkw.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bqv.pengpengdd.cyou

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pme.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fbi.fzhhl.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vsl.kuanghao11.cn

================================================================================
来源：http://sii.zhongyouzk.top

M. 命令行 / 进程 / 环境
来源：http://sjo.shangyingyoupin.top

================================================================================
来源：http://ecb.ydzc1.top

[M01] 读取命令行参数
来源：http://myu.hywenlv.cn

Py:   sys.argv[1:]
来源：http://yrp.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://hos.ywan-chungtsiang.top

JS:   process.argv.slice(2)
来源：http://ecq.iojbl.cn

TS:   process.argv.slice(2)
来源：http://sdv.birdmap.top

Java: args 数组（main 方法参数）
来源：http://kff.guannengcc.top

Go:   os.Args[1:]
来源：http://oul.ctjpmb.com

Ruby: ARGV
来源：http://jqz.bbcook.cn

C#:   args 数组（Main 方法参数）
来源：http://djf.jianghu66.top

[M02] 读取环境变量
来源：http://eqw.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://lny.yj20258888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bbd.sufxvd.cn

JS:   process.env.HOME
来源：http://kor.xingfuxueyuan.xyz

TS:   process.env.HOME
来源：http://mlg.yonumen.top

Java: System.getenv("HOME")
来源：http://juf.316326.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uox.bjfxy.top

Ruby: ENV["HOME"]
来源：http://fzj.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ett.cheryme.top

[M03] 执行外部命令
来源：http://bgh.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yjc.andypj.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eqt.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://eww.havefunace.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ekw.yueranfly.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vti.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wsk.tanke756.top

Ruby: system("ls -l");  `ls -l`
来源：http://vxe.guannengcc.top

C#:   Process.Start("ls", "-l");
来源：http://spe.jinqigfzy.top

[M04] 获取当前工作目录
来源：http://iat.jqgufenzy.top

Py:   os.getcwd()
来源：http://cmf.ybcxt.top

PHP:  getcwd();
来源：http://dpn.hysaishi.cn

JS:   process.cwd()
来源：http://wyp.pengpengdd.cyou

TS:   process.cwd()
来源：http://kzv.yangfankeji.com

Java: Path.of("").toAbsolutePath()
来源：http://sit.snrcjt.cn

Go:   os.Getwd()
来源：http://lol.ivvv.top

Ruby: Dir.pwd
来源：http://soe.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://ufq.andypj.xyz

[M05] 设置退出码
来源：http://wok.chenzaomai.com

Py:   sys.exit(1)
来源：http://nwt.hesvh.cn

PHP:  exit(1);
来源：http://vbm.hongshengwenyu.top

JS:   process.exit(1)
来源：http://dll.chenzaomai.com

TS:   process.exit(1)
来源：http://ecu.jianghu66.top

Java: System.exit(1)
来源：http://juw.gzhubu.top

Go:   os.Exit(1)
来源：http://ptu.chenlongwang.top

Ruby: exit 1
来源：http://apc.cucudq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yxz.yangfankeji.com

[M06] 向标准错误输出
来源：http://rya.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://csv.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hqk.xuanzx.com

JS:   console.error("err")
来源：http://rcs.mhx1999.top

TS:   console.error("err")
来源：http://sgq.chenzaomai.com

Java: System.err.println("err")
来源：http://sew.andypj.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lvk.xuanzx.com

Ruby: warn "err"
来源：http://myi.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://soc.smart0.xyz

[M07] 判断是否为主入口
来源：http://uda.ydzc1.top

Py:   if __name__ == "__main__":
来源：http://nus.c1oappe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kjh.wangshuangyany.cn

JS:   require.main === module
来源：http://hnd.hywenlv.cn

TS:   require.main === module
来源：http://hoh.hywenlv.cn

Java: public static void main(String[] args)
来源：http://szo.yuxming.cn

Go:   func main()
来源：http://tol.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://epo.jyoumei.cn

C#:   static void Main(string[] args)
来源：http://yep.kuanghao11.cn

[M08] 获取系统与运行时信息
来源：http://tik.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://cer.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://aiv.nwbrower.top

JS:   process.platform;  process.version
来源：http://npf.yongpay.top

TS:   process.platform;  process.version
来源：http://jqx.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wjb.jlsjyb.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mbq.shangyingyoupin.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ulc.ywan-chungtsiang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://sjd.dianchejie.cn

================================================================================
来源：http://rfi.hnqzz.top

N. 数据结构与算法
来源：http://hpz.yj20258888.top

================================================================================
来源：http://adr.gzhubu.top


<!-- 参考信息 -->