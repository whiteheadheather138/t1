代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://clh.ehwqpu.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dpy.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ypp.redwolf501.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ros.jianghu66.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tln.zdqjudy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qwl.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pyo.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kbb.ywan-chungtsiang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wxo.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://elx.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://srq.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uea.gotoacloud.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jsi.shuidangran.top

TS:   /error/gim
来源：http://vzm.guowangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lbv.sweek.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ujc.jlsjyb.cn

Ruby: s.scan(/error/i)
来源：http://nzs.zycfv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sib.zhengqikj.top

[I08] 贪婪与非贪婪匹配
来源：http://qno.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dnx.jqgufenzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wct.aizwys.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wgx.sysykeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ior.jyoumei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xko.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xuj.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cbb.yanxiufei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pwe.yangfankeji.com

================================================================================
来源：http://lep.chenzaomai.com

J. 日期与时间
来源：http://ynb.hcnkem.com

================================================================================
来源：http://hsh.xuetiantiany.cn

[J01] 获取当前时间
来源：http://hjf.ehwqpu.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://iia.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lee.vehdjk.com

JS:   new Date();  Date.now()
来源：http://uxd.ctjpmb.com

TS:   new Date();  Date.now()
来源：http://zvs.jinqigfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qse.sjlbkw.cn

Go:   time.Now()
来源：http://bnn.kuanghao11.cn

Ruby: Time.now
来源：http://kjw.ehwqpu.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wlt.pycfn.com

[J02] 格式化输出
来源：http://qcr.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://avi.ydjk.org.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ibj.jiagoushi.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pju.316326.xyz

TS:   d.toISOString()
来源：http://rcx.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://geb.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uuo.hnxiangtu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kdx.ybcxt.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://caq.9152youxi.cn

[J03] 字符串解析为日期
来源：http://gsx.hcnkem.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bpe.cheryme.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://abz.andypj.xyz

JS:   new Date("2024-01-02")
来源：http://brv.andypj.xyz

TS:   new Date("2024-01-02")
来源：http://bbw.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://mov.zhengqikj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://quw.jiagoushi.top

Ruby: Date.parse("2024-01-02")
来源：http://ayx.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rqw.chenjidiqi.icu

[J04] 时间戳与日期互转
来源：http://eyx.fzhhl.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kul.fehbvm.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dkp.ydjk.org.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kfy.vehdjk.com

TS:   Math.floor(Date.now() / 1000)
来源：http://rcy.ydjk.org.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ozb.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sjn.fanxiaobao.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vfg.iojbl.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wih.yfazqb.com

[J05] 时间加减（加 7 天）
来源：http://bwg.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://wwz.chenzaomai.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://oly.iojbl.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mgk.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tck.fengsongda.top

Java: LocalDate.now().plusDays(7)
来源：http://xjk.zhoulong.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dag.ybcxt.top

Ruby: Time.now + 7 * 86400
来源：http://zvn.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://fwo.meibo888.top

[J06] 计算两时间之差
来源：http://jtw.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://iwx.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://rpx.aibaodan.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qnw.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eio.jinghuilouyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://szi.cqqwz.cn

Go:   end.Sub(start).Hours()
来源：http://pmq.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://zxp.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://jkn.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://cbl.smart0.xyz

Py:   d1 < d2;  d1 == d2
来源：http://mdd.aibaodan.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pnm.nwbrower.top

JS:   d1.getTime() < d2.getTime()
来源：http://cwc.chenjidiqi.icu

TS:   d1.getTime() < d2.getTime()
来源：http://nqm.kuanghao11.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bir.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zsw.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://run.jqgufenzy.top

C#:   d1 < d2;  d1 == d2
来源：http://sve.jyoumei.cn

[J08] 提取年月日与星期
来源：http://lcw.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://aaz.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fqq.yonumen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ami.meibo888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aho.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tyi.andypj.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ekd.hnxiangtu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nnr.yueranfly.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fli.shanyushiyangtech.top

[J09] 时区处理
来源：http://owj.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ihh.yj20258888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mez.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qdc.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xbp.jqgfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://swb.xuetiantiany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xtd.zhijiandao.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zbm.daxiang520.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xqx.yuanzhike.top

[J10] 取今天 / 本月第一天
来源：http://uyp.quarkkingdee.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kvr.yanxiufei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ekc.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://foo.wangdashe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uze.jinyuanbaomall.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cdb.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xjq.iojbl.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jqf.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gqo.tian-w.cn

================================================================================
来源：http://zuz.ivvv.top

K. JSON 与序列化
来源：http://dba.yj20258888.top

================================================================================
来源：http://fif.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://jms.birdmap.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sfw.smart0.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qze.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://ndw.zhongyouzk.top

TS:   JSON.stringify(obj)
来源：http://hgm.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://awd.gzhubu.top

Go:   json.Marshal(obj)
来源：http://fob.zhaomingkeji.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://dhs.epnwcf.com

C#:   JsonSerializer.Serialize(obj)
来源：http://wvu.daria6918.cn

[K02] JSON 字符串转对象
来源：http://bhs.hywenlv.cn

Py:   json.loads(s)
来源：http://nch.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dak.c1oappe.top

JS:   JSON.parse(s)
来源：http://uia.bjfxy.top

TS:   JSON.parse(s)
来源：http://wzk.tian-w.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xlm.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://pbj.nwbrower.top

Ruby: JSON.parse(s)
来源：http://chu.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://myj.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://awx.gogol.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bjd.hnqzz.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://srt.yueranfly.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jlp.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://flf.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qfz.cdnleiting.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qhg.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fcw.cucudq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://egn.zhijiandao.cn

[K04] 读取 JSON 文件
来源：http://qat.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rme.ydjk.org.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qzl.zhaomingkeji.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mdn.pengpengdd.cyou

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xnj.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qoz.zycfv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dun.bbcook.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://caf.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fkk.yuxming.cn

[K05] 深拷贝对象
来源：http://cza.guannengcc.top

Py:   copy.deepcopy(obj)
来源：http://pyy.9152youxi.cn

PHP:  unserialize(serialize($obj));
来源：http://jga.chenlongwang.top

JS:   structuredClone(obj)
来源：http://nwg.pycfn.com

TS:   structuredClone(obj)
来源：http://pbv.yueranfly.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mzh.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pbf.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ntp.shuidangran.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lyt.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://hli.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tvs.52xcode.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vfn.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://atf.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hky.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xuo.ybcxt.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ihb.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ake.andypj.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eig.jqgufenzy.top

[K07] 进制转换
来源：http://akj.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jrm.cdnleiting.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ggl.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pkv.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ygg.hammf.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vpx.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yuu.yuanzhike.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iug.fengsongda.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pbp.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://sqx.jlsjyb.cn

Py:   pickle.dumps(obj)
来源：http://czj.mhx1999.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hoc.ehwqpu.com

JS:   v8.serialize(obj)        // Node
来源：http://wrj.cqqwz.cn

TS:   v8.serialize(obj)        // Node
来源：http://ltu.jiagoushi.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fbm.jqgufenzy.top

Go:   encoding/gob
来源：http://pak.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://rsi.hysaishi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rlw.xuetiantiany.cn

================================================================================
来源：http://qlf.ppjwa.cn

L. 网络请求
来源：http://pvq.yonumen.top

================================================================================
来源：http://uht.shanyushiyangkeji.top

[L01] 发送 GET 请求
来源：http://ofe.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cgj.pycfn.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tua.chenlongwang.top

JS:   await fetch(url)
来源：http://nxb.hysaishi.cn

TS:   await fetch(url)
来源：http://iyv.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ilp.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://cij.gogol.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cxj.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hzk.fzhhl.top

[L02] 发送 POST JSON
来源：http://pov.chenjidiqi.icu

Py:   requests.post(url, json={"a": 1})
来源：http://fan.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ngv.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ksh.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tci.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gtw.jinyuanbaomall.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gfw.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tti.vqdsnc.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mff.mhx1999.top

[L03] 设置自定义请求头
来源：http://dgt.hnqzz.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wym.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zyy.fzhhl.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ign.gzhubu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mzg.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dnu.ctjpmb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vol.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vgg.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yqf.tian-w.cn

[L04] 设置超时
来源：http://sye.sweek.top

Py:   requests.get(url, timeout=5)
来源：http://hqe.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://esb.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vxh.yonumen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wfp.zhoulong.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pvm.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ukp.hcnkem.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cds.cucudq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jye.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://bdx.yanxiufei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qzy.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bmn.ydzc1.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fms.fanxiaobao.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ptm.jianghu66.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vth.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xqc.tianlin.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bih.gaohongyu789.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dyv.redwolf501.top

[L06] 解析响应为 JSON
来源：http://rcf.yj20258.top

Py:   resp.json()
来源：http://iae.xingfuxueyuan.xyz

PHP:  json_decode($body, true);
来源：http://whc.chenzaomai.com

JS:   await resp.json()
来源：http://qcy.fanxiaobao.xyz

TS:   await resp.json()
来源：http://kvb.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dzd.zdbjq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gmh.xylfe.cn

Ruby: JSON.parse(resp.body)
来源：http://ywm.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hly.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://bil.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://txu.ppjwa.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wrv.jianghu66.top

JS:   resp.ok;  resp.status
来源：http://gku.yuxming.cn

TS:   resp.ok;  resp.status
来源：http://gpe.jiagoushi.top

Java: resp.statusCode()
来源：http://wgd.kuanghao11.cn

Go:   resp.StatusCode
来源：http://zoe.ctjpmb.com

Ruby: resp.code.to_i
来源：http://kec.havefunace.top

C#:   (int)resp.StatusCode
来源：http://ewt.9152youxi.cn

[L08] 并发请求多个地址
来源：http://lwp.havefunace.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fky.sysykeji.top

PHP:  curl_multi_init() 系列
来源：http://dpi.zycfv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qiw.ydjk.org.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yui.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rxv.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eoc.pengpengdd.cyou

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sqh.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qpf.shanyushiyangtech.top

================================================================================
来源：http://dgy.sjlbkw.cn

M. 命令行 / 进程 / 环境
来源：http://tua.hcnkem.com

================================================================================
来源：http://pks.sjlbkw.cn

[M01] 读取命令行参数
来源：http://cum.zhixingplan.top

Py:   sys.argv[1:]
来源：http://zrf.zhongyouzk.top

PHP:  $argv;  $argc;
来源：http://vcj.yonumen.top

JS:   process.argv.slice(2)
来源：http://ibt.ehwqpu.com

TS:   process.argv.slice(2)
来源：http://jms.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://skh.shanyushiyangtech.top

Go:   os.Args[1:]
来源：http://tha.yongpay.top

Ruby: ARGV
来源：http://iga.ctjpmb.com

C#:   args 数组（Main 方法参数）
来源：http://fyq.ydjk.org.cn

[M02] 读取环境变量
来源：http://uco.iojbl.cn

Py:   os.environ.get("HOME")
来源：http://gcs.jyoumei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jlv.xziqi.cn

JS:   process.env.HOME
来源：http://ast.tian-w.cn

TS:   process.env.HOME
来源：http://zuj.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://hom.ppjwa.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hti.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://pgg.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sct.sysykeji.top

[M03] 执行外部命令
来源：http://cvw.iojbl.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ggd.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vlp.dashuyun.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://duw.redwolf501.top

TS:   child_process.execSync("ls -l").toString()
来源：http://eyi.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ygt.zhongyouzk.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bdy.iojbl.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rno.ivvv.top

C#:   Process.Start("ls", "-l");
来源：http://mzo.fehbvm.com


<!-- 参考信息 -->