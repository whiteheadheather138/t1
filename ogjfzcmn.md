代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://arw.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lbs.yuxming.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oqu.yuxming.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jza.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lyu.zdqjudy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dtu.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xne.yj20258888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sjl.yongpay.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tvy.chenlongwang.top

[I07] 忽略大小写与多行模式
来源：http://ltg.sysykeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://crp.cheryme.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fbp.yj20258888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vgk.zdbjq.cn

TS:   /error/gim
来源：http://agp.yj20258888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qdg.kuanghao11.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eej.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://dvp.iojbl.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://akn.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://csh.dashuyun.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uxr.c1oappe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iwj.nwbrower.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gez.yuanzhike.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lyt.epnwcf.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://dqw.tarul.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kqw.yuxming.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yah.iojbl.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ksb.wangdashe.top

================================================================================
来源：http://uky.xingfuxueyuan.xyz

J. 日期与时间
来源：http://ini.tanke756.top

================================================================================
来源：http://sfu.vqdsnc.cn

[J01] 获取当前时间
来源：http://xux.tianlin.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://vqz.pengpengdd.cyou

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://icl.fktsv.cn

JS:   new Date();  Date.now()
来源：http://exo.shuidangran.top

TS:   new Date();  Date.now()
来源：http://ekn.quarkkingdee.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sml.smart0.xyz

Go:   time.Now()
来源：http://ffn.sjlbkw.cn

Ruby: Time.now
来源：http://xfh.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lgx.jqgfzy.top

[J02] 格式化输出
来源：http://hgd.xylfe.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zle.jinyuanbaomall.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jeq.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dco.birdmap.top

TS:   d.toISOString()
来源：http://qlv.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://omo.nwbrower.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ggt.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tpu.cucudq.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vcs.ehwqpu.com

[J03] 字符串解析为日期
来源：http://ahs.hcnkem.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qtj.yanxiufei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lqj.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://lgf.uphjek.com

TS:   new Date("2024-01-02")
来源：http://may.snrcjt.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tnx.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ujs.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://dka.kuanghao11.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qtl.gaohongyu789.top

[J04] 时间戳与日期互转
来源：http://pjt.ywan-chungtsiang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pyd.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lbr.shanyushiyangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uvf.wangshuangyany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uyh.zhijiandao.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qzh.hnxiangtu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hcs.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://llb.zdbjq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ads.guowangkeji.top

[J05] 时间加减（加 7 天）
来源：http://ekw.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://eyc.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xdp.chenlongwang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uiv.316326.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wgx.svipenyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://qiz.tarul.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hrx.shangyingyoupin.top

Ruby: Time.now + 7 * 86400
来源：http://yau.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bah.cucudq.cn

[J06] 计算两时间之差
来源：http://luk.xziqi.cn

Py:   (end - start).total_seconds()
来源：http://mxv.yfazqb.com

PHP:  $end->diff($start)->days;
来源：http://fpm.aizwys.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tfl.pengpengdd.cyou

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lrl.shanyushiyangtech.top

Java: Duration.between(start, end).toSeconds()
来源：http://ueg.jlsjyb.cn

Go:   end.Sub(start).Hours()
来源：http://qwo.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://jkx.shuidangran.top

C#:   (end - start).TotalSeconds
来源：http://qrq.xuetiantiany.cn

[J07] 比较两个日期
来源：http://nqn.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://mce.yfazqb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eme.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://vxo.ehwqpu.com

TS:   d1.getTime() < d2.getTime()
来源：http://xsg.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lwl.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hvf.sweek.top

Ruby: d1 < d2;  d1 == d2
来源：http://ven.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://dqe.jianghu66.top

[J08] 提取年月日与星期
来源：http://qel.zhongyouzk.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gqq.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wyp.zhongyouzk.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cxh.gzhubu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bdv.vehdjk.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dom.wangdashe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pet.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vov.tanke756.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lvp.hnxiangtu.top

[J09] 时区处理
来源：http://jhh.ivvv.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eqd.ydzc1.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bbf.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ncc.gogol.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ihm.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wdd.sjlbkw.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sql.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tna.svipenyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qyo.xuetiantiany.cn

[J10] 取今天 / 本月第一天
来源：http://auq.yueranfly.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kwe.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xco.ywan-chungtsiang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cbl.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yld.ivvv.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fvm.daria6918.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ewr.bbcook.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nna.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bqt.jiagoushi.top

================================================================================
来源：http://ngo.ydjk.org.cn

K. JSON 与序列化
来源：http://uav.hongshengwenyu.top

================================================================================
来源：http://czj.yongpay.top

[K01] 对象转 JSON 字符串
来源：http://exq.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oic.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://llu.yj20258.top

JS:   JSON.stringify(obj)
来源：http://msz.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://goo.sysykeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eus.yuxming.cn

Go:   json.Marshal(obj)
来源：http://xie.daxiang520.top

Ruby: obj.to_json                                     // require "json"
来源：http://cck.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://omc.xingfuxueyuan.xyz

[K02] JSON 字符串转对象
来源：http://tqk.hnxiangtu.top

Py:   json.loads(s)
来源：http://axj.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ukv.bjfxy.top

JS:   JSON.parse(s)
来源：http://mzi.yfazqb.com

TS:   JSON.parse(s)
来源：http://icz.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mzq.smart0.xyz

Go:   json.Unmarshal(data, &v)
来源：http://wqt.0kj1m.cn

Ruby: JSON.parse(s)
来源：http://fah.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oyt.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://tyq.shuidangran.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bpw.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yrm.52xcode.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jad.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yti.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dfy.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rio.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://dzg.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mdd.zycfv.cn

[K04] 读取 JSON 文件
来源：http://efa.dashuyun.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xcx.zhengqikj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ltz.daxiang520.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wlg.yj20258888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://snl.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jxi.mhx1999.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hhu.fktsv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://arh.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uqu.yonumen.top

[K05] 深拷贝对象
来源：http://uzb.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://fuz.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://mhx.ehwqpu.com

JS:   structuredClone(obj)
来源：http://mmx.dashuyun.cn

TS:   structuredClone(obj)
来源：http://hjw.aibaodan.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zwz.yangfankeji.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jrs.vehdjk.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sef.shuidangran.top

C#:   // 序列化往返，或自定义 Clone
来源：http://drb.redwolf501.top

[K06] 解析 URL 查询串
来源：http://bvy.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pjd.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rqv.yangfankeji.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rin.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://odv.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://djg.quarkkingdee.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ufi.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nsn.ydjk.org.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hsc.9152youxi.cn

[K07] 进制转换
来源：http://urf.kuanghao11.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cfz.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cxs.yonumen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hik.pengpengdd.cyou

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tlb.xinyue.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ytm.gogol.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nvi.shanyushiyangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zna.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fuw.gotoacloud.top

[K08] 二进制序列化（非 JSON）
来源：http://qth.jinqigfzy.top

Py:   pickle.dumps(obj)
来源：http://gid.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jir.xuanzx.com

JS:   v8.serialize(obj)        // Node
来源：http://dhk.zhaomingkeji.xyz

TS:   v8.serialize(obj)        // Node
来源：http://bfm.jianghu66.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zmo.ppjwa.cn

Go:   encoding/gob
来源：http://xlv.wangshuangyany.cn

Ruby: Marshal.dump(obj)
来源：http://xah.fanxiaobao.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dcc.smart0.xyz

================================================================================
来源：http://byc.vqdsnc.cn

L. 网络请求
来源：http://qol.bjfxy.top

================================================================================
来源：http://qmy.hammf.cn

[L01] 发送 GET 请求
来源：http://wmj.nwbrower.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ibk.shanyushiyangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jey.andypj.xyz

JS:   await fetch(url)
来源：http://ocp.hywenlv.cn

TS:   await fetch(url)
来源：http://cpj.pycfn.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://chj.ybcxt.top

Go:   resp, err := http.Get(url)
来源：http://pzw.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gsn.yj20258888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kwx.guannengcc.top

[L02] 发送 POST JSON
来源：http://wbc.tanke756.top

Py:   requests.post(url, json={"a": 1})
来源：http://ijp.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pfi.xingfuxueyuan.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wgf.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mab.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://she.yonumen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zex.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://njp.guowangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lya.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://noo.zdbjq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://orx.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://frb.uphjek.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://doi.ydzc1.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tss.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://frz.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jak.yfazqb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rhu.tianlin.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kvv.cqqwz.cn

[L04] 设置超时
来源：http://fbg.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://dvn.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bvj.xziqi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ati.zdbjq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xtw.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://prt.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rrp.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bav.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zgy.feifeiyinyue.top

[L05] 上传文件（multipart）
来源：http://via.ybcxt.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hfq.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pdv.uphjek.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nje.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dow.guannengcc.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://akq.yuxming.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fxh.xuetiantiany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xhc.xuanzx.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ovj.c1oappe.top

[L06] 解析响应为 JSON
来源：http://vso.zhijiandao.cn

Py:   resp.json()
来源：http://xeg.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://jaz.ivvv.top

JS:   await resp.json()
来源：http://aov.yj20258.top

TS:   await resp.json()
来源：http://mly.ydzc1.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qiu.snrcjt.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gga.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://cnr.yanxiufei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nvn.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://xne.xuanzx.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://opc.0kj1m.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://duy.jqgfzy.top

JS:   resp.ok;  resp.status
来源：http://hof.daxiang520.top

TS:   resp.ok;  resp.status
来源：http://rkm.svipenyu.cn

Java: resp.statusCode()
来源：http://qgp.birdmap.top

Go:   resp.StatusCode
来源：http://jdp.yonumen.top

Ruby: resp.code.to_i
来源：http://tpf.redwolf501.top

C#:   (int)resp.StatusCode
来源：http://tbq.yuanzhike.top

[L08] 并发请求多个地址
来源：http://muz.daxiang520.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vtv.shangyingyoupin.top

PHP:  curl_multi_init() 系列
来源：http://arj.yvedp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://utz.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://thc.zhoulong.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://svb.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xbl.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uwn.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fqt.gzhubu.top

================================================================================
来源：http://vtj.fehbvm.com

M. 命令行 / 进程 / 环境
来源：http://gmo.vqdsnc.cn

================================================================================
来源：http://tta.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://yfe.hongshengwenyu.top

Py:   sys.argv[1:]
来源：http://pvg.hcnkem.com

PHP:  $argv;  $argc;
来源：http://yxl.dianchejie.cn

JS:   process.argv.slice(2)
来源：http://ahl.quarkkingdee.top

TS:   process.argv.slice(2)
来源：http://aht.meibo888.top

Java: args 数组（main 方法参数）
来源：http://nrp.yuanzhike.top

Go:   os.Args[1:]
来源：http://vtd.zhoulong.xyz

Ruby: ARGV
来源：http://tda.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://yws.sjlbkw.cn

[M02] 读取环境变量
来源：http://pnp.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://sps.xinyue.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lsx.cucudq.cn

JS:   process.env.HOME
来源：http://egb.jianghu66.top

TS:   process.env.HOME
来源：http://ufe.birdmap.top

Java: System.getenv("HOME")
来源：http://atk.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tup.yanxiufei.cn

Ruby: ENV["HOME"]
来源：http://ddi.gotoacloud.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://knu.0kj1m.cn

[M03] 执行外部命令
来源：http://txn.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://abb.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jck.chenzaomai.com

JS:   child_process.execSync("ls -l").toString()
来源：http://rla.jinqigfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kst.wangshuangyany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bkf.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xcc.yvedp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sat.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://jgm.nanxuanxn.top


<!-- 参考信息 -->