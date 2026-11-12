代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://pnt.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tzv.cheryme.top

Ruby: s.split(/\s*,\s*/)
来源：http://eis.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uht.uphjek.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rke.xingfuxueyuan.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xta.ywan-chungtsiang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vwg.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cvc.yanxiufei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://roj.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lla.havefunace.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jud.kuanghao11.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eus.zhijiandao.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uek.xziqi.cn

[I07] 忽略大小写与多行模式
来源：http://ciq.dianchejie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kvj.ppjwa.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bbh.birdmap.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mkk.chenjidiqi.icu

TS:   /error/gim
来源：http://uey.guowangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mpl.chenzaomai.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jbs.tarul.cn

Ruby: s.scan(/error/i)
来源：http://fsl.pycfn.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nze.pengpengdd.cyou

[I08] 贪婪与非贪婪匹配
来源：http://mod.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://awe.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ket.smart0.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jxj.ywan-chungtsiang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lrd.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bcm.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://byt.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nxt.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dzu.gaohongyu789.top

================================================================================
来源：http://srt.hongshengwenyu.top

J. 日期与时间
来源：http://bmm.ywan-chungtsiang.top

================================================================================
来源：http://wru.hnqzz.top

[J01] 获取当前时间
来源：http://nyu.chenzaomai.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://zre.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oqo.chenlongwang.top

JS:   new Date();  Date.now()
来源：http://pfv.wangshuangyany.cn

TS:   new Date();  Date.now()
来源：http://mgw.bjfxy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://iji.hammf.cn

Go:   time.Now()
来源：http://vte.daria6918.cn

Ruby: Time.now
来源：http://kno.xinyue.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jov.zhiwuduotai.top

[J02] 格式化输出
来源：http://erb.jyoumei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tyc.dashuyun.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eze.sxryk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lnf.jinqigufen.top

TS:   d.toISOString()
来源：http://ctj.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jcr.zdqjudy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://asm.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mxw.yj202588.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gzq.smart0.xyz

[J03] 字符串解析为日期
来源：http://wyt.xinyue.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wux.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kut.vehdjk.com

JS:   new Date("2024-01-02")
来源：http://ngv.yj202588.top

TS:   new Date("2024-01-02")
来源：http://uqt.nwbrower.top

Java: LocalDate.parse("2024-01-02")
来源：http://qdg.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cgg.aizwys.cn

Ruby: Date.parse("2024-01-02")
来源：http://vop.hcnkem.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tmq.shanyushiyangkeji.top

[J04] 时间戳与日期互转
来源：http://djy.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yrm.zhengqikj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vfr.yvedp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dns.jinyuanbaomall.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wsf.cqqwz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://unv.ybcxt.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sog.jinqigfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fnv.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://udu.zdqjudy.top

[J05] 时间加减（加 7 天）
来源：http://jtp.meibo888.top

Py:   now + timedelta(days=7)
来源：http://xrn.c1oappe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mjc.yj202588.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qzk.bbcook.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qeh.52xcode.cn

Java: LocalDate.now().plusDays(7)
来源：http://fja.ywan-chungtsiang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dwh.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://zgx.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://lfm.fanxiaobao.xyz

[J06] 计算两时间之差
来源：http://nkv.cheryme.top

Py:   (end - start).total_seconds()
来源：http://mcy.cheryme.top

PHP:  $end->diff($start)->days;
来源：http://wrm.9152youxi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ybw.yuanzhike.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yud.hywenlv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ueg.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://xwm.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://ovf.zhongyouzk.top

C#:   (end - start).TotalSeconds
来源：http://vxn.andypj.xyz

[J07] 比较两个日期
来源：http://bjg.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://jfa.hongshengwenyu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jto.zhengqikj.top

JS:   d1.getTime() < d2.getTime()
来源：http://fwr.hnqzz.top

TS:   d1.getTime() < d2.getTime()
来源：http://nkh.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dwc.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jbr.fehbvm.com

Ruby: d1 < d2;  d1 == d2
来源：http://xnp.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://agl.yj20258.top

[J08] 提取年月日与星期
来源：http://cqi.xuetiantiany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://opy.aibaodan.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qjh.52xcode.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cnt.tianlin.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ata.havefunace.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qno.ydjk.org.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zfd.cucudq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://shb.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wze.0kj1m.cn

[J09] 时区处理
来源：http://frp.guannengcc.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rgl.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pac.gaohongyu789.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gfx.nanxuanxn.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://shn.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qyh.bbcook.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qcw.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://syh.sxryk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://efs.xuetiantiany.cn

[J10] 取今天 / 本月第一天
来源：http://gux.guowangkeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://oiy.yanxiufei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zju.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://znh.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://azq.tarul.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lyy.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cls.wangdashe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qhl.jyoumei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jpj.yonumen.top

================================================================================
来源：http://aov.vehdjk.com

K. JSON 与序列化
来源：http://xre.redwolf501.top

================================================================================
来源：http://hvd.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://rfn.yuxming.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kwx.yvedp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jou.nwbrower.top

JS:   JSON.stringify(obj)
来源：http://vcj.tianlin.xyz

TS:   JSON.stringify(obj)
来源：http://piy.wangshuangyany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kyb.ehwqpu.com

Go:   json.Marshal(obj)
来源：http://erk.fanxiaobao.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://sad.316326.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://pyc.daria6918.cn

[K02] JSON 字符串转对象
来源：http://sju.jinqigufen.top

Py:   json.loads(s)
来源：http://fhr.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ita.zdbjq.cn

JS:   JSON.parse(s)
来源：http://ejh.havefunace.top

TS:   JSON.parse(s)
来源：http://wfd.jinghuilouyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rni.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://vlc.jiagoushi.top

Ruby: JSON.parse(s)
来源：http://unk.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jhu.ehwqpu.com

[K03] JSON 美化输出（带缩进）
来源：http://alb.zhengqikj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://niu.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://koa.xinyue.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://ezg.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://vuq.xuetiantiany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ckk.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yre.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://szd.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cvk.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://iio.sufxvd.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aqy.havefunace.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://auz.aizwys.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ndv.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sza.ctjpmb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uxv.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fme.yuanzhike.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://axm.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oui.xziqi.cn

[K05] 深拷贝对象
来源：http://ihl.svipenyu.cn

Py:   copy.deepcopy(obj)
来源：http://hcw.zhoulong.xyz

PHP:  unserialize(serialize($obj));
来源：http://lir.ivvv.top

JS:   structuredClone(obj)
来源：http://fva.wangdashe.top

TS:   structuredClone(obj)
来源：http://xof.jinqigfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wbc.daxiang520.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mmq.epnwcf.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://inf.wangshuangyany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ejz.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://akq.52xcode.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://edf.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lqs.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://arf.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ukr.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nje.gotoacloud.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kvk.vehdjk.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jgv.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qdg.zhongyouzk.top

[K07] 进制转换
来源：http://ydq.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wff.nanxuanxn.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hfu.svipenyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kre.sweek.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bao.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uwu.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yum.c1oappe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bqq.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sfa.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://uax.kuanghao11.cn

Py:   pickle.dumps(obj)
来源：http://tae.cqqwz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ytz.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://ydf.yuxming.cn

TS:   v8.serialize(obj)        // Node
来源：http://toa.zhengqikj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cgh.jinghuilouyu.cn

Go:   encoding/gob
来源：http://twm.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://izd.quarkkingdee.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kkd.ywan-chungtsiang.top

================================================================================
来源：http://ojb.jinqigufen.top

L. 网络请求
来源：http://hwo.gzhubu.top

================================================================================
来源：http://ayk.cucudq.cn

[L01] 发送 GET 请求
来源：http://apv.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gbc.sweek.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sdf.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://sdk.hfpthk.cn

TS:   await fetch(url)
来源：http://aqj.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://daw.nanxuanxn.top

Go:   resp, err := http.Get(url)
来源：http://qox.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oia.zhoulong.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://onw.sweek.top

[L02] 发送 POST JSON
来源：http://nmg.xuanzx.com

Py:   requests.post(url, json={"a": 1})
来源：http://qbw.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zey.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://llz.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pmy.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hff.ydzc1.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ohi.xylfe.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bbr.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fvl.zycfv.cn

[L03] 设置自定义请求头
来源：http://dqp.yangfankeji.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://szi.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qde.nanxinkj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tle.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jnc.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wao.quarkkingdee.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jnx.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://juy.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zkk.pengpengdd.cyou

[L04] 设置超时
来源：http://wvw.dianchejie.cn

Py:   requests.get(url, timeout=5)
来源：http://trk.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xnj.redwolf501.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dai.hesvh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zeq.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vea.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tma.zhengqikj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gdi.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bfd.epnwcf.com

[L05] 上传文件（multipart）
来源：http://kjg.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fbx.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kww.dashuyun.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qmc.gzhubu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lgy.bbcook.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fkz.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qph.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ymc.ydjk.org.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qty.cdnleiting.top

[L06] 解析响应为 JSON
来源：http://ayp.svipenyu.cn

Py:   resp.json()
来源：http://oxc.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://hwb.dashuyun.cn

JS:   await resp.json()
来源：http://ufy.smart0.xyz

TS:   await resp.json()
来源：http://fxy.shangyingyoupin.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vcy.aibaodan.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://via.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://xgh.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://llk.jinghuilouyu.cn

[L07] 处理 HTTP 状态码
来源：http://gff.zhixingplan.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gth.yanxiufei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tmh.nanxuanxn.top

JS:   resp.ok;  resp.status
来源：http://xrz.fanxiaobao.xyz

TS:   resp.ok;  resp.status
来源：http://rcv.vqdsnc.cn

Java: resp.statusCode()
来源：http://hhv.jiagoushi.top

Go:   resp.StatusCode
来源：http://juo.hfpthk.cn

Ruby: resp.code.to_i
来源：http://pzh.chenzaomai.com

C#:   (int)resp.StatusCode
来源：http://tfa.hcnkem.com

[L08] 并发请求多个地址
来源：http://lug.svipenyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lik.dashuyun.cn

PHP:  curl_multi_init() 系列
来源：http://zkg.ywan-chungtsiang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mkw.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wsr.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rtp.xziqi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vtb.havefunace.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cxo.svipenyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ljp.nanxinkj.top

================================================================================
来源：http://crg.gotoacloud.top

M. 命令行 / 进程 / 环境
来源：http://jya.sjlbkw.cn

================================================================================
来源：http://iyi.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://hop.jqgfzy.top

Py:   sys.argv[1:]
来源：http://nvw.ywan-chungtsiang.top

PHP:  $argv;  $argc;
来源：http://wzg.aibaodan.cn

JS:   process.argv.slice(2)
来源：http://cdp.ppjwa.cn

TS:   process.argv.slice(2)
来源：http://qfq.xuetiantiany.cn

Java: args 数组（main 方法参数）
来源：http://onv.iojbl.cn

Go:   os.Args[1:]
来源：http://jgd.guowangkeji.top

Ruby: ARGV
来源：http://dqx.jlsjyb.cn

C#:   args 数组（Main 方法参数）
来源：http://ein.zhijiandao.cn

[M02] 读取环境变量
来源：http://dee.jqgfzy.top

Py:   os.environ.get("HOME")
来源：http://zgx.ctjpmb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ygr.chenjidiqi.icu

JS:   process.env.HOME
来源：http://cbm.fktsv.cn

TS:   process.env.HOME
来源：http://yda.316326.xyz

Java: System.getenv("HOME")
来源：http://hzh.nanxuanxn.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nim.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://zcm.fzhhl.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mtr.sysykeji.top

[M03] 执行外部命令
来源：http://kbg.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fwa.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lfp.jqgfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tur.yfazqb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://amu.zhongyouzk.top


<!-- 参考信息 -->