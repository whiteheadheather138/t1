代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kcb.zhijiandao.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lck.fehbvm.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ool.yuxming.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wlc.hywenlv.cn

[J03] 字符串解析为日期
来源：http://vxq.0kj1m.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://agn.gotoacloud.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ydq.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://vyw.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://wzz.aizwys.cn

Java: LocalDate.parse("2024-01-02")
来源：http://prq.gzhubu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xhe.xuetiantiany.cn

Ruby: Date.parse("2024-01-02")
来源：http://vqg.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mbs.xingfuxueyuan.xyz

[J04] 时间戳与日期互转
来源：http://wxt.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://utj.fktsv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hzx.ydjk.org.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://egl.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ims.hesvh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mss.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zad.guowangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wss.zhaomingkeji.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fhq.aibaodan.cn

[J05] 时间加减（加 7 天）
来源：http://mrk.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://sgm.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://nzc.jinghuilouyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mna.316326.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cwi.fehbvm.com

Java: LocalDate.now().plusDays(7)
来源：http://voo.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fif.dashuyun.cn

Ruby: Time.now + 7 * 86400
来源：http://umi.pycfn.com

C#:   DateTime.Now.AddDays(7)
来源：http://ycn.snrcjt.cn

[J06] 计算两时间之差
来源：http://kde.sweek.top

Py:   (end - start).total_seconds()
来源：http://qzt.zhaomingkeji.xyz

PHP:  $end->diff($start)->days;
来源：http://wjv.dianchejie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jsl.hongshengwenyu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ryo.pycfn.com

Java: Duration.between(start, end).toSeconds()
来源：http://fcd.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://kad.birdmap.top

Ruby: end - start                 # 返回秒数
来源：http://tnv.9152youxi.cn

C#:   (end - start).TotalSeconds
来源：http://bzx.cqqwz.cn

[J07] 比较两个日期
来源：http://iti.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://iih.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bfz.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://jcb.quarkkingdee.top

TS:   d1.getTime() < d2.getTime()
来源：http://hno.zhoulong.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qdq.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://apz.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://eyg.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://nxa.yuanzhike.top

[J08] 提取年月日与星期
来源：http://iij.zycfv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wop.epnwcf.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xtg.yj20258.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gao.quarkkingdee.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nyj.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dhx.shanyushiyangtech.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vzz.jinyuanbaomall.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://miy.shanyushiyangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dag.jinghuilouyu.cn

[J09] 时区处理
来源：http://qps.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tbi.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gdt.hysaishi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nus.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uod.jqgfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rki.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bhg.sysykeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zjp.hcnkem.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://auj.xziqi.cn

[J10] 取今天 / 本月第一天
来源：http://efr.c1oappe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fiy.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ota.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vax.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wyj.jqgufenzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kwo.meibo888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ssb.yj202588.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fsd.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://whh.guowangkeji.top

================================================================================
来源：http://dst.sjlbkw.cn

K. JSON 与序列化
来源：http://szq.xuetiantiany.cn

================================================================================
来源：http://heu.zycfv.cn

[K01] 对象转 JSON 字符串
来源：http://hkw.jqgfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fpd.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ato.cucudq.cn

JS:   JSON.stringify(obj)
来源：http://blw.gotoacloud.top

TS:   JSON.stringify(obj)
来源：http://rqg.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vle.vehdjk.com

Go:   json.Marshal(obj)
来源：http://dsg.yuxming.cn

Ruby: obj.to_json                                     // require "json"
来源：http://say.tanke756.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kos.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://got.ehwqpu.com

Py:   json.loads(s)
来源：http://pyx.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://znk.hfpthk.cn

JS:   JSON.parse(s)
来源：http://yxt.xylfe.cn

TS:   JSON.parse(s)
来源：http://ytp.hfpthk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jrt.yonumen.top

Go:   json.Unmarshal(data, &v)
来源：http://uss.hcnkem.com

Ruby: JSON.parse(s)
来源：http://ygi.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qgj.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://eex.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fup.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lwb.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hoc.hnqzz.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yhh.c1oappe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rps.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wqf.ppjwa.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rkn.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://srf.ybcxt.top

[K04] 读取 JSON 文件
来源：http://naq.jinqigufen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tgz.yuxming.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qgh.zhaomingkeji.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://arn.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://civ.sufxvd.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lln.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://duu.kuanghao11.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ddh.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ldz.cashguo.top

[K05] 深拷贝对象
来源：http://jgm.sxryk.cn

Py:   copy.deepcopy(obj)
来源：http://kvk.cashguo.top

PHP:  unserialize(serialize($obj));
来源：http://ozs.ybcxt.top

JS:   structuredClone(obj)
来源：http://tau.yj20258888.top

TS:   structuredClone(obj)
来源：http://ted.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nzj.yongpay.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tru.jinqigufen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://woa.shanyushiyangtech.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gnl.havefunace.top

[K06] 解析 URL 查询串
来源：http://zpk.jlsjyb.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lzj.dashuyun.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qfq.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://afh.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ggn.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hhz.hnqzz.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rte.52xcode.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ten.jinyuanbaomall.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zbu.ppjwa.cn

[K07] 进制转换
来源：http://pcb.smart0.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zfi.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zxa.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qpk.nwbrower.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pqm.shzxlz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fyo.gaohongyu789.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cfq.zhixingplan.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sja.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zlq.chenjidiqi.icu

[K08] 二进制序列化（非 JSON）
来源：http://ekk.ctjpmb.com

Py:   pickle.dumps(obj)
来源：http://jkf.zdqjudy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sjc.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://xmx.zycfv.cn

TS:   v8.serialize(obj)        // Node
来源：http://ysv.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gvw.vqdsnc.cn

Go:   encoding/gob
来源：http://qoj.feifeiyinyue.top

Ruby: Marshal.dump(obj)
来源：http://mkl.kuanghao11.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pij.havefunace.top

================================================================================
来源：http://ybm.nwbrower.top

L. 网络请求
来源：http://kdu.yuanzhike.top

================================================================================
来源：http://qjc.yanxiufei.cn

[L01] 发送 GET 请求
来源：http://erh.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://osq.cheryme.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rek.hysaishi.cn

JS:   await fetch(url)
来源：http://qvi.hywenlv.cn

TS:   await fetch(url)
来源：http://bxa.chenjidiqi.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xgw.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://lux.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yiz.hesvh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://etc.chenjidiqi.icu

[L02] 发送 POST JSON
来源：http://fih.iojbl.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zrm.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vff.yvedp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kpu.hywenlv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zop.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bqa.birdmap.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nbe.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lvq.daxiang520.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://akz.bjfxy.top

[L03] 设置自定义请求头
来源：http://sft.jiagoushi.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://adj.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zrg.dianchejie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://boq.yangfankeji.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uys.ivvv.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rhx.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://llw.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fye.mhx1999.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://npo.pengpengdd.cyou

[L04] 设置超时
来源：http://yzw.sufxvd.cn

Py:   requests.get(url, timeout=5)
来源：http://ahj.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qgx.yanxiufei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://phs.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ybc.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ywu.snrcjt.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jmv.yuxming.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gfn.yuanzhike.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qcg.xziqi.cn

[L05] 上传文件（multipart）
来源：http://aew.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ppo.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tzq.yuxming.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gyx.sxryk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sfg.yangfankeji.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wom.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pse.pengpengdd.cyou

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uqz.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gyn.vqdsnc.cn

[L06] 解析响应为 JSON
来源：http://wza.jqgfzy.top

Py:   resp.json()
来源：http://sng.ivvv.top

PHP:  json_decode($body, true);
来源：http://qvp.fehbvm.com

JS:   await resp.json()
来源：http://kwt.meibo888.top

TS:   await resp.json()
来源：http://rqe.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rtg.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fmg.shanyushiyangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://mwk.xinyue.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fdq.zhijiandao.cn

[L07] 处理 HTTP 状态码
来源：http://nye.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cuc.andypj.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zdw.hysaishi.cn

JS:   resp.ok;  resp.status
来源：http://dym.hfpthk.cn

TS:   resp.ok;  resp.status
来源：http://gry.yongpay.top

Java: resp.statusCode()
来源：http://qya.xylfe.cn

Go:   resp.StatusCode
来源：http://sty.shanyushiyangkeji.top

Ruby: resp.code.to_i
来源：http://otv.yfazqb.com

C#:   (int)resp.StatusCode
来源：http://dpx.daria6918.cn

[L08] 并发请求多个地址
来源：http://tpw.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ytu.zhongyouzk.top

PHP:  curl_multi_init() 系列
来源：http://omb.chenjidiqi.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kdp.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dfb.shuidangran.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nea.feifeiyinyue.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aul.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pat.yangfankeji.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://umc.cdnleiting.top

================================================================================
来源：http://qob.ctjpmb.com

M. 命令行 / 进程 / 环境
来源：http://wqn.pengpengdd.cyou

================================================================================
来源：http://nuw.zhongyouzk.top

[M01] 读取命令行参数
来源：http://myt.ybcxt.top

Py:   sys.argv[1:]
来源：http://bhq.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://eox.tianlin.xyz

JS:   process.argv.slice(2)
来源：http://nbu.shzxlz.cn

TS:   process.argv.slice(2)
来源：http://vuu.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://nke.fktsv.cn

Go:   os.Args[1:]
来源：http://ujv.fehbvm.com

Ruby: ARGV
来源：http://tvw.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://gum.dianchejie.cn

[M02] 读取环境变量
来源：http://iuq.ivvv.top

Py:   os.environ.get("HOME")
来源：http://gks.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vng.xylfe.cn

JS:   process.env.HOME
来源：http://knq.fengsongda.top

TS:   process.env.HOME
来源：http://jkk.yvedp.cn

Java: System.getenv("HOME")
来源：http://dmc.dianchejie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vis.cucudq.cn

Ruby: ENV["HOME"]
来源：http://trt.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://low.xinyue.icu

[M03] 执行外部命令
来源：http://gri.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vsf.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://khx.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wse.316326.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://xgu.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yhb.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ruy.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kxl.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://vqg.tarul.cn

[M04] 获取当前工作目录
来源：http://eol.bbcook.cn

Py:   os.getcwd()
来源：http://odh.xylfe.cn

PHP:  getcwd();
来源：http://mxn.fengsongda.top

JS:   process.cwd()
来源：http://mpi.jyoumei.cn

TS:   process.cwd()
来源：http://evj.wangshuangyany.cn

Java: Path.of("").toAbsolutePath()
来源：http://ywt.quarkkingdee.top

Go:   os.Getwd()
来源：http://occ.shzxlz.cn

Ruby: Dir.pwd
来源：http://uqf.cdnleiting.top

C#:   Directory.GetCurrentDirectory()
来源：http://kth.cheryme.top

[M05] 设置退出码
来源：http://pdw.sufxvd.cn

Py:   sys.exit(1)
来源：http://amf.9152youxi.cn

PHP:  exit(1);
来源：http://ksn.svipenyu.cn

JS:   process.exit(1)
来源：http://ubp.xingfuxueyuan.xyz

TS:   process.exit(1)
来源：http://fyf.pycfn.com

Java: System.exit(1)
来源：http://vpb.hnqzz.top

Go:   os.Exit(1)
来源：http://vcw.yfazqb.com

Ruby: exit 1
来源：http://dxl.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mvj.redwolf501.top

[M06] 向标准错误输出
来源：http://ama.52xcode.cn

Py:   print("err", file=sys.stderr)
来源：http://cge.yuxming.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fqf.uphjek.com

JS:   console.error("err")
来源：http://bwn.quarkkingdee.top

TS:   console.error("err")
来源：http://xtb.cdnleiting.top

Java: System.err.println("err")
来源：http://ygp.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kis.daxiang520.top

Ruby: warn "err"
来源：http://ueu.yangfankeji.com

C#:   Console.Error.WriteLine("err")
来源：http://wvy.sysykeji.top

[M07] 判断是否为主入口
来源：http://uge.cheryme.top

Py:   if __name__ == "__main__":
来源：http://ndt.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dis.andypj.xyz

JS:   require.main === module
来源：http://csz.fanxiaobao.xyz

TS:   require.main === module
来源：http://kpu.haohaochexian.top

Java: public static void main(String[] args)
来源：http://dcu.vehdjk.com

Go:   func main()
来源：http://gfa.yvedp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mse.ybcxt.top

C#:   static void Main(string[] args)
来源：http://rha.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://mqu.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://pzd.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://zys.epnwcf.com

JS:   process.platform;  process.version
来源：http://kgl.pycfn.com

TS:   process.platform;  process.version
来源：http://qes.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ynr.hammf.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gvu.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xrg.yonumen.top


<!-- 参考信息 -->