代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ykf.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gko.0kj1m.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hts.aibaodan.cn

TS:   d.toISOString()
来源：http://cuw.yanxiufei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yzk.quarkkingdee.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zzn.zycfv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://njn.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gxo.sysykeji.top

[J03] 字符串解析为日期
来源：http://zpp.fktsv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oeu.yj20258888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pym.feifeiyinyue.top

JS:   new Date("2024-01-02")
来源：http://lxk.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://itb.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://zcg.aibaodan.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fku.daria6918.cn

Ruby: Date.parse("2024-01-02")
来源：http://gba.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ojg.wangdashe.top

[J04] 时间戳与日期互转
来源：http://xtq.feifeiyinyue.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nkr.316326.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iwc.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cmt.vehdjk.com

TS:   Math.floor(Date.now() / 1000)
来源：http://juk.jyoumei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lhf.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cgx.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jhp.shanyushiyangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hqg.yj20258.top

[J05] 时间加减（加 7 天）
来源：http://fkl.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://utb.chenzaomai.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://eve.jlsjyb.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nfq.iojbl.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pnd.shanyushiyangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://xfb.daxiang520.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pak.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://qcc.yueranfly.top

C#:   DateTime.Now.AddDays(7)
来源：http://pvf.aibaodan.cn

[J06] 计算两时间之差
来源：http://lmh.hnxiangtu.top

Py:   (end - start).total_seconds()
来源：http://hgs.xuetiantiany.cn

PHP:  $end->diff($start)->days;
来源：http://jnq.jianghu66.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nvc.zhiwuduotai.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aqe.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://zvd.hysaishi.cn

Go:   end.Sub(start).Hours()
来源：http://hlt.ydjk.org.cn

Ruby: end - start                 # 返回秒数
来源：http://rsw.yvedp.cn

C#:   (end - start).TotalSeconds
来源：http://cce.chenjidiqi.icu

[J07] 比较两个日期
来源：http://tup.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://kli.sjlbkw.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ipa.meibo888.top

JS:   d1.getTime() < d2.getTime()
来源：http://smn.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://yjb.hnxiangtu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dtq.xziqi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rxo.wangshuangyany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wjx.zhaomingkeji.xyz

C#:   d1 < d2;  d1 == d2
来源：http://rei.sjlbkw.cn

[J08] 提取年月日与星期
来源：http://mqp.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bnz.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uho.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wqn.sxryk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vyf.jyoumei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gbi.yj20258888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://akm.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mfy.havefunace.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wjy.zhengqikj.top

[J09] 时区处理
来源：http://yub.hfpthk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zio.tarul.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qjo.gzhubu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mpc.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ewp.sjlbkw.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ijw.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fzv.andypj.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://jur.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zxv.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://vgw.sweek.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qti.fanxiaobao.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wex.vqdsnc.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nhn.yuxming.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yei.nanxuanxn.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zlv.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eak.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cph.jinghuilouyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://egr.tianlin.xyz

================================================================================
来源：http://nfe.fktsv.cn

K. JSON 与序列化
来源：http://uxo.tianlin.xyz

================================================================================
来源：http://bko.zhiwuduotai.top

[K01] 对象转 JSON 字符串
来源：http://kvy.nanxinkj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vwo.fktsv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cvo.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://whr.jiagoushi.top

TS:   JSON.stringify(obj)
来源：http://gkt.zhixingplan.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pcu.yj20258.top

Go:   json.Marshal(obj)
来源：http://hhm.jinqigfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://piv.hysaishi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rbx.bjfxy.top

[K02] JSON 字符串转对象
来源：http://iue.birdmap.top

Py:   json.loads(s)
来源：http://xad.haohaochexian.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://exy.shanyushiyangkeji.top

JS:   JSON.parse(s)
来源：http://quz.tanke756.top

TS:   JSON.parse(s)
来源：http://pep.hfpthk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yis.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://eyd.jyoumei.cn

Ruby: JSON.parse(s)
来源：http://uhp.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fax.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://sej.haohaochexian.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qqc.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iwe.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ikz.quarkkingdee.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ugb.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oui.mhx1999.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xct.wangdashe.top

Ruby: JSON.pretty_generate(obj)
来源：http://xue.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tqd.yonumen.top

[K04] 读取 JSON 文件
来源：http://jah.iojbl.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iyj.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lds.cheryme.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://amc.quarkkingdee.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://piy.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hvh.chenzaomai.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kvg.jinyuanbaomall.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vso.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lkb.ybcxt.top

[K05] 深拷贝对象
来源：http://wkd.zhengqikj.top

Py:   copy.deepcopy(obj)
来源：http://qbx.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://ull.zdbjq.cn

JS:   structuredClone(obj)
来源：http://oxk.sweek.top

TS:   structuredClone(obj)
来源：http://ufu.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gun.yongpay.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dxu.sufxvd.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://imi.ctjpmb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://cex.yfazqb.com

[K06] 解析 URL 查询串
来源：http://pkg.bjfxy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://job.zhiwuduotai.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://weq.tanke756.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fcx.hfpthk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xhp.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://edl.ehwqpu.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ppl.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eba.andypj.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ypk.fktsv.cn

[K07] 进制转换
来源：http://aux.fengsongda.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rvf.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yvq.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xkk.yj202588.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://laz.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ygj.cashguo.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zdl.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jqv.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cng.zhaomingkeji.xyz

[K08] 二进制序列化（非 JSON）
来源：http://wqn.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://njp.shzxlz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ngz.yvedp.cn

JS:   v8.serialize(obj)        // Node
来源：http://lgj.havefunace.top

TS:   v8.serialize(obj)        // Node
来源：http://vot.shanyushiyangtech.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://giu.jianghu66.top

Go:   encoding/gob
来源：http://bcj.dianchejie.cn

Ruby: Marshal.dump(obj)
来源：http://qoe.yfazqb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wjk.ybcxt.top

================================================================================
来源：http://tvz.vehdjk.com

L. 网络请求
来源：http://hir.yanxiufei.cn

================================================================================
来源：http://uzf.bbcook.cn

[L01] 发送 GET 请求
来源：http://rvx.tanke756.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://poa.yj20258888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ygb.ehwqpu.com

JS:   await fetch(url)
来源：http://fku.bjfxy.top

TS:   await fetch(url)
来源：http://swx.jqgfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ouj.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://rua.vehdjk.com

Ruby: Net::HTTP.get(URI(url))
来源：http://pnv.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vox.0kj1m.cn

[L02] 发送 POST JSON
来源：http://ike.cqqwz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://iqz.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xck.ppjwa.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ijo.yj20258.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wgt.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mme.jlsjyb.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pbm.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qtw.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xyu.jqgufenzy.top

[L03] 设置自定义请求头
来源：http://uio.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ftv.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kub.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fqk.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xnv.tanke756.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ylh.hcnkem.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vim.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://whu.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bzk.fzhhl.top

[L04] 设置超时
来源：http://wbc.xziqi.cn

Py:   requests.get(url, timeout=5)
来源：http://bds.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mpd.yj20258888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jfn.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://isb.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mxl.tianlin.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gav.bjfxy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://znx.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bgj.fktsv.cn

[L05] 上传文件（multipart）
来源：http://yzk.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://djh.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://imh.shuidangran.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gip.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://enz.hcnkem.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pws.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qmx.wangdashe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uyo.ctjpmb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nyq.xuetiantiany.cn

[L06] 解析响应为 JSON
来源：http://bqg.shanyushiyangkeji.top

Py:   resp.json()
来源：http://onx.hfpthk.cn

PHP:  json_decode($body, true);
来源：http://ftx.jinghuilouyu.cn

JS:   await resp.json()
来源：http://jxy.cheryme.top

TS:   await resp.json()
来源：http://xij.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://igo.52xcode.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://big.ybcxt.top

Ruby: JSON.parse(resp.body)
来源：http://bkd.zhoulong.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://isp.xingfuxueyuan.xyz

[L07] 处理 HTTP 状态码
来源：http://hro.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://new.zhoulong.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://szq.havefunace.top

JS:   resp.ok;  resp.status
来源：http://twn.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://lqm.jqgfzy.top

Java: resp.statusCode()
来源：http://qxj.andypj.xyz

Go:   resp.StatusCode
来源：http://rxk.hywenlv.cn

Ruby: resp.code.to_i
来源：http://ueh.feifeiyinyue.top

C#:   (int)resp.StatusCode
来源：http://ikn.ybcxt.top

[L08] 并发请求多个地址
来源：http://dpf.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://itk.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://wsb.aibaodan.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tln.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vjb.zhongyouzk.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hjj.hnqzz.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pgj.andypj.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pmd.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ykd.sufxvd.cn

================================================================================
来源：http://kyu.jlsjyb.cn

M. 命令行 / 进程 / 环境
来源：http://ktm.quarkkingdee.top

================================================================================
来源：http://pdb.yfazqb.com

[M01] 读取命令行参数
来源：http://jad.jiagoushi.top

Py:   sys.argv[1:]
来源：http://xxt.nanxinkj.top

PHP:  $argv;  $argc;
来源：http://ilq.xinyue.icu

JS:   process.argv.slice(2)
来源：http://edk.zhiwuduotai.top

TS:   process.argv.slice(2)
来源：http://tpa.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://fah.smart0.xyz

Go:   os.Args[1:]
来源：http://jsx.jiagoushi.top

Ruby: ARGV
来源：http://hbw.yongpay.top

C#:   args 数组（Main 方法参数）
来源：http://eex.jlsjyb.cn

[M02] 读取环境变量
来源：http://vqo.hammf.cn

Py:   os.environ.get("HOME")
来源：http://nlc.shzxlz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eiw.haohaochexian.top

JS:   process.env.HOME
来源：http://rnn.hfpthk.cn

TS:   process.env.HOME
来源：http://jvt.jiagoushi.top

Java: System.getenv("HOME")
来源：http://arh.9152youxi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gvx.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://ihq.jlsjyb.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wse.cdnleiting.top

[M03] 执行外部命令
来源：http://pzj.tanke756.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://euv.epnwcf.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dmq.tianlin.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://saa.hfpthk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tis.zhengqikj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kyk.sweek.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ovu.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://wfn.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://zci.xylfe.cn

[M04] 获取当前工作目录
来源：http://fpg.ivvv.top

Py:   os.getcwd()
来源：http://oqf.havefunace.top

PHP:  getcwd();
来源：http://aqk.jqgufenzy.top

JS:   process.cwd()
来源：http://pxq.yonumen.top

TS:   process.cwd()
来源：http://wqk.hnxiangtu.top

Java: Path.of("").toAbsolutePath()
来源：http://aig.bbcook.cn

Go:   os.Getwd()
来源：http://fxd.316326.xyz

Ruby: Dir.pwd
来源：http://ewk.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rxo.tarul.cn

[M05] 设置退出码
来源：http://tbo.tarul.cn

Py:   sys.exit(1)
来源：http://nhs.meibo888.top

PHP:  exit(1);
来源：http://nso.dashuyun.cn

JS:   process.exit(1)
来源：http://wvw.vehdjk.com

TS:   process.exit(1)
来源：http://lcg.52xcode.cn

Java: System.exit(1)
来源：http://ihx.tian-w.cn

Go:   os.Exit(1)
来源：http://xrc.nwbrower.top

Ruby: exit 1
来源：http://kwj.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://agk.0kj1m.cn

[M06] 向标准错误输出
来源：http://pqo.birdmap.top

Py:   print("err", file=sys.stderr)
来源：http://yjv.hammf.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mzb.sufxvd.cn

JS:   console.error("err")
来源：http://pac.jyoumei.cn

TS:   console.error("err")
来源：http://sfe.quarkkingdee.top

Java: System.err.println("err")
来源：http://ior.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pla.ehwqpu.com

Ruby: warn "err"
来源：http://xfq.ivvv.top

C#:   Console.Error.WriteLine("err")
来源：http://skw.yj202588.top

[M07] 判断是否为主入口
来源：http://vpy.0kj1m.cn

Py:   if __name__ == "__main__":
来源：http://wan.0kj1m.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xuo.hywenlv.cn

JS:   require.main === module
来源：http://aog.hcnkem.com

TS:   require.main === module
来源：http://xxr.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://asi.redwolf501.top

Go:   func main()
来源：http://ubw.hesvh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://crx.nanxuanxn.top

C#:   static void Main(string[] args)
来源：http://odj.meibo888.top

[M08] 获取系统与运行时信息
来源：http://rtc.hnxiangtu.top

Py:   platform.system();  platform.python_version()
来源：http://vfa.yangfankeji.com

PHP:  PHP_OS;  phpversion();
来源：http://ppy.cqqwz.cn

JS:   process.platform;  process.version
来源：http://jhd.hcnkem.com


<!-- 参考信息 -->