代发 wailian999

TS:   new Date("2024-01-02")
来源：http://mpb.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://ptg.daria6918.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jyn.xinyue.icu

Ruby: Date.parse("2024-01-02")
来源：http://edp.52xcode.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://seu.guowangkeji.top

[J04] 时间戳与日期互转
来源：http://kah.ydzc1.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iuf.haohaochexian.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fle.yanxiufei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aen.316326.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://xct.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://foe.redwolf501.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qpr.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cct.hnxiangtu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kpx.tian-w.cn

[J05] 时间加减（加 7 天）
来源：http://fgz.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://ptr.jyoumei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://soy.nanxuanxn.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gjt.shanyushiyangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eer.ppjwa.cn

Java: LocalDate.now().plusDays(7)
来源：http://txn.havefunace.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ucm.chenzaomai.com

Ruby: Time.now + 7 * 86400
来源：http://zmr.yanxiufei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vem.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://vsd.haohaochexian.top

Py:   (end - start).total_seconds()
来源：http://tcz.hongshengwenyu.top

PHP:  $end->diff($start)->days;
来源：http://qhn.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xir.sufxvd.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://djd.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://wlp.cucudq.cn

Go:   end.Sub(start).Hours()
来源：http://woe.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://gra.ctjpmb.com

C#:   (end - start).TotalSeconds
来源：http://ezo.quarkkingdee.top

[J07] 比较两个日期
来源：http://lcc.0kj1m.cn

Py:   d1 < d2;  d1 == d2
来源：http://uad.andypj.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jzc.xinyue.icu

JS:   d1.getTime() < d2.getTime()
来源：http://vvj.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://otj.gotoacloud.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://daw.yj202588.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eet.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://hwp.xuetiantiany.cn

C#:   d1 < d2;  d1 == d2
来源：http://aon.chenzaomai.com

[J08] 提取年月日与星期
来源：http://wzi.tanke756.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jcv.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://krx.epnwcf.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kgr.sjlbkw.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zjh.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://whc.andypj.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zsh.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lvd.zhoulong.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xlo.zhoulong.xyz

[J09] 时区处理
来源：http://nrg.yanxiufei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sja.epnwcf.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gwv.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oyp.xingfuxueyuan.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://trs.cqqwz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qve.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cnk.sysykeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rsh.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xzf.tanke756.top

[J10] 取今天 / 本月第一天
来源：http://pgm.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://owy.shanyushiyangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nhg.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wci.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bvg.yj202588.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://got.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hql.yvedp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jnd.daxiang520.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dqt.tanke756.top

================================================================================
来源：http://oia.andypj.xyz

K. JSON 与序列化
来源：http://ysm.sxryk.cn

================================================================================
来源：http://lbn.yanxiufei.cn

[K01] 对象转 JSON 字符串
来源：http://lei.ivvv.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://and.shzxlz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dcr.ctjpmb.com

JS:   JSON.stringify(obj)
来源：http://bux.tian-w.cn

TS:   JSON.stringify(obj)
来源：http://jxm.fengsongda.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://scp.birdmap.top

Go:   json.Marshal(obj)
来源：http://ear.yvedp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wcs.ivvv.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vij.meibo888.top

[K02] JSON 字符串转对象
来源：http://ano.fanxiaobao.xyz

Py:   json.loads(s)
来源：http://bxx.zhongyouzk.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rtu.hnqzz.top

JS:   JSON.parse(s)
来源：http://qtx.zdqjudy.top

TS:   JSON.parse(s)
来源：http://hhb.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xwt.zycfv.cn

Go:   json.Unmarshal(data, &v)
来源：http://awx.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://gxk.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://meb.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://cpl.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uoz.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bly.ppjwa.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sgx.gzhubu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rru.ywan-chungtsiang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cxd.shanyushiyangtech.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wwk.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xhb.sysykeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sws.ydjk.org.cn

[K04] 读取 JSON 文件
来源：http://hor.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fba.dashuyun.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jux.shangyingyoupin.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://foe.daria6918.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cwl.yuxming.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lnf.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ryf.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://pxb.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fzk.jianghu66.top

[K05] 深拷贝对象
来源：http://ozr.yanxiufei.cn

Py:   copy.deepcopy(obj)
来源：http://une.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://veg.yuxming.cn

JS:   structuredClone(obj)
来源：http://eem.tian-w.cn

TS:   structuredClone(obj)
来源：http://mke.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dpo.xingfuxueyuan.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iqy.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pgc.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://lsz.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://rod.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vrm.hammf.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bep.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kop.zhijiandao.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zxu.ehwqpu.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mok.cqqwz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zia.sweek.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://trn.fengsongda.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pwq.quarkkingdee.top

[K07] 进制转换
来源：http://rfl.fzhhl.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fcs.pengpengdd.cyou

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pow.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mhs.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bgp.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zsi.jqgufenzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gel.ydjk.org.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cin.vehdjk.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tuh.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://ndq.9152youxi.cn

Py:   pickle.dumps(obj)
来源：http://toq.shzxlz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ptj.uphjek.com

JS:   v8.serialize(obj)        // Node
来源：http://dyx.yj20258888.top

TS:   v8.serialize(obj)        // Node
来源：http://adf.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pcv.hongshengwenyu.top

Go:   encoding/gob
来源：http://dfj.gzhubu.top

Ruby: Marshal.dump(obj)
来源：http://bxb.pycfn.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fus.hammf.cn

================================================================================
来源：http://uxz.hammf.cn

L. 网络请求
来源：http://sii.kuanghao11.cn

================================================================================
来源：http://nmm.shanyushiyangkeji.top

[L01] 发送 GET 请求
来源：http://xzz.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xof.ctjpmb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zjw.guowangkeji.top

JS:   await fetch(url)
来源：http://xse.ydjk.org.cn

TS:   await fetch(url)
来源：http://ppr.shanyushiyangtech.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wij.fanxiaobao.xyz

Go:   resp, err := http.Get(url)
来源：http://kby.zhixingplan.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lfp.bbcook.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mkl.hywenlv.cn

[L02] 发送 POST JSON
来源：http://onb.tanke756.top

Py:   requests.post(url, json={"a": 1})
来源：http://xdm.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tgs.bjfxy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://igd.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://msb.birdmap.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ace.gaohongyu789.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://axg.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qeg.zhongyouzk.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fft.sysykeji.top

[L03] 设置自定义请求头
来源：http://lhf.vqdsnc.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ghy.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ooq.yj202588.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hid.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kcb.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vhe.sxryk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ibp.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fda.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://luy.gzhubu.top

[L04] 设置超时
来源：http://ybw.svipenyu.cn

Py:   requests.get(url, timeout=5)
来源：http://rmh.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xrr.xuetiantiany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gsd.hysaishi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ckd.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://euo.zhongyouzk.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rta.316326.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tuc.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://swe.yueranfly.top

[L05] 上传文件（multipart）
来源：http://cbp.vqdsnc.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pbm.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://plr.smart0.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kpz.bjfxy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oay.yonumen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://elk.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bcl.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://agy.zhoulong.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://njd.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://eog.ydzc1.top

Py:   resp.json()
来源：http://ncd.xylfe.cn

PHP:  json_decode($body, true);
来源：http://mtw.jqgfzy.top

JS:   await resp.json()
来源：http://ybe.zhoulong.xyz

TS:   await resp.json()
来源：http://cvp.feifeiyinyue.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pdf.jianghu66.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vtj.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://pet.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://plf.yanxiufei.cn

[L07] 处理 HTTP 状态码
来源：http://isx.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gqk.aizwys.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ciw.ydzc1.top

JS:   resp.ok;  resp.status
来源：http://hnn.pycfn.com

TS:   resp.ok;  resp.status
来源：http://fhq.jinqigufen.top

Java: resp.statusCode()
来源：http://oio.zhijiandao.cn

Go:   resp.StatusCode
来源：http://kpy.snrcjt.cn

Ruby: resp.code.to_i
来源：http://bzo.hammf.cn

C#:   (int)resp.StatusCode
来源：http://yrk.zhoulong.xyz

[L08] 并发请求多个地址
来源：http://mjo.vqdsnc.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://idl.tianlin.xyz

PHP:  curl_multi_init() 系列
来源：http://nqm.bjfxy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fmt.meibo888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vec.yuanzhike.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aap.yueranfly.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://exr.jyoumei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vjf.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jlu.yangfankeji.com

================================================================================
来源：http://cep.zhengqikj.top

M. 命令行 / 进程 / 环境
来源：http://ntx.yj20258888.top

================================================================================
来源：http://saw.iojbl.cn

[M01] 读取命令行参数
来源：http://qka.jlsjyb.cn

Py:   sys.argv[1:]
来源：http://dee.epnwcf.com

PHP:  $argv;  $argc;
来源：http://eqn.aizwys.cn

JS:   process.argv.slice(2)
来源：http://kuf.uphjek.com

TS:   process.argv.slice(2)
来源：http://qsi.havefunace.top

Java: args 数组（main 方法参数）
来源：http://uja.sysykeji.top

Go:   os.Args[1:]
来源：http://ahd.fktsv.cn

Ruby: ARGV
来源：http://sgy.fanxiaobao.xyz

C#:   args 数组（Main 方法参数）
来源：http://yot.zhiwuduotai.top

[M02] 读取环境变量
来源：http://cqo.fktsv.cn

Py:   os.environ.get("HOME")
来源：http://bgn.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ehh.316326.xyz

JS:   process.env.HOME
来源：http://vas.zdbjq.cn

TS:   process.env.HOME
来源：http://mnc.aibaodan.cn

Java: System.getenv("HOME")
来源：http://xvm.quarkkingdee.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dgd.yonumen.top

Ruby: ENV["HOME"]
来源：http://dif.aibaodan.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eei.zhoulong.xyz

[M03] 执行外部命令
来源：http://qes.dianchejie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pas.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vxj.yanxiufei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ozr.sysykeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kkw.dashuyun.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cyn.nanxinkj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pav.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://wkr.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://sls.sxryk.cn

[M04] 获取当前工作目录
来源：http://dud.cheryme.top

Py:   os.getcwd()
来源：http://udt.aibaodan.cn

PHP:  getcwd();
来源：http://bxq.aizwys.cn

JS:   process.cwd()
来源：http://wqo.nwbrower.top

TS:   process.cwd()
来源：http://wgu.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://bqo.vqdsnc.cn

Go:   os.Getwd()
来源：http://wfr.guannengcc.top

Ruby: Dir.pwd
来源：http://mop.gaohongyu789.top

C#:   Directory.GetCurrentDirectory()
来源：http://xzu.svipenyu.cn

[M05] 设置退出码
来源：http://rcv.xuanzx.com

Py:   sys.exit(1)
来源：http://jnp.316326.xyz

PHP:  exit(1);
来源：http://qhs.gogol.net.cn

JS:   process.exit(1)
来源：http://rqd.c1oappe.top

TS:   process.exit(1)
来源：http://vgc.bbcook.cn

Java: System.exit(1)
来源：http://zku.316326.xyz

Go:   os.Exit(1)
来源：http://vkg.hywenlv.cn

Ruby: exit 1
来源：http://btl.smart0.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qao.haohaochexian.top

[M06] 向标准错误输出
来源：http://adq.hongshengwenyu.top

Py:   print("err", file=sys.stderr)
来源：http://omq.jinqigfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tdn.wangdashe.top

JS:   console.error("err")
来源：http://jmo.52xcode.cn

TS:   console.error("err")
来源：http://nbv.hysaishi.cn

Java: System.err.println("err")
来源：http://hcv.feifeiyinyue.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mtq.hnxiangtu.top

Ruby: warn "err"
来源：http://ewc.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://jqx.cheryme.top

[M07] 判断是否为主入口
来源：http://kzz.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://exh.nwbrower.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nmf.hywenlv.cn

JS:   require.main === module
来源：http://frz.jqgfzy.top

TS:   require.main === module
来源：http://sbx.xziqi.cn

Java: public static void main(String[] args)
来源：http://nra.hysaishi.cn

Go:   func main()
来源：http://wvs.kuanghao11.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vdo.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://xcf.svipenyu.cn

[M08] 获取系统与运行时信息
来源：http://qfp.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://bfq.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://rvi.xuetiantiany.cn

JS:   process.platform;  process.version
来源：http://tcq.chenjidiqi.icu

TS:   process.platform;  process.version
来源：http://gfn.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jec.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dqh.52xcode.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ljb.yj202588.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://cyk.sweek.top

================================================================================
来源：http://kdn.xuanzx.com

N. 数据结构与算法
来源：http://hax.zhengqikj.top

================================================================================
来源：http://oxz.havefunace.top

[N01] 二分查找（有序数组）
来源：http://qhq.jinghuilouyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tun.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://adh.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ryd.zhijiandao.cn


<!-- 参考信息 -->