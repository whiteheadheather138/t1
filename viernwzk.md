代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://eav.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hmf.gotoacloud.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://osu.yuanzhike.top

[I05] 按正则拆分
来源：http://vze.hcnkem.com

Py:   re.split(r"\s*,\s*", s)
来源：http://hyj.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://omn.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://xul.uphjek.com

TS:   s.split(/\s*,\s*/)
来源：http://gjv.hnqzz.top

Java: s.split("\\s*,\\s*")
来源：http://dse.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mnl.hfpthk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wuu.svipenyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jfc.hesvh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hcd.cheryme.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yvp.hammf.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://thb.9152youxi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qpj.fzhhl.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pkv.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ysx.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xfo.havefunace.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://abj.0kj1m.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pob.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://scf.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fsg.aizwys.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dcn.hnxiangtu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yog.xziqi.cn

TS:   /error/gim
来源：http://jmf.jinghuilouyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cjy.snrcjt.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://npg.fehbvm.com

Ruby: s.scan(/error/i)
来源：http://zqk.smart0.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sft.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://qrj.chenzaomai.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tvy.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tzi.xingfuxueyuan.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gwz.redwolf501.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://efe.mhx1999.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://woz.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dop.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xwy.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://efz.ydzc1.top

================================================================================
来源：http://wrk.iojbl.cn

J. 日期与时间
来源：http://wlj.jqgufenzy.top

================================================================================
来源：http://dkb.smart0.xyz

[J01] 获取当前时间
来源：http://ofx.gotoacloud.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cof.zhiwuduotai.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xum.zhongyouzk.top

JS:   new Date();  Date.now()
来源：http://mud.guannengcc.top

TS:   new Date();  Date.now()
来源：http://cqq.havefunace.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ngx.jinghuilouyu.cn

Go:   time.Now()
来源：http://hfv.andypj.xyz

Ruby: Time.now
来源：http://wmw.c1oappe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jbs.yuxming.cn

[J02] 格式化输出
来源：http://ipz.gaohongyu789.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mvh.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hge.havefunace.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cms.yuxming.cn

TS:   d.toISOString()
来源：http://zuk.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rcg.cucudq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jkw.yangfankeji.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nqm.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nsx.xingfuxueyuan.xyz

[J03] 字符串解析为日期
来源：http://zty.nanxuanxn.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uyz.jqgfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sby.9152youxi.cn

JS:   new Date("2024-01-02")
来源：http://txy.meibo888.top

TS:   new Date("2024-01-02")
来源：http://ktm.daxiang520.top

Java: LocalDate.parse("2024-01-02")
来源：http://tru.wangdashe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://agc.hywenlv.cn

Ruby: Date.parse("2024-01-02")
来源：http://isp.hesvh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wan.zhaomingkeji.xyz

[J04] 时间戳与日期互转
来源：http://oja.ctjpmb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vqg.yanxiufei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wol.cdnleiting.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kkn.wangshuangyany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jmn.jyoumei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blf.yueranfly.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://byr.tianlin.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://phz.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ice.ivvv.top

[J05] 时间加减（加 7 天）
来源：http://lph.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://pqi.cucudq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kwo.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kor.hcnkem.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tju.haohaochexian.top

Java: LocalDate.now().plusDays(7)
来源：http://hbn.yuanzhike.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pup.xylfe.cn

Ruby: Time.now + 7 * 86400
来源：http://zdv.gzhubu.top

C#:   DateTime.Now.AddDays(7)
来源：http://wpl.tianlin.xyz

[J06] 计算两时间之差
来源：http://bkn.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://mbn.wangshuangyany.cn

PHP:  $end->diff($start)->days;
来源：http://qnt.sjlbkw.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://drd.ybcxt.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aww.quarkkingdee.top

Java: Duration.between(start, end).toSeconds()
来源：http://jru.yuxming.cn

Go:   end.Sub(start).Hours()
来源：http://ypn.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://wyu.guannengcc.top

C#:   (end - start).TotalSeconds
来源：http://buo.zdqjudy.top

[J07] 比较两个日期
来源：http://dsm.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://glq.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iyu.wangdashe.top

JS:   d1.getTime() < d2.getTime()
来源：http://rvq.zhongyouzk.top

TS:   d1.getTime() < d2.getTime()
来源：http://qtg.jqgfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pxg.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bby.zhongyouzk.top

Ruby: d1 < d2;  d1 == d2
来源：http://qso.hcnkem.com

C#:   d1 < d2;  d1 == d2
来源：http://dal.yangfankeji.com

[J08] 提取年月日与星期
来源：http://qoo.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rnp.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kjr.tarul.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gow.316326.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://duq.zhongyouzk.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://auv.cheryme.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zuu.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://atv.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tfx.316326.xyz

[J09] 时区处理
来源：http://pcf.xuanzx.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xhd.pengpengdd.cyou

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ynr.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lsq.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cdy.cqqwz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://smf.chenlongwang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dty.redwolf501.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lgb.tanke756.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wlt.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://nyw.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bwi.c1oappe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sxp.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://epg.snrcjt.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wqb.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ujz.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cfl.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sny.ydzc1.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xmd.hnxiangtu.top

================================================================================
来源：http://uip.kuanghao11.cn

K. JSON 与序列化
来源：http://tco.zhiwuduotai.top

================================================================================
来源：http://cit.fzhhl.top

[K01] 对象转 JSON 字符串
来源：http://jni.zhixingplan.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bdy.jqgfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ryg.ivvv.top

JS:   JSON.stringify(obj)
来源：http://kdd.jinyuanbaomall.cn

TS:   JSON.stringify(obj)
来源：http://czr.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://env.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://uab.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://qps.hammf.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xcw.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://tvi.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://mxu.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cno.gogol.net.cn

JS:   JSON.parse(s)
来源：http://oed.zhiwuduotai.top

TS:   JSON.parse(s)
来源：http://tzq.ctjpmb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kzn.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://hdw.hywenlv.cn

Ruby: JSON.parse(s)
来源：http://pgw.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rof.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://icx.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oua.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hte.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ino.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fal.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jzn.shanyushiyangtech.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://udy.yuxming.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uib.nwbrower.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gnj.ppjwa.cn

[K04] 读取 JSON 文件
来源：http://ycc.fanxiaobao.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xwx.pengpengdd.cyou

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://typ.nwbrower.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://thd.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qgl.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ehp.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aol.sysykeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mvj.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lkp.zhongyouzk.top

[K05] 深拷贝对象
来源：http://ejr.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://hye.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://bai.feifeiyinyue.top

JS:   structuredClone(obj)
来源：http://kxk.gogol.net.cn

TS:   structuredClone(obj)
来源：http://mam.nanxuanxn.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pgm.ybcxt.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bto.hcnkem.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://umy.c1oappe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zbf.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://fny.yuanzhike.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jqd.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eeh.yuanzhike.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zqd.uphjek.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://frb.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nsl.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pcq.bbcook.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cir.epnwcf.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pti.ppjwa.cn

[K07] 进制转换
来源：http://brj.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dkk.chenzaomai.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ulo.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ipr.ppjwa.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://atx.zhengqikj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dmh.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dbo.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ibh.sjlbkw.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qjy.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://pkk.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://xam.yuxming.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cnr.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://esy.gzhubu.top

TS:   v8.serialize(obj)        // Node
来源：http://mff.fanxiaobao.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nqk.yanxiufei.cn

Go:   encoding/gob
来源：http://ebi.aizwys.cn

Ruby: Marshal.dump(obj)
来源：http://lpr.hesvh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xlk.jianghu66.top

================================================================================
来源：http://bko.yuxming.cn

L. 网络请求
来源：http://nxw.52xcode.cn

================================================================================
来源：http://uhn.zycfv.cn

[L01] 发送 GET 请求
来源：http://ntj.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://alm.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jyz.zhijiandao.cn

JS:   await fetch(url)
来源：http://lhr.zhaomingkeji.xyz

TS:   await fetch(url)
来源：http://xtg.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ltu.ybcxt.top

Go:   resp, err := http.Get(url)
来源：http://ite.xuanzx.com

Ruby: Net::HTTP.get(URI(url))
来源：http://bco.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wsx.chenlongwang.top

[L02] 发送 POST JSON
来源：http://ypg.pycfn.com

Py:   requests.post(url, json={"a": 1})
来源：http://stp.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ahi.haohaochexian.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pxw.pengpengdd.cyou

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nat.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qhe.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eds.316326.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ocr.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lcy.jqgufenzy.top

[L03] 设置自定义请求头
来源：http://lyk.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://juh.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://whk.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bqn.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bov.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qsk.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://anl.nanxuanxn.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gwe.hfpthk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zuu.jlsjyb.cn

[L04] 设置超时
来源：http://jnb.zhijiandao.cn

Py:   requests.get(url, timeout=5)
来源：http://yvo.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zhc.zhengqikj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fsp.jinghuilouyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oza.nanxuanxn.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tnu.cucudq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mov.cucudq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://olw.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tqd.xylfe.cn

[L05] 上传文件（multipart）
来源：http://jst.fehbvm.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qvp.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ggf.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ico.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://glo.bbcook.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wyz.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://snf.nwbrower.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qez.snrcjt.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gsu.ehwqpu.com

[L06] 解析响应为 JSON
来源：http://jhy.ivvv.top

Py:   resp.json()
来源：http://gqs.hysaishi.cn

PHP:  json_decode($body, true);
来源：http://ekx.tanke756.top

JS:   await resp.json()
来源：http://hbm.smart0.xyz

TS:   await resp.json()
来源：http://npy.shuidangran.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mrc.hammf.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jxy.epnwcf.com

Ruby: JSON.parse(resp.body)
来源：http://mgs.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vgv.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://lmm.dianchejie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lsh.daxiang520.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fou.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://hns.aibaodan.cn

TS:   resp.ok;  resp.status
来源：http://ifk.chenlongwang.top

Java: resp.statusCode()
来源：http://kon.hcnkem.com

Go:   resp.StatusCode
来源：http://uta.haohaochexian.top

Ruby: resp.code.to_i
来源：http://dsq.iojbl.cn

C#:   (int)resp.StatusCode
来源：http://quq.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://bms.snrcjt.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://atk.iojbl.cn

PHP:  curl_multi_init() 系列
来源：http://chn.316326.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rfr.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://srt.xinyue.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nxp.0kj1m.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yst.vehdjk.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rki.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vag.tarul.cn

================================================================================
来源：http://qca.sysykeji.top

M. 命令行 / 进程 / 环境
来源：http://qlk.gzhubu.top

================================================================================
来源：http://ttx.jinghuilouyu.cn

[M01] 读取命令行参数
来源：http://ewl.yuanzhike.top

Py:   sys.argv[1:]
来源：http://esp.hnqzz.top

PHP:  $argv;  $argc;
来源：http://lwv.nanxinkj.top

JS:   process.argv.slice(2)
来源：http://soy.xuetiantiany.cn

TS:   process.argv.slice(2)
来源：http://jjs.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://qya.daxiang520.top

Go:   os.Args[1:]
来源：http://pyw.hammf.cn

Ruby: ARGV
来源：http://del.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://xxo.sweek.top

[M02] 读取环境变量
来源：http://ggh.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://yuz.nanxinkj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://isx.jinghuilouyu.cn

JS:   process.env.HOME
来源：http://ffu.shzxlz.cn

TS:   process.env.HOME
来源：http://yfz.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://zxy.quarkkingdee.top


<!-- 参考信息 -->