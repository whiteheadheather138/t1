代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://urm.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yxt.hywenlv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lnk.chenlongwang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mjv.hfpthk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xts.9152youxi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mbg.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rrr.yvedp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dww.9152youxi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pov.jqgfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mwq.mhx1999.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uvw.iojbl.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sub.hywenlv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gdg.yuxming.cn

[I07] 忽略大小写与多行模式
来源：http://gwt.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qlv.yvedp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rne.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zwm.xziqi.cn

TS:   /error/gim
来源：http://xho.jlsjyb.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://udv.chenjidiqi.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eja.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://ptm.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nth.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://zlc.smart0.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pgt.wangshuangyany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dei.svipenyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eml.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cqr.ivvv.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wbs.cucudq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gys.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bju.cashguo.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://you.aizwys.cn

================================================================================
来源：http://bgf.wangdashe.top

J. 日期与时间
来源：http://eyv.smart0.xyz

================================================================================
来源：http://prz.yonumen.top

[J01] 获取当前时间
来源：http://okl.xuanzx.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://orr.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bdx.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://bnv.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://pro.nanxinkj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ioa.ybcxt.top

Go:   time.Now()
来源：http://ugk.yonumen.top

Ruby: Time.now
来源：http://plz.epnwcf.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cog.fehbvm.com

[J02] 格式化输出
来源：http://zrz.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://shx.gogol.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ncq.jinghuilouyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ona.nanxinkj.top

TS:   d.toISOString()
来源：http://qzb.zhoulong.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pfn.shuidangran.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xif.sufxvd.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tuz.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dja.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://nus.pengpengdd.cyou

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fru.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dmi.cashguo.top

JS:   new Date("2024-01-02")
来源：http://mke.yangfankeji.com

TS:   new Date("2024-01-02")
来源：http://irr.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tga.hfpthk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nvh.zhongyouzk.top

Ruby: Date.parse("2024-01-02")
来源：http://yji.zhaomingkeji.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lib.sxryk.cn

[J04] 时间戳与日期互转
来源：http://ods.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ync.ppjwa.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xwx.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qbc.daxiang520.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kvm.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qel.wangshuangyany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pnz.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ovi.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xft.aibaodan.cn

[J05] 时间加减（加 7 天）
来源：http://vhv.hfpthk.cn

Py:   now + timedelta(days=7)
来源：http://gyo.hongshengwenyu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jul.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bxd.wangdashe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mys.svipenyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://vnu.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vdw.yj20258.top

Ruby: Time.now + 7 * 86400
来源：http://bia.zycfv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ssf.redwolf501.top

[J06] 计算两时间之差
来源：http://ejg.zhijiandao.cn

Py:   (end - start).total_seconds()
来源：http://xrc.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://ikc.hongshengwenyu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xww.9152youxi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pja.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://pmo.pengpengdd.cyou

Go:   end.Sub(start).Hours()
来源：http://cbq.yj202588.top

Ruby: end - start                 # 返回秒数
来源：http://qdg.9152youxi.cn

C#:   (end - start).TotalSeconds
来源：http://dgf.xziqi.cn

[J07] 比较两个日期
来源：http://qwv.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://hsx.havefunace.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ife.hnqzz.top

JS:   d1.getTime() < d2.getTime()
来源：http://fif.nanxinkj.top

TS:   d1.getTime() < d2.getTime()
来源：http://fzf.nwbrower.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uvw.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mel.bjfxy.top

Ruby: d1 < d2;  d1 == d2
来源：http://gcd.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://och.yj202588.top

[J08] 提取年月日与星期
来源：http://myy.ivvv.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://obg.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zll.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xnr.hywenlv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ncl.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ixh.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://thj.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://btf.aizwys.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bmf.gotoacloud.top

[J09] 时区处理
来源：http://ptb.jqgufenzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yyj.smart0.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cia.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ffv.hfpthk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ube.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ozs.sjlbkw.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jgk.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kdv.vqdsnc.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://swa.ydzc1.top

[J10] 取今天 / 本月第一天
来源：http://nig.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qtd.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yvm.zycfv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uzo.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lmg.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pmi.yuxming.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qzi.cheryme.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bwi.birdmap.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ltf.jlsjyb.cn

================================================================================
来源：http://ozl.hfpthk.cn

K. JSON 与序列化
来源：http://kfg.nanxuanxn.top

================================================================================
来源：http://izp.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://chi.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mbc.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://faf.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://ipg.jinqigufen.top

TS:   JSON.stringify(obj)
来源：http://jby.tian-w.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mai.zhijiandao.cn

Go:   json.Marshal(obj)
来源：http://eez.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ihf.svipenyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://htw.gotoacloud.top

[K02] JSON 字符串转对象
来源：http://fzw.smart0.xyz

Py:   json.loads(s)
来源：http://wmf.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qql.ehwqpu.com

JS:   JSON.parse(s)
来源：http://dhx.yangfankeji.com

TS:   JSON.parse(s)
来源：http://glr.quarkkingdee.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://czt.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://sro.jiagoushi.top

Ruby: JSON.parse(s)
来源：http://wfr.jqgufenzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pby.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://gzr.guannengcc.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blu.tian-w.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oqp.hywenlv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fnq.feifeiyinyue.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vfi.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qap.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dvv.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vhx.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kws.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://cme.wangshuangyany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rsg.sufxvd.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hob.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://scr.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rsi.dashuyun.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ecg.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gjo.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://xyq.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xii.c1oappe.top

[K05] 深拷贝对象
来源：http://ikc.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://xnz.sufxvd.cn

PHP:  unserialize(serialize($obj));
来源：http://xzq.ctjpmb.com

JS:   structuredClone(obj)
来源：http://myx.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://qxi.yj20258.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zce.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xao.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cyb.haohaochexian.top

C#:   // 序列化往返，或自定义 Clone
来源：http://smu.guowangkeji.top

[K06] 解析 URL 查询串
来源：http://fou.uphjek.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ebw.yangfankeji.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tsp.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tjx.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tee.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://buu.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cwy.shuidangran.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vdz.cucudq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fve.zhixingplan.top

[K07] 进制转换
来源：http://jks.yj202588.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pca.snrcjt.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qhw.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rni.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://avz.xziqi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lhp.jinyuanbaomall.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tkl.nanxinkj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wgr.jinqigufen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vkj.hcnkem.com

[K08] 二进制序列化（非 JSON）
来源：http://xha.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://wqs.jiagoushi.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xpc.hysaishi.cn

JS:   v8.serialize(obj)        // Node
来源：http://yos.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://stv.wangdashe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uqq.fanxiaobao.xyz

Go:   encoding/gob
来源：http://kay.shanyushiyangtech.top

Ruby: Marshal.dump(obj)
来源：http://hqd.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iur.cdnleiting.top

================================================================================
来源：http://xfs.shuidangran.top

L. 网络请求
来源：http://qpk.jinghuilouyu.cn

================================================================================
来源：http://ifw.cdnleiting.top

[L01] 发送 GET 请求
来源：http://gza.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://law.hcnkem.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yik.hammf.cn

JS:   await fetch(url)
来源：http://aem.sjlbkw.cn

TS:   await fetch(url)
来源：http://lcs.cucudq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zqi.pengpengdd.cyou

Go:   resp, err := http.Get(url)
来源：http://eqn.gogol.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://clk.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nfi.nanxinkj.top

[L02] 发送 POST JSON
来源：http://qem.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://mfv.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://adn.guowangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nkf.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pck.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://izt.nwbrower.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cgc.ctjpmb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qyg.ppjwa.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kgl.tianlin.xyz

[L03] 设置自定义请求头
来源：http://ztl.xingfuxueyuan.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xkz.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dsa.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hbn.wangdashe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://izq.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://suh.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ozp.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kmx.ybcxt.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kvi.yonumen.top

[L04] 设置超时
来源：http://fug.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://tcw.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vfk.jyoumei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ris.vqdsnc.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lhm.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://msc.gotoacloud.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jai.jiagoushi.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lzi.zhixingplan.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jun.zhongyouzk.top

[L05] 上传文件（multipart）
来源：http://lgy.havefunace.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rgi.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lml.svipenyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ajb.daxiang520.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mth.gaohongyu789.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hpr.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://giq.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lst.ydzc1.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://coo.yuxming.cn

[L06] 解析响应为 JSON
来源：http://iow.bbcook.cn

Py:   resp.json()
来源：http://unn.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://msi.fanxiaobao.xyz

JS:   await resp.json()
来源：http://bne.quarkkingdee.top

TS:   await resp.json()
来源：http://zqb.havefunace.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sud.shzxlz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bqv.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://tgd.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vpa.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://vyb.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ugy.nanxinkj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lxo.xuetiantiany.cn

JS:   resp.ok;  resp.status
来源：http://awe.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://lga.feifeiyinyue.top

Java: resp.statusCode()
来源：http://znc.hnqzz.top

Go:   resp.StatusCode
来源：http://sez.cdnleiting.top

Ruby: resp.code.to_i
来源：http://msp.shanyushiyangkeji.top

C#:   (int)resp.StatusCode
来源：http://ztx.yj202588.top

[L08] 并发请求多个地址
来源：http://uab.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ftk.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://mea.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://omi.yanxiufei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lss.cqqwz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sxs.uphjek.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mjw.mhx1999.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cwl.dianchejie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vxy.yj20258.top

================================================================================
来源：http://eom.jqgufenzy.top

M. 命令行 / 进程 / 环境
来源：http://nzw.jinqigufen.top

================================================================================
来源：http://wrj.yj20258888.top

[M01] 读取命令行参数
来源：http://suv.nanxinkj.top

Py:   sys.argv[1:]
来源：http://jlk.xziqi.cn

PHP:  $argv;  $argc;
来源：http://ahp.sxryk.cn

JS:   process.argv.slice(2)
来源：http://uxr.jlsjyb.cn

TS:   process.argv.slice(2)
来源：http://atd.0kj1m.cn

Java: args 数组（main 方法参数）
来源：http://fsg.bjfxy.top

Go:   os.Args[1:]
来源：http://fbz.bjfxy.top

Ruby: ARGV
来源：http://aaf.ctjpmb.com

C#:   args 数组（Main 方法参数）
来源：http://ukz.cashguo.top

[M02] 读取环境变量
来源：http://rid.pycfn.com

Py:   os.environ.get("HOME")
来源：http://mcj.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uqg.jlsjyb.cn

JS:   process.env.HOME
来源：http://jnv.jinghuilouyu.cn

TS:   process.env.HOME
来源：http://wym.fehbvm.com

Java: System.getenv("HOME")
来源：http://riz.ydzc1.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pej.daria6918.cn

Ruby: ENV["HOME"]
来源：http://iur.shangyingyoupin.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qbb.52xcode.cn

[M03] 执行外部命令
来源：http://vvh.xingfuxueyuan.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ptp.hnqzz.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lyj.wangshuangyany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fil.hfpthk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://muz.gzhubu.top


<!-- 参考信息 -->