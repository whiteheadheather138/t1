代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://arz.nwbrower.top

TS:   /error/gim
来源：http://meu.yuxming.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jnf.ivvv.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xth.kuanghao11.cn

Ruby: s.scan(/error/i)
来源：http://gec.sysykeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wlq.hnxiangtu.top

[I08] 贪婪与非贪婪匹配
来源：http://edk.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dfs.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://reb.iojbl.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kkj.chenzaomai.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qdw.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lnq.chenjidiqi.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rnh.xuetiantiany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bjj.nwbrower.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hez.9152youxi.cn

================================================================================
来源：http://cyz.ivvv.top

J. 日期与时间
来源：http://zds.tanke756.top

================================================================================
来源：http://one.xylfe.cn

[J01] 获取当前时间
来源：http://bfq.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lyg.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yan.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://xqf.haohaochexian.top

TS:   new Date();  Date.now()
来源：http://mnz.ivvv.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lqx.ybcxt.top

Go:   time.Now()
来源：http://ysw.guannengcc.top

Ruby: Time.now
来源：http://eoy.guannengcc.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ihw.jinqigfzy.top

[J02] 格式化输出
来源：http://myc.xuetiantiany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fnq.wangshuangyany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uel.meibo888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xqi.zhongyouzk.top

TS:   d.toISOString()
来源：http://hem.zdbjq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gyu.jinghuilouyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xem.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://epg.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fdx.ybcxt.top

[J03] 字符串解析为日期
来源：http://zzp.ivvv.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hwb.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://szx.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://xum.sjlbkw.cn

TS:   new Date("2024-01-02")
来源：http://dht.yj202588.top

Java: LocalDate.parse("2024-01-02")
来源：http://ptr.shzxlz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iai.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://knz.kuanghao11.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://amb.0kj1m.cn

[J04] 时间戳与日期互转
来源：http://ihd.yanxiufei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qbf.zdqjudy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fcd.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vkv.jinghuilouyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vsr.fzhhl.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rac.zhiwuduotai.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xgb.iojbl.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xeo.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://koy.cqqwz.cn

[J05] 时间加减（加 7 天）
来源：http://tpx.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://fcc.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wgm.jlsjyb.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bjj.tianlin.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vmi.dashuyun.cn

Java: LocalDate.now().plusDays(7)
来源：http://syx.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tgt.nanxinkj.top

Ruby: Time.now + 7 * 86400
来源：http://gfv.zdbjq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://knz.sweek.top

[J06] 计算两时间之差
来源：http://rqu.sweek.top

Py:   (end - start).total_seconds()
来源：http://dja.hywenlv.cn

PHP:  $end->diff($start)->days;
来源：http://tkl.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nna.tianlin.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mjr.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vfq.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://dpj.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://oem.xuetiantiany.cn

C#:   (end - start).TotalSeconds
来源：http://emd.hnqzz.top

[J07] 比较两个日期
来源：http://idj.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://aob.zdbjq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uat.nanxuanxn.top

JS:   d1.getTime() < d2.getTime()
来源：http://myj.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://quo.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tti.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ifw.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://gkw.gzhubu.top

C#:   d1 < d2;  d1 == d2
来源：http://dcb.birdmap.top

[J08] 提取年月日与星期
来源：http://yym.yj20258.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://slj.shzxlz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fvv.ywan-chungtsiang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uxj.zdbjq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cvp.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pgt.kuanghao11.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xdw.9152youxi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ilt.vehdjk.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fcx.dianchejie.cn

[J09] 时区处理
来源：http://chz.fanxiaobao.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pmh.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sju.zhengqikj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xan.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aoc.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://coj.snrcjt.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mun.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://tbu.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cvr.jyoumei.cn

[J10] 取今天 / 本月第一天
来源：http://aqq.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ydm.chenzaomai.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aeu.yonumen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kfi.iojbl.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zzn.yanxiufei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hyt.shanyushiyangtech.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eth.fzhhl.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mua.yonumen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pto.tian-w.cn

================================================================================
来源：http://zwb.shzxlz.cn

K. JSON 与序列化
来源：http://flu.cqqwz.cn

================================================================================
来源：http://mqw.zhaomingkeji.xyz

[K01] 对象转 JSON 字符串
来源：http://mso.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oqu.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eug.cheryme.top

JS:   JSON.stringify(obj)
来源：http://azm.tarul.cn

TS:   JSON.stringify(obj)
来源：http://hzc.hongshengwenyu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oih.hesvh.cn

Go:   json.Marshal(obj)
来源：http://lxs.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mfk.yj20258.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uux.aibaodan.cn

[K02] JSON 字符串转对象
来源：http://xkm.zdqjudy.top

Py:   json.loads(s)
来源：http://vjn.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yyp.yvedp.cn

JS:   JSON.parse(s)
来源：http://fow.nanxinkj.top

TS:   JSON.parse(s)
来源：http://adk.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ziz.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://lxo.wangdashe.top

Ruby: JSON.parse(s)
来源：http://kqr.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nor.vqdsnc.cn

[K03] JSON 美化输出（带缩进）
来源：http://vwy.ehwqpu.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cef.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eol.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://bas.jqgfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nmv.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mgz.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eax.bbcook.cn

Ruby: JSON.pretty_generate(obj)
来源：http://axc.chenlongwang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qlk.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://ize.hcnkem.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://feb.guowangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vuw.dianchejie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iuh.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kfo.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ipd.ehwqpu.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://avi.jyoumei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bhr.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mmu.ydjk.org.cn

[K05] 深拷贝对象
来源：http://kok.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://tnm.fanxiaobao.xyz

PHP:  unserialize(serialize($obj));
来源：http://pxh.shzxlz.cn

JS:   structuredClone(obj)
来源：http://tnl.fktsv.cn

TS:   structuredClone(obj)
来源：http://vle.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://zyp.hnqzz.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xxi.daxiang520.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vki.yongpay.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pys.cqqwz.cn

[K06] 解析 URL 查询串
来源：http://vcx.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jne.xingfuxueyuan.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sjg.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rrz.fktsv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tnw.ydzc1.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wes.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rbh.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://alv.fanxiaobao.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tmk.zdqjudy.top

[K07] 进制转换
来源：http://xju.hcnkem.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fgy.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yig.jyoumei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ljy.hammf.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sfz.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jca.cashguo.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mcy.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wpc.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cqm.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://agb.jiagoushi.top

Py:   pickle.dumps(obj)
来源：http://lys.0kj1m.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vvk.tianlin.xyz

JS:   v8.serialize(obj)        // Node
来源：http://lav.wangshuangyany.cn

TS:   v8.serialize(obj)        // Node
来源：http://tyt.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://crg.wangdashe.top

Go:   encoding/gob
来源：http://npi.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://dtz.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://crq.shzxlz.cn

================================================================================
来源：http://hzu.zdbjq.cn

L. 网络请求
来源：http://zzf.guannengcc.top

================================================================================
来源：http://rca.jqgufenzy.top

[L01] 发送 GET 请求
来源：http://nwt.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nwi.redwolf501.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xpj.sysykeji.top

JS:   await fetch(url)
来源：http://svt.shuidangran.top

TS:   await fetch(url)
来源：http://hht.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vjo.sweek.top

Go:   resp, err := http.Get(url)
来源：http://wtn.tanke756.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bjw.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://emm.shzxlz.cn

[L02] 发送 POST JSON
来源：http://iex.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jdl.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ezx.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lye.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ajj.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aia.jiagoushi.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iit.zycfv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://efe.cucudq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xbb.zhoulong.xyz

[L03] 设置自定义请求头
来源：http://xmw.fzhhl.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hfc.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wtm.hcnkem.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pfv.jqgfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://diy.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dwz.yj20258.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vgj.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://duj.xingfuxueyuan.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dpy.sxryk.cn

[L04] 设置超时
来源：http://rsb.jlsjyb.cn

Py:   requests.get(url, timeout=5)
来源：http://nov.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://leu.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ggr.yj20258.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kmx.yongpay.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kmj.sjlbkw.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://udx.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sqi.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jww.aizwys.cn

[L05] 上传文件（multipart）
来源：http://qsj.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://klu.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xgv.cashguo.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tgi.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yct.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oew.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jru.epnwcf.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tsq.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ckd.shanyushiyangtech.top

[L06] 解析响应为 JSON
来源：http://yix.wangshuangyany.cn

Py:   resp.json()
来源：http://gma.hesvh.cn

PHP:  json_decode($body, true);
来源：http://wmu.chenlongwang.top

JS:   await resp.json()
来源：http://gpe.jqgufenzy.top

TS:   await resp.json()
来源：http://eeg.hfpthk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vko.cucudq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nff.xuanzx.com

Ruby: JSON.parse(resp.body)
来源：http://twq.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zrw.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://joy.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sdx.yueranfly.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ldi.316326.xyz

JS:   resp.ok;  resp.status
来源：http://pwf.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://zey.vehdjk.com

Java: resp.statusCode()
来源：http://dex.pycfn.com

Go:   resp.StatusCode
来源：http://pxs.aibaodan.cn

Ruby: resp.code.to_i
来源：http://whd.shuidangran.top

C#:   (int)resp.StatusCode
来源：http://bbr.yfazqb.com

[L08] 并发请求多个地址
来源：http://fqh.gogol.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wiw.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://oun.jqgufenzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jza.guannengcc.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jau.bbcook.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vzi.yongpay.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kse.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ctd.ppjwa.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ccj.hammf.cn

================================================================================
来源：http://vxt.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://gab.daxiang520.top

================================================================================
来源：http://awm.vehdjk.com

[M01] 读取命令行参数
来源：http://hnt.ppjwa.cn

Py:   sys.argv[1:]
来源：http://sxg.fanxiaobao.xyz

PHP:  $argv;  $argc;
来源：http://wrd.hnqzz.top

JS:   process.argv.slice(2)
来源：http://iaz.guowangkeji.top

TS:   process.argv.slice(2)
来源：http://trg.zhengqikj.top

Java: args 数组（main 方法参数）
来源：http://vuf.ydjk.org.cn

Go:   os.Args[1:]
来源：http://hkz.jlsjyb.cn

Ruby: ARGV
来源：http://dyw.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://vxq.tanke756.top

[M02] 读取环境变量
来源：http://ame.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://twx.shanyushiyangtech.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yuh.zycfv.cn

JS:   process.env.HOME
来源：http://rvy.ehwqpu.com

TS:   process.env.HOME
来源：http://ics.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://dkn.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tlb.jinqigufen.top

Ruby: ENV["HOME"]
来源：http://yar.jqgufenzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mdc.yueranfly.top

[M03] 执行外部命令
来源：http://zju.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lkj.tarul.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wvs.jiagoushi.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cvd.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tgq.gotoacloud.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lah.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lnz.ybcxt.top

Ruby: system("ls -l");  `ls -l`
来源：http://gya.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://gds.xziqi.cn

[M04] 获取当前工作目录
来源：http://njd.cdnleiting.top

Py:   os.getcwd()
来源：http://fpx.xuanzx.com

PHP:  getcwd();
来源：http://zhl.daria6918.cn

JS:   process.cwd()
来源：http://fhq.9152youxi.cn

TS:   process.cwd()
来源：http://ufb.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://gfu.vehdjk.com

Go:   os.Getwd()
来源：http://ueg.bjfxy.top

Ruby: Dir.pwd
来源：http://uer.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hql.haohaochexian.top

[M05] 设置退出码
来源：http://npf.yj20258888.top

Py:   sys.exit(1)
来源：http://ubl.chenjidiqi.icu

PHP:  exit(1);
来源：http://gam.tianlin.xyz


<!-- 参考信息 -->