代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://enn.yangfankeji.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iug.yj20258.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://isg.hnxiangtu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://snd.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ewe.hfpthk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://obh.tian-w.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wdu.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tag.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hhw.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://ygr.yj202588.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xdy.zhoulong.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vsj.gaohongyu789.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ndc.gotoacloud.top

TS:   /error/gim
来源：http://qlh.cashguo.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zwg.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ghc.jinyuanbaomall.cn

Ruby: s.scan(/error/i)
来源：http://otq.cqqwz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qul.gogol.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://hkh.ybcxt.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hji.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aiv.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bhz.tianlin.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wcx.feifeiyinyue.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wco.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gal.hnqzz.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qqj.jinghuilouyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://htd.zhixingplan.top

================================================================================
来源：http://mqa.sufxvd.cn

J. 日期与时间
来源：http://kfp.tianlin.xyz

================================================================================
来源：http://ztl.xziqi.cn

[J01] 获取当前时间
来源：http://ips.tian-w.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aqc.chenjidiqi.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yap.dashuyun.cn

JS:   new Date();  Date.now()
来源：http://fwl.redwolf501.top

TS:   new Date();  Date.now()
来源：http://hxy.jinqigfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://juz.zdbjq.cn

Go:   time.Now()
来源：http://qkp.sysykeji.top

Ruby: Time.now
来源：http://sln.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lpa.nwbrower.top

[J02] 格式化输出
来源：http://nby.yueranfly.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jzd.cheryme.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xok.zhixingplan.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wpv.meibo888.top

TS:   d.toISOString()
来源：http://zqj.chenjidiqi.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://spw.zhijiandao.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hei.jinqigufen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cgf.jlsjyb.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://glq.c1oappe.top

[J03] 字符串解析为日期
来源：http://tel.tianlin.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cst.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://akw.ydjk.org.cn

JS:   new Date("2024-01-02")
来源：http://ljm.cucudq.cn

TS:   new Date("2024-01-02")
来源：http://hhx.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qop.pycfn.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cdx.bjfxy.top

Ruby: Date.parse("2024-01-02")
来源：http://ako.kuanghao11.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fdi.yonumen.top

[J04] 时间戳与日期互转
来源：http://qnz.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qiy.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zik.tarul.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ubs.zhongyouzk.top

TS:   Math.floor(Date.now() / 1000)
来源：http://oyn.ywan-chungtsiang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iyz.zhiwuduotai.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zik.zhiwuduotai.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jck.xingfuxueyuan.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ilz.vehdjk.com

[J05] 时间加减（加 7 天）
来源：http://bri.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://ent.xingfuxueyuan.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://mfw.shangyingyoupin.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pzs.zhiwuduotai.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oar.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://lle.9152youxi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lav.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://ymd.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://lum.zhongyouzk.top

[J06] 计算两时间之差
来源：http://gcj.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://byq.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://ixl.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://may.fengsongda.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hxd.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rmz.zhoulong.xyz

Go:   end.Sub(start).Hours()
来源：http://kya.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://eow.shangyingyoupin.top

C#:   (end - start).TotalSeconds
来源：http://bqo.jqgfzy.top

[J07] 比较两个日期
来源：http://tkh.jqgfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://rkn.mhx1999.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sif.hfpthk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ppi.zhongyouzk.top

TS:   d1.getTime() < d2.getTime()
来源：http://izc.gotoacloud.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gvu.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kru.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://pvf.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://ouk.cqqwz.cn

[J08] 提取年月日与星期
来源：http://ter.jinyuanbaomall.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://atn.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://txo.316326.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bhe.jqgufenzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ydk.bbcook.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gsd.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ysa.zycfv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dne.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gpv.gzhubu.top

[J09] 时区处理
来源：http://lwb.shuidangran.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://low.yfazqb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kpr.cdnleiting.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lpj.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ymh.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://muv.chenjidiqi.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gei.jinqigufen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ipb.ydjk.org.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hfj.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://bvl.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://xdf.ydjk.org.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dwz.chenlongwang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xgg.9152youxi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dzg.jianghu66.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ejj.aibaodan.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://svu.zhongyouzk.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://awp.jinyuanbaomall.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yfm.9152youxi.cn

================================================================================
来源：http://esv.yanxiufei.cn

K. JSON 与序列化
来源：http://cui.jinyuanbaomall.cn

================================================================================
来源：http://glb.epnwcf.com

[K01] 对象转 JSON 字符串
来源：http://ysx.hnqzz.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nwh.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tqk.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://aut.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://ktd.xuetiantiany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vbb.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://nfv.52xcode.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mhs.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fms.epnwcf.com

[K02] JSON 字符串转对象
来源：http://iub.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://gvf.fehbvm.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://prn.ybcxt.top

JS:   JSON.parse(s)
来源：http://wrn.jianghu66.top

TS:   JSON.parse(s)
来源：http://alb.xuetiantiany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zfd.ehwqpu.com

Go:   json.Unmarshal(data, &v)
来源：http://ela.xinyue.icu

Ruby: JSON.parse(s)
来源：http://ydg.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ecm.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://muz.zhixingplan.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hbt.yvedp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://job.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nfy.hammf.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mim.xinyue.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cwa.cdnleiting.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bdw.yj20258.top

Ruby: JSON.pretty_generate(obj)
来源：http://fkv.uphjek.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oqf.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://squ.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bjl.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wxi.9152youxi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bfe.redwolf501.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://osx.kuanghao11.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nrb.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://okn.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ryh.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pdx.ivvv.top

[K05] 深拷贝对象
来源：http://elb.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://cgk.ybcxt.top

PHP:  unserialize(serialize($obj));
来源：http://lqh.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://slm.chenjidiqi.icu

TS:   structuredClone(obj)
来源：http://gpo.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ubt.yonumen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pbm.bjfxy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dpa.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ehk.yvedp.cn

[K06] 解析 URL 查询串
来源：http://msa.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lsl.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pox.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cbv.jqgufenzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://woj.nwbrower.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gct.guowangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jsv.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jvg.uphjek.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ldj.daxiang520.top

[K07] 进制转换
来源：http://dze.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kqj.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mpt.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://spm.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wqi.smart0.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vna.yj20258888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qnu.jinghuilouyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ngy.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nti.daria6918.cn

[K08] 二进制序列化（非 JSON）
来源：http://ejd.shanyushiyangkeji.top

Py:   pickle.dumps(obj)
来源：http://gjk.aibaodan.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gdx.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://oqd.epnwcf.com

TS:   v8.serialize(obj)        // Node
来源：http://ymh.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://etu.zycfv.cn

Go:   encoding/gob
来源：http://wtz.xziqi.cn

Ruby: Marshal.dump(obj)
来源：http://yqc.xylfe.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pry.hnxiangtu.top

================================================================================
来源：http://mns.ydzc1.top

L. 网络请求
来源：http://qti.guowangkeji.top

================================================================================
来源：http://ltk.hcnkem.com

[L01] 发送 GET 请求
来源：http://myv.xinyue.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mby.sjlbkw.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vcy.dashuyun.cn

JS:   await fetch(url)
来源：http://fex.zhengqikj.top

TS:   await fetch(url)
来源：http://xch.chenzaomai.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jpp.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://bip.fehbvm.com

Ruby: Net::HTTP.get(URI(url))
来源：http://chq.cucudq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qpd.pycfn.com

[L02] 发送 POST JSON
来源：http://snk.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://sxt.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bvw.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://axm.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cjs.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ccl.sweek.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tys.fzhhl.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lse.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dgf.ybcxt.top

[L03] 设置自定义请求头
来源：http://pbm.shzxlz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sek.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rba.yangfankeji.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oir.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jus.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ipd.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mmw.zhaomingkeji.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zta.cqqwz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iqz.fehbvm.com

[L04] 设置超时
来源：http://xmw.fktsv.cn

Py:   requests.get(url, timeout=5)
来源：http://imo.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hsj.yvedp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ycn.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ygb.redwolf501.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hct.zdqjudy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ygv.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yxh.daria6918.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://akz.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://ewh.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://psi.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ced.hesvh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gmo.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xwa.cqqwz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ocm.jinyuanbaomall.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yzx.daxiang520.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ioz.cucudq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iaq.yj202588.top

[L06] 解析响应为 JSON
来源：http://gbv.yonumen.top

Py:   resp.json()
来源：http://tpu.shanyushiyangkeji.top

PHP:  json_decode($body, true);
来源：http://tdb.dianchejie.cn

JS:   await resp.json()
来源：http://tdb.zycfv.cn

TS:   await resp.json()
来源：http://weq.hfpthk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://auw.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tcy.tanke756.top

Ruby: JSON.parse(resp.body)
来源：http://own.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wef.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://tda.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qej.zhongyouzk.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fcy.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://ygf.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://sbb.hongshengwenyu.top

Java: resp.statusCode()
来源：http://wwa.zhiwuduotai.top

Go:   resp.StatusCode
来源：http://lnc.jiagoushi.top

Ruby: resp.code.to_i
来源：http://osi.tarul.cn

C#:   (int)resp.StatusCode
来源：http://xrk.vqdsnc.cn

[L08] 并发请求多个地址
来源：http://uys.jinghuilouyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://som.bjfxy.top

PHP:  curl_multi_init() 系列
来源：http://sue.xylfe.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ccb.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zwu.ydjk.org.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lya.haohaochexian.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yug.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cwc.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lki.zdbjq.cn

================================================================================
来源：http://qzb.andypj.xyz

M. 命令行 / 进程 / 环境
来源：http://grw.sufxvd.cn

================================================================================
来源：http://hsf.yj20258888.top

[M01] 读取命令行参数
来源：http://fut.cheryme.top

Py:   sys.argv[1:]
来源：http://qck.zhongyouzk.top

PHP:  $argv;  $argc;
来源：http://nqe.tian-w.cn

JS:   process.argv.slice(2)
来源：http://bdx.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://cqk.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://ncn.shangyingyoupin.top

Go:   os.Args[1:]
来源：http://otj.cheryme.top

Ruby: ARGV
来源：http://dvi.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://zpk.sysykeji.top

[M02] 读取环境变量
来源：http://cco.yj20258.top

Py:   os.environ.get("HOME")
来源：http://ddy.sxryk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xby.zhiwuduotai.top

JS:   process.env.HOME
来源：http://otw.guannengcc.top

TS:   process.env.HOME
来源：http://xcn.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://xir.bjfxy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bfx.jqgfzy.top

Ruby: ENV["HOME"]
来源：http://cqb.yongpay.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cwc.aizwys.cn

[M03] 执行外部命令
来源：http://xkk.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lxx.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hwk.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://kfr.yonumen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xdt.aibaodan.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vrh.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://odm.nanxinkj.top

Ruby: system("ls -l");  `ls -l`
来源：http://pjy.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://oft.fzhhl.top


<!-- 参考信息 -->