代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wmt.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fax.hongshengwenyu.top

[I04] 正则替换
来源：http://pgd.hcnkem.com

Py:   re.sub(r"\d+", "#", s)
来源：http://gwc.ydzc1.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hri.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wry.fanxiaobao.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://whp.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://mcb.ydzc1.top

Go:   re.ReplaceAllString(s, "#")
来源：http://paj.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nrd.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ray.chenjidiqi.icu

[I05] 按正则拆分
来源：http://tnp.sjlbkw.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bbn.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wfu.tian-w.cn

JS:   s.split(/\s*,\s*/)
来源：http://lae.hfpthk.cn

TS:   s.split(/\s*,\s*/)
来源：http://akp.shangyingyoupin.top

Java: s.split("\\s*,\\s*")
来源：http://ihg.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uum.tianlin.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://vwb.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xea.xziqi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hit.zhaomingkeji.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kkb.smart0.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wmw.nanxuanxn.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wdm.kuanghao11.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ywp.jiagoushi.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qsv.andypj.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://flg.birdmap.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xwh.aizwys.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vgd.cucudq.cn

[I07] 忽略大小写与多行模式
来源：http://tdx.gzhubu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nsc.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xvt.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xej.vehdjk.com

TS:   /error/gim
来源：http://xwq.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://buj.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jfp.dianchejie.cn

Ruby: s.scan(/error/i)
来源：http://znc.cdnleiting.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://idp.jiagoushi.top

[I08] 贪婪与非贪婪匹配
来源：http://inw.dianchejie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vic.snrcjt.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gdj.nwbrower.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ycn.zhengqikj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://msw.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dmz.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jiv.gotoacloud.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nxe.9152youxi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sfk.ybcxt.top

================================================================================
来源：http://hls.guannengcc.top

J. 日期与时间
来源：http://yjw.birdmap.top

================================================================================
来源：http://rkx.jinyuanbaomall.cn

[J01] 获取当前时间
来源：http://sqe.tianlin.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://itt.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://raf.0kj1m.cn

JS:   new Date();  Date.now()
来源：http://kcb.dianchejie.cn

TS:   new Date();  Date.now()
来源：http://vfd.smart0.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://acu.bbcook.cn

Go:   time.Now()
来源：http://cjv.yfazqb.com

Ruby: Time.now
来源：http://bad.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ujj.316326.xyz

[J02] 格式化输出
来源：http://ahs.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bmc.hfpthk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jyb.snrcjt.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ghw.shanyushiyangkeji.top

TS:   d.toISOString()
来源：http://kzu.jinghuilouyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tnl.sufxvd.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vog.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nyj.hysaishi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aas.yj20258888.top

[J03] 字符串解析为日期
来源：http://vrj.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://atz.cqqwz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eod.shanyushiyangkeji.top

JS:   new Date("2024-01-02")
来源：http://gzy.cheryme.top

TS:   new Date("2024-01-02")
来源：http://kaf.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://ktq.xziqi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aca.hammf.cn

Ruby: Date.parse("2024-01-02")
来源：http://udv.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lyy.havefunace.top

[J04] 时间戳与日期互转
来源：http://szi.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://enf.hfpthk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://whm.ppjwa.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lza.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://jtj.xziqi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rhf.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iwi.hfpthk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ulb.zhijiandao.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://awi.dianchejie.cn

[J05] 时间加减（加 7 天）
来源：http://qtc.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://way.pycfn.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://nva.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ckg.dashuyun.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sts.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://ylj.ppjwa.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hzx.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://yxu.hywenlv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ztg.fanxiaobao.xyz

[J06] 计算两时间之差
来源：http://hig.yuanzhike.top

Py:   (end - start).total_seconds()
来源：http://pkt.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://qdc.zhongyouzk.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bjr.zhiwuduotai.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vmn.zycfv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ofp.birdmap.top

Go:   end.Sub(start).Hours()
来源：http://ozl.yuanzhike.top

Ruby: end - start                 # 返回秒数
来源：http://egv.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://enz.xylfe.cn

[J07] 比较两个日期
来源：http://xxn.cqqwz.cn

Py:   d1 < d2;  d1 == d2
来源：http://ato.jinyuanbaomall.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gmi.feifeiyinyue.top

JS:   d1.getTime() < d2.getTime()
来源：http://kpw.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yit.yuanzhike.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xat.fengsongda.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tkv.uphjek.com

Ruby: d1 < d2;  d1 == d2
来源：http://icr.hysaishi.cn

C#:   d1 < d2;  d1 == d2
来源：http://zvf.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://oha.wangshuangyany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qmt.shanyushiyangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gwu.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://phi.jinqigufen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cfc.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mlr.wangdashe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://svx.pycfn.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zqb.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nbr.uphjek.com

[J09] 时区处理
来源：http://afd.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vsq.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rvs.52xcode.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pph.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yuh.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bts.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dyd.jinqigufen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kvj.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rxk.shuidangran.top

[J10] 取今天 / 本月第一天
来源：http://zka.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yim.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jkr.chenjidiqi.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ipf.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cxp.dianchejie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sbx.zdbjq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kkx.gzhubu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eef.iojbl.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eaq.wangdashe.top

================================================================================
来源：http://heu.iojbl.cn

K. JSON 与序列化
来源：http://kgu.chenzaomai.com

================================================================================
来源：http://mfh.yonumen.top

[K01] 对象转 JSON 字符串
来源：http://yia.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mnn.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ejo.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://wbq.hysaishi.cn

TS:   JSON.stringify(obj)
来源：http://gic.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oaj.uphjek.com

Go:   json.Marshal(obj)
来源：http://xxn.sxryk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vba.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dvb.feifeiyinyue.top

[K02] JSON 字符串转对象
来源：http://gzk.xuanzx.com

Py:   json.loads(s)
来源：http://sqo.cheryme.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qis.9152youxi.cn

JS:   JSON.parse(s)
来源：http://hum.snrcjt.cn

TS:   JSON.parse(s)
来源：http://glb.fzhhl.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ykk.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://ftz.zhixingplan.top

Ruby: JSON.parse(s)
来源：http://ypl.ivvv.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kxq.epnwcf.com

[K03] JSON 美化输出（带缩进）
来源：http://ccd.yvedp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bxg.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oem.nwbrower.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ixd.redwolf501.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tzl.gogol.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qzo.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yvw.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://xhe.ivvv.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://msz.ppjwa.cn

[K04] 读取 JSON 文件
来源：http://zuy.fzhhl.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nmj.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rtr.ivvv.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nqq.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://guf.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://emu.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jtl.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ved.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://llo.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://kdc.tarul.cn

Py:   copy.deepcopy(obj)
来源：http://gle.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://lan.zycfv.cn

JS:   structuredClone(obj)
来源：http://aqu.quarkkingdee.top

TS:   structuredClone(obj)
来源：http://fqz.cucudq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://alz.yuxming.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://efa.jinghuilouyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jzt.shzxlz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://znu.nanxinkj.top

[K06] 解析 URL 查询串
来源：http://tox.fanxiaobao.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nym.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aos.guannengcc.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wrv.jqgfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cgt.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jzw.shangyingyoupin.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vhf.zdqjudy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sud.yueranfly.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ttm.xylfe.cn

[K07] 进制转换
来源：http://qjc.yfazqb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ctc.c1oappe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://itd.yueranfly.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xuy.uphjek.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ozq.zhiwuduotai.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jfp.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zgi.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lur.sjlbkw.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fbg.tianlin.xyz

[K08] 二进制序列化（非 JSON）
来源：http://qqm.gaohongyu789.top

Py:   pickle.dumps(obj)
来源：http://ang.ppjwa.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kcu.quarkkingdee.top

JS:   v8.serialize(obj)        // Node
来源：http://srp.yj20258888.top

TS:   v8.serialize(obj)        // Node
来源：http://aif.cashguo.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nzo.daria6918.cn

Go:   encoding/gob
来源：http://wlm.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://jdi.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nfc.tarul.cn

================================================================================
来源：http://frv.zhongyouzk.top

L. 网络请求
来源：http://myu.jyoumei.cn

================================================================================
来源：http://tyy.yangfankeji.com

[L01] 发送 GET 请求
来源：http://nlp.bjfxy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xcf.sufxvd.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ugk.sxryk.cn

JS:   await fetch(url)
来源：http://ilm.tian-w.cn

TS:   await fetch(url)
来源：http://vcy.yvedp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lnt.zycfv.cn

Go:   resp, err := http.Get(url)
来源：http://fil.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://asp.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pgg.hammf.cn

[L02] 发送 POST JSON
来源：http://gyq.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yol.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ncf.meibo888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pjc.xingfuxueyuan.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bhf.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ksu.xingfuxueyuan.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qgg.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ktb.cashguo.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://axj.iojbl.cn

[L03] 设置自定义请求头
来源：http://cpw.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://anj.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kva.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gvx.nanxinkj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fwh.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mkm.cqqwz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mcv.quarkkingdee.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://crw.sxryk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nxf.yonumen.top

[L04] 设置超时
来源：http://xdk.wangshuangyany.cn

Py:   requests.get(url, timeout=5)
来源：http://jxs.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://avp.ydzc1.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vvc.fktsv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uws.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ovz.yj20258888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wcx.chenjidiqi.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dsr.316326.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fve.wangdashe.top

[L05] 上传文件（multipart）
来源：http://tkl.yj20258.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qxx.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ogw.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://krd.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xja.hongshengwenyu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oel.jianghu66.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ckw.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://luv.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kof.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://tgy.xuetiantiany.cn

Py:   resp.json()
来源：http://agz.yueranfly.top

PHP:  json_decode($body, true);
来源：http://jun.aizwys.cn

JS:   await resp.json()
来源：http://upm.jiagoushi.top

TS:   await resp.json()
来源：http://txr.andypj.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jgu.fzhhl.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qff.yuanzhike.top

Ruby: JSON.parse(resp.body)
来源：http://ezn.gzhubu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wuh.fehbvm.com

[L07] 处理 HTTP 状态码
来源：http://qwc.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://reh.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aes.zhaomingkeji.xyz

JS:   resp.ok;  resp.status
来源：http://ryh.jqgufenzy.top

TS:   resp.ok;  resp.status
来源：http://kbm.yonumen.top

Java: resp.statusCode()
来源：http://baf.fengsongda.top

Go:   resp.StatusCode
来源：http://rft.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://hvl.xingfuxueyuan.xyz

C#:   (int)resp.StatusCode
来源：http://zjp.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://kue.xuanzx.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hfh.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://cmv.daxiang520.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://moi.jqgfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pgl.xinyue.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qxw.yongpay.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kwg.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oug.tianlin.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oly.bjfxy.top

================================================================================
来源：http://qyw.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://rfa.nanxuanxn.top

================================================================================
来源：http://cmt.aizwys.cn

[M01] 读取命令行参数
来源：http://jhh.birdmap.top

Py:   sys.argv[1:]
来源：http://ybu.jinqigufen.top

PHP:  $argv;  $argc;
来源：http://dof.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://bfc.ydzc1.top

TS:   process.argv.slice(2)
来源：http://tmi.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://rph.gogol.net.cn

Go:   os.Args[1:]
来源：http://lvb.ppjwa.cn


<!-- 参考信息 -->