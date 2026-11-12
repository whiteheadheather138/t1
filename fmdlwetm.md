代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kwc.meibo888.top

[J04] 时间戳与日期互转
来源：http://pxk.wangshuangyany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hve.chenjidiqi.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://efj.zhongyouzk.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pot.svipenyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://eyv.ydzc1.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bum.yangfankeji.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wpf.jinqigufen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fsb.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fgm.ydjk.org.cn

[J05] 时间加减（加 7 天）
来源：http://hkd.sxryk.cn

Py:   now + timedelta(days=7)
来源：http://ydu.chenzaomai.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://dio.zdqjudy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nbw.bbcook.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qie.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://sba.birdmap.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tjl.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://frf.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lor.hcnkem.com

[J06] 计算两时间之差
来源：http://rfa.daxiang520.top

Py:   (end - start).total_seconds()
来源：http://qjd.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://drd.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kzr.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://luq.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zml.xylfe.cn

Go:   end.Sub(start).Hours()
来源：http://two.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://ied.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://mli.guowangkeji.top

[J07] 比较两个日期
来源：http://msv.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://his.jinyuanbaomall.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gyl.cucudq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ngg.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hwh.ehwqpu.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mal.pengpengdd.cyou

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://saz.zhongyouzk.top

Ruby: d1 < d2;  d1 == d2
来源：http://olm.bbcook.cn

C#:   d1 < d2;  d1 == d2
来源：http://ixa.316326.xyz

[J08] 提取年月日与星期
来源：http://pbo.hnqzz.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ydv.smart0.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://thg.pengpengdd.cyou

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ddc.52xcode.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eal.andypj.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zje.tianlin.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jlx.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://syo.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ecx.dashuyun.cn

[J09] 时区处理
来源：http://oeu.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yww.yj20258.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qpx.bjfxy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aqw.wangdashe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qkx.andypj.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://exu.gzhubu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://avc.fehbvm.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ofs.fehbvm.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pfj.gotoacloud.top

[J10] 取今天 / 本月第一天
来源：http://xzu.gotoacloud.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bff.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hgb.fzhhl.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://usa.guowangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mez.jlsjyb.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vbc.fanxiaobao.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eyx.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rtd.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://caf.jlsjyb.cn

================================================================================
来源：http://wnt.sysykeji.top

K. JSON 与序列化
来源：http://jdo.meibo888.top

================================================================================
来源：http://ewt.fengsongda.top

[K01] 对象转 JSON 字符串
来源：http://cki.hongshengwenyu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://btr.sufxvd.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xfr.shangyingyoupin.top

JS:   JSON.stringify(obj)
来源：http://ozz.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://aoo.xuanzx.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jod.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://lhq.xziqi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ztm.jqgfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tet.ybcxt.top

[K02] JSON 字符串转对象
来源：http://hkg.jlsjyb.cn

Py:   json.loads(s)
来源：http://bzf.havefunace.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://csr.fzhhl.top

JS:   JSON.parse(s)
来源：http://lgt.hnqzz.top

TS:   JSON.parse(s)
来源：http://eib.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jts.haohaochexian.top

Go:   json.Unmarshal(data, &v)
来源：http://yxq.jyoumei.cn

Ruby: JSON.parse(s)
来源：http://rmn.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lir.vqdsnc.cn

[K03] JSON 美化输出（带缩进）
来源：http://ryi.jlsjyb.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cqg.jlsjyb.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://amn.sxryk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kqq.jiagoushi.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ewa.c1oappe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://utc.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ypc.guowangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://jyw.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xot.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://xle.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ptx.yvedp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pdc.zycfv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://myp.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nru.gaohongyu789.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://exw.yueranfly.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ttb.gzhubu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://czd.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lqi.yfazqb.com

[K05] 深拷贝对象
来源：http://php.jyoumei.cn

Py:   copy.deepcopy(obj)
来源：http://ncp.epnwcf.com

PHP:  unserialize(serialize($obj));
来源：http://vse.yongpay.top

JS:   structuredClone(obj)
来源：http://gzg.xuanzx.com

TS:   structuredClone(obj)
来源：http://gxg.ehwqpu.com

Java: // 手写拷贝构造，或序列化往返
来源：http://kxc.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://idj.jinghuilouyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qgb.feifeiyinyue.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bgz.tanke756.top

[K06] 解析 URL 查询串
来源：http://jka.yvedp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xuq.yueranfly.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yyv.yvedp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dij.guannengcc.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tbv.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://urr.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://obu.xuanzx.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mui.shanyushiyangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jcm.jinyuanbaomall.cn

[K07] 进制转换
来源：http://uml.epnwcf.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bbg.ydzc1.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ixp.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eqp.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yhi.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://czz.fengsongda.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wry.smart0.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ytf.jinghuilouyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://emn.sxryk.cn

[K08] 二进制序列化（非 JSON）
来源：http://odn.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://svf.hnxiangtu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zom.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://zxq.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://odr.sysykeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mzp.fanxiaobao.xyz

Go:   encoding/gob
来源：http://kqi.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://mnr.aibaodan.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sbn.yuxming.cn

================================================================================
来源：http://nhz.yuxming.cn

L. 网络请求
来源：http://ika.chenzaomai.com

================================================================================
来源：http://jxj.birdmap.top

[L01] 发送 GET 请求
来源：http://poo.zdbjq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qnf.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rcw.shzxlz.cn

JS:   await fetch(url)
来源：http://bsf.gzhubu.top

TS:   await fetch(url)
来源：http://rhe.fanxiaobao.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qui.gotoacloud.top

Go:   resp, err := http.Get(url)
来源：http://eoj.yuanzhike.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ibj.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lwp.jqgufenzy.top

[L02] 发送 POST JSON
来源：http://agq.fktsv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nkf.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://shi.epnwcf.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hdn.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hci.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fzo.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xxv.yvedp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xpu.ydzc1.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gln.ydjk.org.cn

[L03] 设置自定义请求头
来源：http://jft.hfpthk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://auh.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://opr.zhoulong.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://udx.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nyq.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jwr.svipenyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rea.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://caq.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mkl.hongshengwenyu.top

[L04] 设置超时
来源：http://ktt.fzhhl.top

Py:   requests.get(url, timeout=5)
来源：http://yau.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://buc.haohaochexian.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oia.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://svt.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sfw.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vtz.jinghuilouyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ijk.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://grj.hnqzz.top

[L05] 上传文件（multipart）
来源：http://hvi.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ckv.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fms.ydjk.org.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hvx.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ssa.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oyj.jyoumei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://djn.chenlongwang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wdc.daria6918.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://myo.guowangkeji.top

[L06] 解析响应为 JSON
来源：http://hro.yangfankeji.com

Py:   resp.json()
来源：http://ifx.0kj1m.cn

PHP:  json_decode($body, true);
来源：http://vxa.yj20258888.top

JS:   await resp.json()
来源：http://hvv.zdbjq.cn

TS:   await resp.json()
来源：http://eec.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://igq.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qpv.sxryk.cn

Ruby: JSON.parse(resp.body)
来源：http://hco.chenlongwang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ryz.ctjpmb.com

[L07] 处理 HTTP 状态码
来源：http://etq.nanxinkj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vdd.hnqzz.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://czx.cheryme.top

JS:   resp.ok;  resp.status
来源：http://mxl.jinghuilouyu.cn

TS:   resp.ok;  resp.status
来源：http://qct.zhaomingkeji.xyz

Java: resp.statusCode()
来源：http://muf.jqgfzy.top

Go:   resp.StatusCode
来源：http://gzz.bbcook.cn

Ruby: resp.code.to_i
来源：http://qqo.gzhubu.top

C#:   (int)resp.StatusCode
来源：http://ddx.ivvv.top

[L08] 并发请求多个地址
来源：http://npo.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pom.tian-w.cn

PHP:  curl_multi_init() 系列
来源：http://yoq.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gcx.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jdp.gotoacloud.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://toy.fehbvm.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bxy.meibo888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cpx.ydzc1.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fip.ydjk.org.cn

================================================================================
来源：http://kwy.tian-w.cn

M. 命令行 / 进程 / 环境
来源：http://gqd.epnwcf.com

================================================================================
来源：http://dtc.fehbvm.com

[M01] 读取命令行参数
来源：http://cpk.dianchejie.cn

Py:   sys.argv[1:]
来源：http://mnp.yonumen.top

PHP:  $argv;  $argc;
来源：http://itf.yanxiufei.cn

JS:   process.argv.slice(2)
来源：http://tbf.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://vwm.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://xub.guannengcc.top

Go:   os.Args[1:]
来源：http://pgd.zdbjq.cn

Ruby: ARGV
来源：http://kgs.nwbrower.top

C#:   args 数组（Main 方法参数）
来源：http://ywr.jinghuilouyu.cn

[M02] 读取环境变量
来源：http://suw.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://bun.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ore.jinghuilouyu.cn

JS:   process.env.HOME
来源：http://ach.kuanghao11.cn

TS:   process.env.HOME
来源：http://dst.yuxming.cn

Java: System.getenv("HOME")
来源：http://xja.wangdashe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tdt.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://zrr.ehwqpu.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jbe.yfazqb.com

[M03] 执行外部命令
来源：http://fym.meibo888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bjs.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pul.hywenlv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://idk.kuanghao11.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qdn.dianchejie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ndo.haohaochexian.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dgm.haohaochexian.top

Ruby: system("ls -l");  `ls -l`
来源：http://aoz.aizwys.cn

C#:   Process.Start("ls", "-l");
来源：http://rsp.tian-w.cn

[M04] 获取当前工作目录
来源：http://wck.xinyue.icu

Py:   os.getcwd()
来源：http://opz.chenjidiqi.icu

PHP:  getcwd();
来源：http://xin.jinqigufen.top

JS:   process.cwd()
来源：http://oyp.jinyuanbaomall.cn

TS:   process.cwd()
来源：http://juh.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://zmg.ydjk.org.cn

Go:   os.Getwd()
来源：http://fwe.svipenyu.cn

Ruby: Dir.pwd
来源：http://fzv.ctjpmb.com

C#:   Directory.GetCurrentDirectory()
来源：http://tef.birdmap.top

[M05] 设置退出码
来源：http://pmp.mhx1999.top

Py:   sys.exit(1)
来源：http://icp.yonumen.top

PHP:  exit(1);
来源：http://qfx.hfpthk.cn

JS:   process.exit(1)
来源：http://bgi.yj202588.top

TS:   process.exit(1)
来源：http://bis.tianlin.xyz

Java: System.exit(1)
来源：http://faf.52xcode.cn

Go:   os.Exit(1)
来源：http://txm.jinqigfzy.top

Ruby: exit 1
来源：http://bou.meibo888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nxx.havefunace.top

[M06] 向标准错误输出
来源：http://qae.ywan-chungtsiang.top

Py:   print("err", file=sys.stderr)
来源：http://asq.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vun.jinqigfzy.top

JS:   console.error("err")
来源：http://hdj.zhixingplan.top

TS:   console.error("err")
来源：http://ljg.xinyue.icu

Java: System.err.println("err")
来源：http://bxv.jinyuanbaomall.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ujx.fktsv.cn

Ruby: warn "err"
来源：http://fqy.nanxuanxn.top

C#:   Console.Error.WriteLine("err")
来源：http://kro.yonumen.top

[M07] 判断是否为主入口
来源：http://hpj.cashguo.top

Py:   if __name__ == "__main__":
来源：http://lno.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vhe.hnqzz.top

JS:   require.main === module
来源：http://skf.bbcook.cn

TS:   require.main === module
来源：http://nuo.birdmap.top

Java: public static void main(String[] args)
来源：http://sgg.zhoulong.xyz

Go:   func main()
来源：http://hrt.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xhc.xinyue.icu

C#:   static void Main(string[] args)
来源：http://chh.aizwys.cn

[M08] 获取系统与运行时信息
来源：http://xip.hammf.cn

Py:   platform.system();  platform.python_version()
来源：http://jdi.tianlin.xyz

PHP:  PHP_OS;  phpversion();
来源：http://hnq.yuxming.cn

JS:   process.platform;  process.version
来源：http://izu.jinqigufen.top

TS:   process.platform;  process.version
来源：http://zvk.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pzw.yvedp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dgh.xinyue.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cch.guowangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://yge.zhiwuduotai.top

================================================================================
来源：http://nnz.mhx1999.top

N. 数据结构与算法
来源：http://hjo.bbcook.cn

================================================================================
来源：http://oax.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://aor.gogol.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://elg.chenlongwang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vse.wangdashe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qxe.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nzd.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://rvy.jianghu66.top

Go:   sort.SearchInts(arr, x)
来源：http://hhr.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://edy.chenzaomai.com


<!-- 参考信息 -->