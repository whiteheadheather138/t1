代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qnt.smart0.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xps.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://liw.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yfv.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yjl.zhijiandao.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zgn.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jxv.hesvh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qck.ydjk.org.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gze.daxiang520.top

[I07] 忽略大小写与多行模式
来源：http://wgw.yanxiufei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pku.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dbr.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gyo.daxiang520.top

TS:   /error/gim
来源：http://spy.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gqe.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://egl.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://eic.wangdashe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pur.dashuyun.cn

[I08] 贪婪与非贪婪匹配
来源：http://bsb.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nut.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dok.ppjwa.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xob.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xya.zhaomingkeji.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://lht.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ucr.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lfs.52xcode.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://otu.yvedp.cn

================================================================================
来源：http://urr.fengsongda.top

J. 日期与时间
来源：http://qab.jlsjyb.cn

================================================================================
来源：http://lru.pycfn.com

[J01] 获取当前时间
来源：http://oqd.yj20258888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ngj.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ehg.pycfn.com

JS:   new Date();  Date.now()
来源：http://bmb.jqgufenzy.top

TS:   new Date();  Date.now()
来源：http://cdg.xylfe.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://amk.zhoulong.xyz

Go:   time.Now()
来源：http://brt.nanxinkj.top

Ruby: Time.now
来源：http://mkq.daxiang520.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yio.dianchejie.cn

[J02] 格式化输出
来源：http://uyc.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gye.cashguo.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zdx.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jwd.cashguo.top

TS:   d.toISOString()
来源：http://fon.xylfe.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zzi.zhijiandao.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gxb.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wqx.jinqigufen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mnz.daxiang520.top

[J03] 字符串解析为日期
来源：http://wkl.jqgufenzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qio.ehwqpu.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lie.yanxiufei.cn

JS:   new Date("2024-01-02")
来源：http://eux.jinyuanbaomall.cn

TS:   new Date("2024-01-02")
来源：http://usl.sweek.top

Java: LocalDate.parse("2024-01-02")
来源：http://qhe.ywan-chungtsiang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cxn.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://qpb.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vhq.jinghuilouyu.cn

[J04] 时间戳与日期互转
来源：http://uoy.hcnkem.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jdx.zhaomingkeji.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gxv.nanxinkj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bfy.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://qbr.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://obw.yuanzhike.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://usu.fktsv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wpn.tian-w.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qvs.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://xak.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://jgb.gaohongyu789.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ymq.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ikv.ivvv.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aid.jinqigfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://hqf.andypj.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://owb.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://nyx.zdqjudy.top

C#:   DateTime.Now.AddDays(7)
来源：http://ifk.ywan-chungtsiang.top

[J06] 计算两时间之差
来源：http://wim.zhengqikj.top

Py:   (end - start).total_seconds()
来源：http://pri.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://rda.9152youxi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kqf.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tvw.wangdashe.top

Java: Duration.between(start, end).toSeconds()
来源：http://dwv.sweek.top

Go:   end.Sub(start).Hours()
来源：http://smj.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://bmk.hnqzz.top

C#:   (end - start).TotalSeconds
来源：http://vok.daria6918.cn

[J07] 比较两个日期
来源：http://fig.shanyushiyangtech.top

Py:   d1 < d2;  d1 == d2
来源：http://jrk.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nam.snrcjt.cn

JS:   d1.getTime() < d2.getTime()
来源：http://leg.316326.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://ivr.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tpe.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pgy.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://mul.ydjk.org.cn

C#:   d1 < d2;  d1 == d2
来源：http://qbb.vehdjk.com

[J08] 提取年月日与星期
来源：http://nxg.316326.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qka.chenzaomai.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uce.cdnleiting.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sok.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lwp.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://opj.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qcp.xuetiantiany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://awi.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://btd.haohaochexian.top

[J09] 时区处理
来源：http://ete.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rft.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bmw.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tnu.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yxq.hongshengwenyu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kyi.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rzn.jiagoushi.top

Ruby: Time.now.getlocal("+08:00")
来源：http://buc.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vlr.sweek.top

[J10] 取今天 / 本月第一天
来源：http://jdb.tian-w.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://teh.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ght.wangshuangyany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bqy.yuanzhike.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ntx.ctjpmb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nkq.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vqd.fehbvm.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xmp.hnxiangtu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bqa.jiagoushi.top

================================================================================
来源：http://eam.cqqwz.cn

K. JSON 与序列化
来源：http://dxr.yj20258888.top

================================================================================
来源：http://wpx.cucudq.cn

[K01] 对象转 JSON 字符串
来源：http://ktp.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mjw.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bpx.cheryme.top

JS:   JSON.stringify(obj)
来源：http://trx.ydjk.org.cn

TS:   JSON.stringify(obj)
来源：http://rks.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xky.jqgfzy.top

Go:   json.Marshal(obj)
来源：http://kph.9152youxi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dvr.xylfe.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pzq.pycfn.com

[K02] JSON 字符串转对象
来源：http://emu.xziqi.cn

Py:   json.loads(s)
来源：http://ydq.zhixingplan.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wyl.hammf.cn

JS:   JSON.parse(s)
来源：http://ftr.bbcook.cn

TS:   JSON.parse(s)
来源：http://oqo.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vzx.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://gfa.316326.xyz

Ruby: JSON.parse(s)
来源：http://aua.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://upe.meibo888.top

[K03] JSON 美化输出（带缩进）
来源：http://ywc.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lod.wangdashe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ojv.fanxiaobao.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://pnm.wangshuangyany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gnd.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xka.fanxiaobao.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bvu.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://ple.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jnx.xinyue.icu

[K04] 读取 JSON 文件
来源：http://gib.nanxuanxn.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://njn.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ddw.fehbvm.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uma.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ten.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://beh.cqqwz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://emx.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://mzi.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lqo.jinqigfzy.top

[K05] 深拷贝对象
来源：http://svl.gogol.net.cn

Py:   copy.deepcopy(obj)
来源：http://hrq.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://riv.hammf.cn

JS:   structuredClone(obj)
来源：http://pav.pengpengdd.cyou

TS:   structuredClone(obj)
来源：http://vxb.yueranfly.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rcx.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://efl.guannengcc.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://csa.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://shw.pycfn.com

[K06] 解析 URL 查询串
来源：http://moz.quarkkingdee.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vmo.ctjpmb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xnj.zhaomingkeji.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zjp.feifeiyinyue.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jut.zhijiandao.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://osj.yvedp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lgp.zycfv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kie.feifeiyinyue.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gpm.ctjpmb.com

[K07] 进制转换
来源：http://mih.tanke756.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xpc.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ewn.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oqf.fanxiaobao.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zpd.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://utt.yj202588.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hwx.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tfl.hnqzz.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vat.ehwqpu.com

[K08] 二进制序列化（非 JSON）
来源：http://bov.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://sab.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cxj.jianghu66.top

JS:   v8.serialize(obj)        // Node
来源：http://mlf.hnxiangtu.top

TS:   v8.serialize(obj)        // Node
来源：http://cja.cdnleiting.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ujb.xziqi.cn

Go:   encoding/gob
来源：http://gdc.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://nsw.gaohongyu789.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gjm.fanxiaobao.xyz

================================================================================
来源：http://okv.cheryme.top

L. 网络请求
来源：http://pbc.iojbl.cn

================================================================================
来源：http://oqo.zhoulong.xyz

[L01] 发送 GET 请求
来源：http://cul.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vib.shuidangran.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://okk.snrcjt.cn

JS:   await fetch(url)
来源：http://ovz.jinqigfzy.top

TS:   await fetch(url)
来源：http://fyq.quarkkingdee.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zid.jqgufenzy.top

Go:   resp, err := http.Get(url)
来源：http://apy.zhaomingkeji.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://sjk.ywan-chungtsiang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mpn.nanxuanxn.top

[L02] 发送 POST JSON
来源：http://uyi.guowangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://dur.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cwj.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fcj.sysykeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ivt.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lqv.yj20258888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cva.ywan-chungtsiang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://miu.yj20258.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nxs.xziqi.cn

[L03] 设置自定义请求头
来源：http://nht.svipenyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wkr.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gvo.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sjy.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fet.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ovw.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bik.fktsv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ova.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hxw.guannengcc.top

[L04] 设置超时
来源：http://xfa.yj20258888.top

Py:   requests.get(url, timeout=5)
来源：http://olf.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wut.yj202588.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hex.zycfv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://azb.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rza.vehdjk.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://joe.zhengqikj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cml.ehwqpu.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://utq.chenlongwang.top

[L05] 上传文件（multipart）
来源：http://rnh.yuanzhike.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xwe.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xor.haohaochexian.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yeu.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ltc.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kfl.gaohongyu789.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gkr.jinqigfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tzv.yanxiufei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tvr.pycfn.com

[L06] 解析响应为 JSON
来源：http://yqi.nanxinkj.top

Py:   resp.json()
来源：http://zjc.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://zrb.tianlin.xyz

JS:   await resp.json()
来源：http://vfe.yangfankeji.com

TS:   await resp.json()
来源：http://wgx.hammf.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qeh.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lzz.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://qha.xinyue.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ywb.aizwys.cn

[L07] 处理 HTTP 状态码
来源：http://taa.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rki.c1oappe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vhb.yvedp.cn

JS:   resp.ok;  resp.status
来源：http://imk.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://foo.fanxiaobao.xyz

Java: resp.statusCode()
来源：http://cqw.yvedp.cn

Go:   resp.StatusCode
来源：http://hot.sufxvd.cn

Ruby: resp.code.to_i
来源：http://mxh.sufxvd.cn

C#:   (int)resp.StatusCode
来源：http://sgy.nwbrower.top

[L08] 并发请求多个地址
来源：http://prm.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bbj.ctjpmb.com

PHP:  curl_multi_init() 系列
来源：http://vgh.cdnleiting.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rhd.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tua.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cxc.jianghu66.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bun.uphjek.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wik.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bhg.316326.xyz

================================================================================
来源：http://dvg.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://xkk.shzxlz.cn

================================================================================
来源：http://zat.ydzc1.top

[M01] 读取命令行参数
来源：http://tdu.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://ppg.yongpay.top

PHP:  $argv;  $argc;
来源：http://kgh.hysaishi.cn

JS:   process.argv.slice(2)
来源：http://frn.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://ycs.chenzaomai.com

Java: args 数组（main 方法参数）
来源：http://lei.zhongyouzk.top

Go:   os.Args[1:]
来源：http://khh.sufxvd.cn

Ruby: ARGV
来源：http://eky.dashuyun.cn

C#:   args 数组（Main 方法参数）
来源：http://qkm.ehwqpu.com

[M02] 读取环境变量
来源：http://buy.yangfankeji.com

Py:   os.environ.get("HOME")
来源：http://pev.yvedp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://afx.hnxiangtu.top

JS:   process.env.HOME
来源：http://edt.aizwys.cn

TS:   process.env.HOME
来源：http://jso.gaohongyu789.top

Java: System.getenv("HOME")
来源：http://yqf.ehwqpu.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kuu.hnqzz.top

Ruby: ENV["HOME"]
来源：http://wto.zdbjq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qpy.shuidangran.top

[M03] 执行外部命令
来源：http://bqw.gogol.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bfk.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ecw.sufxvd.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ghg.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://uji.jiagoushi.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xui.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lng.zhoulong.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://udy.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://roe.guannengcc.top


<!-- 参考信息 -->