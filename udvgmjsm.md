代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vtz.zycfv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mqo.jlsjyb.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rsb.yuanzhike.top

TS:   d.toISOString()
来源：http://fdz.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bao.aizwys.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wio.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vmv.nanxuanxn.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xvp.tianlin.xyz

[J03] 字符串解析为日期
来源：http://mni.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qyy.zdbjq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dpm.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://gyo.aizwys.cn

TS:   new Date("2024-01-02")
来源：http://mni.cqqwz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ggw.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fnj.yj20258888.top

Ruby: Date.parse("2024-01-02")
来源：http://qjg.zhijiandao.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xas.smart0.xyz

[J04] 时间戳与日期互转
来源：http://wmk.gotoacloud.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xzt.haohaochexian.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pfa.zhongyouzk.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bkv.zhijiandao.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ibq.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bti.jinqigfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nrq.hongshengwenyu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ina.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rzu.ydzc1.top

[J05] 时间加减（加 7 天）
来源：http://ikd.zhoulong.xyz

Py:   now + timedelta(days=7)
来源：http://utz.iojbl.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wnb.cashguo.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jzj.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fel.gaohongyu789.top

Java: LocalDate.now().plusDays(7)
来源：http://sps.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://isg.wangshuangyany.cn

Ruby: Time.now + 7 * 86400
来源：http://xfz.jqgfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://dsq.ybcxt.top

[J06] 计算两时间之差
来源：http://eta.cucudq.cn

Py:   (end - start).total_seconds()
来源：http://atn.quarkkingdee.top

PHP:  $end->diff($start)->days;
来源：http://isy.guannengcc.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mex.fktsv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yst.yj202588.top

Java: Duration.between(start, end).toSeconds()
来源：http://xjs.yuxming.cn

Go:   end.Sub(start).Hours()
来源：http://aoe.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://cni.cashguo.top

C#:   (end - start).TotalSeconds
来源：http://tme.feifeiyinyue.top

[J07] 比较两个日期
来源：http://syf.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://wqb.guannengcc.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zsj.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://jqj.yj202588.top

TS:   d1.getTime() < d2.getTime()
来源：http://amu.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://isc.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wsj.tanke756.top

Ruby: d1 < d2;  d1 == d2
来源：http://wzf.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://vlg.haohaochexian.top

[J08] 提取年月日与星期
来源：http://ojk.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mmu.daria6918.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tcp.yonumen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qdu.zhengqikj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://twv.ydjk.org.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vmm.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mvo.hywenlv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://elz.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bgs.meibo888.top

[J09] 时区处理
来源：http://mqx.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aob.jqgufenzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fzg.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ykr.sjlbkw.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uqe.gotoacloud.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vro.yj20258.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mdw.yvedp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zrp.hnxiangtu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ghm.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://kkj.ppjwa.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cjl.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kch.zhixingplan.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xza.yj20258.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nlw.nanxuanxn.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jml.9152youxi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oed.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gzf.gogol.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fco.jqgufenzy.top

================================================================================
来源：http://qks.jlsjyb.cn

K. JSON 与序列化
来源：http://few.jinqigufen.top

================================================================================
来源：http://iti.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://ouz.sufxvd.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lxb.c1oappe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iuh.guannengcc.top

JS:   JSON.stringify(obj)
来源：http://vgp.yueranfly.top

TS:   JSON.stringify(obj)
来源：http://kmm.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pzu.cashguo.top

Go:   json.Marshal(obj)
来源：http://snj.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://qcu.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jpx.epnwcf.com

[K02] JSON 字符串转对象
来源：http://pou.yuanzhike.top

Py:   json.loads(s)
来源：http://huv.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yhg.sysykeji.top

JS:   JSON.parse(s)
来源：http://obm.zhixingplan.top

TS:   JSON.parse(s)
来源：http://alo.yuanzhike.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dqy.iojbl.cn

Go:   json.Unmarshal(data, &v)
来源：http://mpm.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://vnx.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wwa.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://ouw.gotoacloud.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qts.52xcode.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ils.ppjwa.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lyy.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ept.zdbjq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zes.tian-w.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://use.dianchejie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xoh.guowangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pgi.zhixingplan.top

[K04] 读取 JSON 文件
来源：http://nbb.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qrr.nanxuanxn.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xri.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dto.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://chg.nanxuanxn.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gha.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aos.vehdjk.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://awd.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hkk.sxryk.cn

[K05] 深拷贝对象
来源：http://zuv.redwolf501.top

Py:   copy.deepcopy(obj)
来源：http://xne.wangdashe.top

PHP:  unserialize(serialize($obj));
来源：http://mhv.yvedp.cn

JS:   structuredClone(obj)
来源：http://qtm.c1oappe.top

TS:   structuredClone(obj)
来源：http://sjw.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://iko.fzhhl.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aca.sjlbkw.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://txd.jinqigufen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ojg.hnqzz.top

[K06] 解析 URL 查询串
来源：http://uqj.kuanghao11.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wwl.yangfankeji.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uuy.cucudq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uxl.snrcjt.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tgz.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bua.pengpengdd.cyou

Go:   url.ParseQuery("a=1&b=2")
来源：http://nwd.yj20258.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ofh.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aqy.chenzaomai.com

[K07] 进制转换
来源：http://mlc.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cpb.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wrj.zycfv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xql.hnxiangtu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bvg.zdqjudy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zwv.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uve.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jxe.hnqzz.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://egn.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://bft.jianghu66.top

Py:   pickle.dumps(obj)
来源：http://req.hfpthk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zyn.cqqwz.cn

JS:   v8.serialize(obj)        // Node
来源：http://qxy.yvedp.cn

TS:   v8.serialize(obj)        // Node
来源：http://faj.cheryme.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gih.bjfxy.top

Go:   encoding/gob
来源：http://opi.zdqjudy.top

Ruby: Marshal.dump(obj)
来源：http://bgp.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gba.zhijiandao.cn

================================================================================
来源：http://bnu.ybcxt.top

L. 网络请求
来源：http://sap.smart0.xyz

================================================================================
来源：http://rmp.ehwqpu.com

[L01] 发送 GET 请求
来源：http://lhd.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jbx.gaohongyu789.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kit.tian-w.cn

JS:   await fetch(url)
来源：http://djj.hammf.cn

TS:   await fetch(url)
来源：http://ipo.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rbv.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://sod.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nlj.redwolf501.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://flj.hcnkem.com

[L02] 发送 POST JSON
来源：http://jdn.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xjs.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xtu.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ivy.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kbi.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tpn.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sdn.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mvr.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rua.zhengqikj.top

[L03] 设置自定义请求头
来源：http://ird.sweek.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fhj.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://opl.hfpthk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ybv.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lky.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pgr.jyoumei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fcg.tianlin.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dsp.fehbvm.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fax.gzhubu.top

[L04] 设置超时
来源：http://irf.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://hvr.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zgy.hnqzz.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nsr.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lri.meibo888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bow.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fpm.snrcjt.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aby.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ntw.cqqwz.cn

[L05] 上传文件（multipart）
来源：http://qnk.ctjpmb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gfi.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pja.cashguo.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ngu.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dgf.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zqb.bjfxy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://syt.yvedp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vep.fengsongda.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ndt.jianghu66.top

[L06] 解析响应为 JSON
来源：http://qmh.cheryme.top

Py:   resp.json()
来源：http://jcx.daxiang520.top

PHP:  json_decode($body, true);
来源：http://kyk.fengsongda.top

JS:   await resp.json()
来源：http://gna.daxiang520.top

TS:   await resp.json()
来源：http://mgn.hammf.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wko.jinghuilouyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hjj.jinqigufen.top

Ruby: JSON.parse(resp.body)
来源：http://esm.wangshuangyany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vfq.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://isi.ehwqpu.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nye.xingfuxueyuan.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ghr.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://emm.guannengcc.top

TS:   resp.ok;  resp.status
来源：http://sys.aibaodan.cn

Java: resp.statusCode()
来源：http://idz.52xcode.cn

Go:   resp.StatusCode
来源：http://fto.sufxvd.cn

Ruby: resp.code.to_i
来源：http://spw.cqqwz.cn

C#:   (int)resp.StatusCode
来源：http://ohr.yonumen.top

[L08] 并发请求多个地址
来源：http://wyn.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gfd.jinqigufen.top

PHP:  curl_multi_init() 系列
来源：http://cqq.316326.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dkg.ydjk.org.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ucg.tanke756.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ayo.havefunace.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dvl.ctjpmb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wnz.havefunace.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://van.tanke756.top

================================================================================
来源：http://pzo.bbcook.cn

M. 命令行 / 进程 / 环境
来源：http://yhh.hnxiangtu.top

================================================================================
来源：http://och.guowangkeji.top

[M01] 读取命令行参数
来源：http://apw.epnwcf.com

Py:   sys.argv[1:]
来源：http://jiy.chenlongwang.top

PHP:  $argv;  $argc;
来源：http://rlx.hysaishi.cn

JS:   process.argv.slice(2)
来源：http://hrx.316326.xyz

TS:   process.argv.slice(2)
来源：http://zhc.zycfv.cn

Java: args 数组（main 方法参数）
来源：http://bqy.haohaochexian.top

Go:   os.Args[1:]
来源：http://vkx.ybcxt.top

Ruby: ARGV
来源：http://ubx.ppjwa.cn

C#:   args 数组（Main 方法参数）
来源：http://vdi.bjfxy.top

[M02] 读取环境变量
来源：http://fid.hysaishi.cn

Py:   os.environ.get("HOME")
来源：http://wwk.vqdsnc.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uxu.cashguo.top

JS:   process.env.HOME
来源：http://jec.epnwcf.com

TS:   process.env.HOME
来源：http://gfa.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://ayv.nanxuanxn.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mgf.hysaishi.cn

Ruby: ENV["HOME"]
来源：http://bxf.sufxvd.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://glp.yj20258.top

[M03] 执行外部命令
来源：http://yqk.ydzc1.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lkq.ydjk.org.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pyg.bbcook.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://itm.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://thy.fzhhl.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oqq.nanxinkj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fzg.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://rux.hcnkem.com

C#:   Process.Start("ls", "-l");
来源：http://jiw.snrcjt.cn

[M04] 获取当前工作目录
来源：http://qup.vqdsnc.cn

Py:   os.getcwd()
来源：http://ivo.hnqzz.top

PHP:  getcwd();
来源：http://lhk.zycfv.cn

JS:   process.cwd()
来源：http://oyg.feifeiyinyue.top

TS:   process.cwd()
来源：http://ueo.yj20258888.top

Java: Path.of("").toAbsolutePath()
来源：http://ytk.chenlongwang.top

Go:   os.Getwd()
来源：http://pmy.tian-w.cn

Ruby: Dir.pwd
来源：http://izj.ppjwa.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mar.xuetiantiany.cn

[M05] 设置退出码
来源：http://eii.vqdsnc.cn

Py:   sys.exit(1)
来源：http://tzs.bbcook.cn

PHP:  exit(1);
来源：http://glo.andypj.xyz

JS:   process.exit(1)
来源：http://ive.xylfe.cn

TS:   process.exit(1)
来源：http://ejx.sjlbkw.cn

Java: System.exit(1)
来源：http://ura.shuidangran.top

Go:   os.Exit(1)
来源：http://pqy.pycfn.com

Ruby: exit 1
来源：http://gye.zycfv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://aqm.hammf.cn

[M06] 向标准错误输出
来源：http://sxp.shuidangran.top

Py:   print("err", file=sys.stderr)
来源：http://daw.cashguo.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ngl.wangshuangyany.cn

JS:   console.error("err")
来源：http://fpp.gotoacloud.top

TS:   console.error("err")
来源：http://ymy.jinqigufen.top

Java: System.err.println("err")
来源：http://pxw.wangshuangyany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kve.gogol.net.cn

Ruby: warn "err"
来源：http://ynu.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://csw.epnwcf.com

[M07] 判断是否为主入口
来源：http://pta.hysaishi.cn

Py:   if __name__ == "__main__":
来源：http://zzm.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zqa.xuetiantiany.cn

JS:   require.main === module
来源：http://axp.tian-w.cn

TS:   require.main === module
来源：http://ezx.vqdsnc.cn

Java: public static void main(String[] args)
来源：http://ddo.tarul.cn

Go:   func main()
来源：http://pic.wangshuangyany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ewh.sweek.top

C#:   static void Main(string[] args)
来源：http://nfd.guowangkeji.top

[M08] 获取系统与运行时信息
来源：http://mmx.tian-w.cn

Py:   platform.system();  platform.python_version()
来源：http://vsi.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://dye.chenzaomai.com

JS:   process.platform;  process.version
来源：http://hof.fktsv.cn


<!-- 参考信息 -->