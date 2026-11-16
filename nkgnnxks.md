代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://ugs.fktsv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iow.zdbjq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ecp.zhengqikj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ewx.dianchejie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sxq.zdqjudy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hqw.ybcxt.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ueb.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zxy.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bhm.daxiang520.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rhj.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ppd.hcnkem.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wnf.guannengcc.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zib.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://roq.sweek.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://khz.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jxi.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://roi.sufxvd.cn

TS:   /error/gim
来源：http://afb.xuanzx.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sad.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jap.zdbjq.cn

Ruby: s.scan(/error/i)
来源：http://dxn.ydjk.org.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://chg.vehdjk.com

[I08] 贪婪与非贪婪匹配
来源：http://vtq.hongshengwenyu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sic.c1oappe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qjz.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rcs.sufxvd.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ipg.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tue.xingfuxueyuan.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uav.yuanzhike.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gpd.nanxuanxn.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://usr.ehwqpu.com

================================================================================
来源：http://mhe.sjlbkw.cn

J. 日期与时间
来源：http://cur.pengpengdd.cyou

================================================================================
来源：http://zak.shangyingyoupin.top

[J01] 获取当前时间
来源：http://zcm.dashuyun.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tun.cqqwz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nxe.sysykeji.top

JS:   new Date();  Date.now()
来源：http://nvu.fanxiaobao.xyz

TS:   new Date();  Date.now()
来源：http://anb.yj20258.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mef.ivvv.top

Go:   time.Now()
来源：http://puw.quarkkingdee.top

Ruby: Time.now
来源：http://hvc.gotoacloud.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ufc.shanyushiyangkeji.top

[J02] 格式化输出
来源：http://utx.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oee.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tjf.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://flr.jinqigufen.top

TS:   d.toISOString()
来源：http://kyd.0kj1m.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gkp.ydzc1.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eaa.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jpu.guowangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oxm.aizwys.cn

[J03] 字符串解析为日期
来源：http://fhq.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bqo.xuetiantiany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nus.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://psw.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://brb.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://ejq.bbcook.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://siy.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://icj.zdbjq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mhq.cashguo.top

[J04] 时间戳与日期互转
来源：http://osa.aizwys.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qqo.vehdjk.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vja.tian-w.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://icz.tian-w.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rnp.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ngq.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cvq.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zdi.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sox.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://swc.yuxming.cn

Py:   now + timedelta(days=7)
来源：http://zly.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vdj.hesvh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tft.hammf.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xby.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://irf.shanyushiyangtech.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mog.fanxiaobao.xyz

Ruby: Time.now + 7 * 86400
来源：http://sqe.kuanghao11.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nwk.birdmap.top

[J06] 计算两时间之差
来源：http://ynf.yvedp.cn

Py:   (end - start).total_seconds()
来源：http://yek.aizwys.cn

PHP:  $end->diff($start)->days;
来源：http://dsr.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tja.jinqigfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bzr.zhixingplan.top

Java: Duration.between(start, end).toSeconds()
来源：http://qlk.ybcxt.top

Go:   end.Sub(start).Hours()
来源：http://cnp.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://ncd.yj20258888.top

C#:   (end - start).TotalSeconds
来源：http://qnf.gaohongyu789.top

[J07] 比较两个日期
来源：http://mns.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://zva.guowangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pqb.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://ack.xuanzx.com

TS:   d1.getTime() < d2.getTime()
来源：http://zsu.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rcb.ppjwa.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fdc.vqdsnc.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tdm.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://kjz.xingfuxueyuan.xyz

[J08] 提取年月日与星期
来源：http://yxu.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qfk.epnwcf.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kbx.yuxming.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qrj.redwolf501.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mke.yuanzhike.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vsb.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dul.hysaishi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hiu.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dsp.guowangkeji.top

[J09] 时区处理
来源：http://oxj.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lyw.vqdsnc.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nuw.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://prx.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mix.ydzc1.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://erb.jyoumei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wmn.sxryk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://atk.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://twn.fktsv.cn

[J10] 取今天 / 本月第一天
来源：http://imu.yangfankeji.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ahc.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gdn.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vam.gogol.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rph.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vcy.mhx1999.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xjh.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sax.redwolf501.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://csf.feifeiyinyue.top

================================================================================
来源：http://hvy.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://vti.cucudq.cn

================================================================================
来源：http://gqj.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://zbc.andypj.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pyo.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yfe.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://xch.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://qtx.hesvh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jcf.yj20258888.top

Go:   json.Marshal(obj)
来源：http://caw.vqdsnc.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rre.nwbrower.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bay.ydjk.org.cn

[K02] JSON 字符串转对象
来源：http://egl.tarul.cn

Py:   json.loads(s)
来源：http://ktd.bjfxy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fsr.zhixingplan.top

JS:   JSON.parse(s)
来源：http://aym.yuxming.cn

TS:   JSON.parse(s)
来源：http://qpg.redwolf501.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zkk.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://rns.xuanzx.com

Ruby: JSON.parse(s)
来源：http://wrc.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://odu.fengsongda.top

[K03] JSON 美化输出（带缩进）
来源：http://ofb.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xim.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ddt.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://njs.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://siz.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://okr.ybcxt.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eme.jlsjyb.cn

Ruby: JSON.pretty_generate(obj)
来源：http://esm.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://frg.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://tai.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nfo.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kwx.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nuv.sxryk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tix.zhaomingkeji.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gqn.aizwys.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://acu.yj202588.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kpv.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gsk.guannengcc.top

[K05] 深拷贝对象
来源：http://jdc.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://qrj.tian-w.cn

PHP:  unserialize(serialize($obj));
来源：http://qng.cashguo.top

JS:   structuredClone(obj)
来源：http://feg.jiagoushi.top

TS:   structuredClone(obj)
来源：http://keu.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://krf.shangyingyoupin.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wny.daxiang520.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ixe.fengsongda.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ozj.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://owg.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ank.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bev.ydzc1.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cmj.svipenyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://htd.nanxinkj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://snz.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://qeo.tian-w.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xhh.chenzaomai.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aqu.jinghuilouyu.cn

[K07] 进制转换
来源：http://gnb.chenlongwang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kvv.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ufe.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lpy.jqgfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://poo.cashguo.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://owk.jianghu66.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://okw.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://toq.guannengcc.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://suu.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://cfi.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://tbc.zhiwuduotai.top

PHP:  serialize($obj);  unserialize($s);
来源：http://txe.cqqwz.cn

JS:   v8.serialize(obj)        // Node
来源：http://qiu.yfazqb.com

TS:   v8.serialize(obj)        // Node
来源：http://jyq.fehbvm.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fjx.cucudq.cn

Go:   encoding/gob
来源：http://gri.hongshengwenyu.top

Ruby: Marshal.dump(obj)
来源：http://mnn.yuanzhike.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hnx.chenzaomai.com

================================================================================
来源：http://mse.uphjek.com

L. 网络请求
来源：http://snw.guannengcc.top

================================================================================
来源：http://zpe.ehwqpu.com

[L01] 发送 GET 请求
来源：http://zno.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rzt.316326.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ukf.quarkkingdee.top

JS:   await fetch(url)
来源：http://aym.shuidangran.top

TS:   await fetch(url)
来源：http://dgs.iojbl.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tby.fanxiaobao.xyz

Go:   resp, err := http.Get(url)
来源：http://sbg.ppjwa.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fdc.shanyushiyangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bbv.hcnkem.com

[L02] 发送 POST JSON
来源：http://rvj.guannengcc.top

Py:   requests.post(url, json={"a": 1})
来源：http://rzi.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://few.yj20258.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jef.haohaochexian.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fdu.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wlt.pycfn.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cqg.ppjwa.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fba.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yll.sufxvd.cn

[L03] 设置自定义请求头
来源：http://sky.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rtp.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rjv.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oml.fehbvm.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hai.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ake.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fxy.zdbjq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lql.fehbvm.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cdm.hnxiangtu.top

[L04] 设置超时
来源：http://rfr.ybcxt.top

Py:   requests.get(url, timeout=5)
来源：http://uhp.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ddf.zhixingplan.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fne.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jvc.sjlbkw.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hvf.daria6918.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tpc.gzhubu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ofq.xziqi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dru.cashguo.top

[L05] 上传文件（multipart）
来源：http://pfc.yangfankeji.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://unj.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gqt.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lma.chenlongwang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://upv.yvedp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yoh.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://swk.yanxiufei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jre.nanxuanxn.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jkk.tanke756.top

[L06] 解析响应为 JSON
来源：http://igs.zhaomingkeji.xyz

Py:   resp.json()
来源：http://fkz.yj20258.top

PHP:  json_decode($body, true);
来源：http://use.daria6918.cn

JS:   await resp.json()
来源：http://cfv.jqgufenzy.top

TS:   await resp.json()
来源：http://rle.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pim.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iyp.yj202588.top

Ruby: JSON.parse(resp.body)
来源：http://njl.zhoulong.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://orw.chenjidiqi.icu

[L07] 处理 HTTP 状态码
来源：http://plz.yanxiufei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ott.ywan-chungtsiang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wjl.nwbrower.top

JS:   resp.ok;  resp.status
来源：http://tlc.nwbrower.top

TS:   resp.ok;  resp.status
来源：http://zqu.yfazqb.com

Java: resp.statusCode()
来源：http://epa.316326.xyz

Go:   resp.StatusCode
来源：http://agg.xuanzx.com

Ruby: resp.code.to_i
来源：http://ajg.wangshuangyany.cn

C#:   (int)resp.StatusCode
来源：http://kcc.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://qrd.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lqp.cucudq.cn

PHP:  curl_multi_init() 系列
来源：http://rqf.dianchejie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xqu.yonumen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hnl.yuanzhike.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fwq.sjlbkw.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tkg.pycfn.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aiy.ctjpmb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cri.tarul.cn

================================================================================
来源：http://czk.xziqi.cn

M. 命令行 / 进程 / 环境
来源：http://wvo.shzxlz.cn

================================================================================
来源：http://lwd.epnwcf.com

[M01] 读取命令行参数
来源：http://glx.gzhubu.top

Py:   sys.argv[1:]
来源：http://wlw.xinyue.icu

PHP:  $argv;  $argc;
来源：http://nne.xylfe.cn

JS:   process.argv.slice(2)
来源：http://iye.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://olb.xingfuxueyuan.xyz

Java: args 数组（main 方法参数）
来源：http://fyo.52xcode.cn

Go:   os.Args[1:]
来源：http://pql.shuidangran.top

Ruby: ARGV
来源：http://yla.yfazqb.com

C#:   args 数组（Main 方法参数）
来源：http://oiy.bjfxy.top

[M02] 读取环境变量
来源：http://yuj.fzhhl.top

Py:   os.environ.get("HOME")
来源：http://seh.andypj.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cdy.jinqigfzy.top

JS:   process.env.HOME
来源：http://qkv.dianchejie.cn

TS:   process.env.HOME
来源：http://lpj.zhoulong.xyz

Java: System.getenv("HOME")
来源：http://thf.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uzx.jqgufenzy.top

Ruby: ENV["HOME"]
来源：http://nab.sweek.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zrx.0kj1m.cn

[M03] 执行外部命令
来源：http://inf.sjlbkw.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://paf.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eaa.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gyl.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tnq.ybcxt.top


<!-- 参考信息 -->