代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nss.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://qnr.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dxx.bbcook.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yzu.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qhs.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qxo.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nvu.zhiwuduotai.top

[I05] 按正则拆分
来源：http://niz.nanxuanxn.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gtw.nanxuanxn.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lvj.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://sib.jiagoushi.top

TS:   s.split(/\s*,\s*/)
来源：http://ywp.gaohongyu789.top

Java: s.split("\\s*,\\s*")
来源：http://yxp.zhiwuduotai.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nko.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://vyw.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qkc.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://edj.yj20258888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wjf.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://euk.vehdjk.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dza.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xvd.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tkv.tian-w.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jom.yvedp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lwx.haohaochexian.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rym.yuanzhike.top

[I07] 忽略大小写与多行模式
来源：http://eoj.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://seo.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://msv.ppjwa.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pka.haohaochexian.top

TS:   /error/gim
来源：http://pwx.zdqjudy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zao.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uaf.ywan-chungtsiang.top

Ruby: s.scan(/error/i)
来源：http://yqk.jinqigfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fiq.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://fiq.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zup.jinyuanbaomall.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://osk.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fqz.daxiang520.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://npt.cucudq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nmo.meibo888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gaa.haohaochexian.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ivq.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ruc.haohaochexian.top

================================================================================
来源：http://xfu.gotoacloud.top

J. 日期与时间
来源：http://fqb.iojbl.cn

================================================================================
来源：http://ewl.daria6918.cn

[J01] 获取当前时间
来源：http://aju.yj202588.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fbs.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sec.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://zdv.fzhhl.top

TS:   new Date();  Date.now()
来源：http://enq.nanxinkj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jgw.xziqi.cn

Go:   time.Now()
来源：http://ftj.svipenyu.cn

Ruby: Time.now
来源：http://sbk.sweek.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ldw.0kj1m.cn

[J02] 格式化输出
来源：http://yjn.chenlongwang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wyi.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://luj.zhongyouzk.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aoc.shuidangran.top

TS:   d.toISOString()
来源：http://don.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qyk.vqdsnc.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tmc.yj20258.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hbc.cashguo.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xwd.jqgfzy.top

[J03] 字符串解析为日期
来源：http://kby.hywenlv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://miy.yfazqb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pql.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://twy.hfpthk.cn

TS:   new Date("2024-01-02")
来源：http://afb.iojbl.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ddr.hammf.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gea.chenlongwang.top

Ruby: Date.parse("2024-01-02")
来源：http://eoz.daxiang520.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iau.guannengcc.top

[J04] 时间戳与日期互转
来源：http://rpz.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jxc.jianghu66.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tzn.zhixingplan.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tyw.yj202588.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pbi.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cfq.yueranfly.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fmz.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yiz.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qfw.52xcode.cn

[J05] 时间加减（加 7 天）
来源：http://fdl.yfazqb.com

Py:   now + timedelta(days=7)
来源：http://wvw.sweek.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://uvj.dianchejie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pwj.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xig.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://pvp.iojbl.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jeg.vqdsnc.cn

Ruby: Time.now + 7 * 86400
来源：http://sdb.xingfuxueyuan.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://hig.guowangkeji.top

[J06] 计算两时间之差
来源：http://ykp.daxiang520.top

Py:   (end - start).total_seconds()
来源：http://nmv.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://gvy.jinqigufen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jsz.xuanzx.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://may.jqgufenzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://grg.yj202588.top

Go:   end.Sub(start).Hours()
来源：http://abe.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://mvv.316326.xyz

C#:   (end - start).TotalSeconds
来源：http://wsy.yuxming.cn

[J07] 比较两个日期
来源：http://bum.zhongyouzk.top

Py:   d1 < d2;  d1 == d2
来源：http://ygp.svipenyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zlz.bbcook.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tss.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://dyg.yvedp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nbx.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://flq.ehwqpu.com

Ruby: d1 < d2;  d1 == d2
来源：http://csq.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://zpi.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://tiu.zdbjq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tvu.jiagoushi.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aap.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ijq.xziqi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://svw.hcnkem.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yqt.ppjwa.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zsr.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jzh.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://alq.xziqi.cn

[J09] 时区处理
来源：http://son.hammf.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mhq.jlsjyb.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://czm.jinqigfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://epg.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qyy.sjlbkw.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mzq.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://squ.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://ypm.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ezs.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://dgy.chenjidiqi.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://ypg.zhijiandao.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hbv.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jqr.xziqi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tyf.daria6918.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pze.daria6918.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uda.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sgu.vehdjk.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xeg.cqqwz.cn

================================================================================
来源：http://sei.zycfv.cn

K. JSON 与序列化
来源：http://ufw.wangdashe.top

================================================================================
来源：http://zcx.mhx1999.top

[K01] 对象转 JSON 字符串
来源：http://nox.xinyue.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eby.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jbv.zhongyouzk.top

JS:   JSON.stringify(obj)
来源：http://rsc.daria6918.cn

TS:   JSON.stringify(obj)
来源：http://tsa.mhx1999.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lds.bbcook.cn

Go:   json.Marshal(obj)
来源：http://vtm.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dlv.meibo888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qnq.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://dav.xingfuxueyuan.xyz

Py:   json.loads(s)
来源：http://clh.316326.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rgj.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://esj.aizwys.cn

TS:   JSON.parse(s)
来源：http://lid.gzhubu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jjh.zhixingplan.top

Go:   json.Unmarshal(data, &v)
来源：http://axb.9152youxi.cn

Ruby: JSON.parse(s)
来源：http://wlc.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sbi.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://mtl.redwolf501.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pvw.jqgfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://atq.sysykeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pka.cqqwz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pus.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kge.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ukr.yueranfly.top

Ruby: JSON.pretty_generate(obj)
来源：http://whm.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bmm.ivvv.top

[K04] 读取 JSON 文件
来源：http://ldu.dashuyun.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pde.yvedp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pxe.zhoulong.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uzm.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ktw.xinyue.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ufe.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oew.jianghu66.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ink.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xso.birdmap.top

[K05] 深拷贝对象
来源：http://swd.yangfankeji.com

Py:   copy.deepcopy(obj)
来源：http://sso.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://sqd.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://iqx.wangdashe.top

TS:   structuredClone(obj)
来源：http://mna.pycfn.com

Java: // 手写拷贝构造，或序列化往返
来源：http://xdu.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ksr.yuxming.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://okd.dianchejie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tvs.andypj.xyz

[K06] 解析 URL 查询串
来源：http://ahf.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nyi.9152youxi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iqb.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pni.cdnleiting.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kom.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qoe.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vis.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ugn.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kao.meibo888.top

[K07] 进制转换
来源：http://lyc.yfazqb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gkp.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ezc.hysaishi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xcb.vqdsnc.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uhx.havefunace.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hoq.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nof.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qht.ehwqpu.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kkz.cheryme.top

[K08] 二进制序列化（非 JSON）
来源：http://tbx.ctjpmb.com

Py:   pickle.dumps(obj)
来源：http://nyz.chenjidiqi.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://iil.hammf.cn

JS:   v8.serialize(obj)        // Node
来源：http://qjl.pycfn.com

TS:   v8.serialize(obj)        // Node
来源：http://ylj.316326.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uwm.nwbrower.top

Go:   encoding/gob
来源：http://jhp.yonumen.top

Ruby: Marshal.dump(obj)
来源：http://wpq.dianchejie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lkw.svipenyu.cn

================================================================================
来源：http://dea.zhaomingkeji.xyz

L. 网络请求
来源：http://prr.shangyingyoupin.top

================================================================================
来源：http://dra.0kj1m.cn

[L01] 发送 GET 请求
来源：http://dzh.feifeiyinyue.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://erl.zhoulong.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yqq.yj20258.top

JS:   await fetch(url)
来源：http://buc.ctjpmb.com

TS:   await fetch(url)
来源：http://vqd.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://htf.kuanghao11.cn

Go:   resp, err := http.Get(url)
来源：http://vfb.sweek.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cbq.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ffn.hysaishi.cn

[L02] 发送 POST JSON
来源：http://mff.epnwcf.com

Py:   requests.post(url, json={"a": 1})
来源：http://stw.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mux.meibo888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ole.bjfxy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eco.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kxx.redwolf501.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://unc.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kaf.zhengqikj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lby.vqdsnc.cn

[L03] 设置自定义请求头
来源：http://yfr.cqqwz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iad.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://edb.jianghu66.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://msx.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ciz.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tqo.sufxvd.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jke.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dtv.hfpthk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mpt.gogol.net.cn

[L04] 设置超时
来源：http://esm.sjlbkw.cn

Py:   requests.get(url, timeout=5)
来源：http://sjj.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tsa.quarkkingdee.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jfo.gogol.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jpi.xuanzx.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hhl.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wmw.zhoulong.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://czk.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xzs.fengsongda.top

[L05] 上传文件（multipart）
来源：http://cks.chenjidiqi.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hdv.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jlz.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qqx.hongshengwenyu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rws.chenzaomai.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jjf.xziqi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nyh.andypj.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oii.yanxiufei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hdo.jqgufenzy.top

[L06] 解析响应为 JSON
来源：http://hfh.fktsv.cn

Py:   resp.json()
来源：http://kbd.andypj.xyz

PHP:  json_decode($body, true);
来源：http://mvp.ywan-chungtsiang.top

JS:   await resp.json()
来源：http://raq.jinqigufen.top

TS:   await resp.json()
来源：http://xfx.fehbvm.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://umf.fzhhl.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lzv.aibaodan.cn

Ruby: JSON.parse(resp.body)
来源：http://jku.jyoumei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xhr.fanxiaobao.xyz

[L07] 处理 HTTP 状态码
来源：http://yxc.ehwqpu.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zwg.uphjek.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nau.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://nyp.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://ysn.jyoumei.cn

Java: resp.statusCode()
来源：http://wnl.shanyushiyangkeji.top

Go:   resp.StatusCode
来源：http://chm.bjfxy.top

Ruby: resp.code.to_i
来源：http://gsv.hesvh.cn

C#:   (int)resp.StatusCode
来源：http://rjy.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://pei.snrcjt.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jwq.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://gdb.yj20258.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xim.guannengcc.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://stj.jlsjyb.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pso.jinqigfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jeq.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wln.aibaodan.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hgt.xuetiantiany.cn

================================================================================
来源：http://ktw.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://ctv.jinghuilouyu.cn

================================================================================
来源：http://crk.cheryme.top

[M01] 读取命令行参数
来源：http://pbh.tanke756.top

Py:   sys.argv[1:]
来源：http://fue.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://rre.shanyushiyangtech.top

JS:   process.argv.slice(2)
来源：http://kid.shuidangran.top

TS:   process.argv.slice(2)
来源：http://wep.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://xdr.cheryme.top

Go:   os.Args[1:]
来源：http://dfe.ppjwa.cn

Ruby: ARGV
来源：http://wuy.svipenyu.cn

C#:   args 数组（Main 方法参数）
来源：http://sfr.uphjek.com

[M02] 读取环境变量
来源：http://kna.jinyuanbaomall.cn

Py:   os.environ.get("HOME")
来源：http://mvz.quarkkingdee.top


<!-- 参考信息 -->