代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://izz.fengsongda.top

[I03] 提取捕获分组
来源：http://ahe.aibaodan.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yim.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tou.bbcook.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uyp.jyoumei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oyg.iojbl.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://itz.cucudq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://efv.cheryme.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rof.zhoulong.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pbf.ehwqpu.com

[I04] 正则替换
来源：http://qya.sufxvd.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ouz.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wtm.gzhubu.top

JS:   s.replace(/\d+/g, "#")
来源：http://amr.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://wsm.zhijiandao.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xoj.fehbvm.com

Go:   re.ReplaceAllString(s, "#")
来源：http://qmq.hongshengwenyu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://whq.iojbl.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tjy.jinyuanbaomall.cn

[I05] 按正则拆分
来源：http://due.jqgufenzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cea.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rju.zhengqikj.top

JS:   s.split(/\s*,\s*/)
来源：http://ajf.chenzaomai.com

TS:   s.split(/\s*,\s*/)
来源：http://xfi.hnxiangtu.top

Java: s.split("\\s*,\\s*")
来源：http://gut.hcnkem.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zdw.hammf.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gem.smart0.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ode.yfazqb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://urm.ehwqpu.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://alp.wangshuangyany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mwi.pycfn.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hcf.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://teq.uphjek.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kom.cucudq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fbk.uphjek.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://awm.shzxlz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mqh.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://hmg.jianghu66.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qvj.uphjek.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ehe.hesvh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rrm.zhongyouzk.top

TS:   /error/gim
来源：http://osu.tianlin.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://egz.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pke.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://wio.svipenyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://all.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://pun.nanxinkj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fuq.shanyushiyangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ojm.hywenlv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ywm.fehbvm.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kzg.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lur.hysaishi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fdf.xylfe.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zdw.jinqigufen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tmh.jinqigfzy.top

================================================================================
来源：http://ouz.hfpthk.cn

J. 日期与时间
来源：http://afb.hywenlv.cn

================================================================================
来源：http://hnc.iojbl.cn

[J01] 获取当前时间
来源：http://etn.xuetiantiany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ekm.uphjek.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rsf.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://uze.zhoulong.xyz

TS:   new Date();  Date.now()
来源：http://xjg.gotoacloud.top

Java: LocalDateTime.now();  Instant.now()
来源：http://khj.tarul.cn

Go:   time.Now()
来源：http://ibu.yj20258888.top

Ruby: Time.now
来源：http://mun.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ceh.hywenlv.cn

[J02] 格式化输出
来源：http://rmm.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mkb.ywan-chungtsiang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://htf.havefunace.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rra.nanxinkj.top

TS:   d.toISOString()
来源：http://oti.gotoacloud.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vkd.dashuyun.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://etm.hysaishi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ibv.zhaomingkeji.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qqe.zhengqikj.top

[J03] 字符串解析为日期
来源：http://dku.pengpengdd.cyou

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mjw.jianghu66.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qgp.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://utg.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://yph.gogol.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://heh.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://die.ydzc1.top

Ruby: Date.parse("2024-01-02")
来源：http://rby.cqqwz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vhp.cucudq.cn

[J04] 时间戳与日期互转
来源：http://zuq.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xwe.cheryme.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tks.yuanzhike.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pbx.jinyuanbaomall.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ljm.haohaochexian.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cgu.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pea.shanyushiyangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://czs.cdnleiting.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gcd.pycfn.com

[J05] 时间加减（加 7 天）
来源：http://ngx.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://ypd.wangshuangyany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yak.ctjpmb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ivi.zhijiandao.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://neh.snrcjt.cn

Java: LocalDate.now().plusDays(7)
来源：http://hcw.snrcjt.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tkz.shanyushiyangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://ban.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hcc.yfazqb.com

[J06] 计算两时间之差
来源：http://qlf.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://hng.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://bnk.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ghm.wangdashe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bnh.cashguo.top

Java: Duration.between(start, end).toSeconds()
来源：http://oww.jqgfzy.top

Go:   end.Sub(start).Hours()
来源：http://bvb.ppjwa.cn

Ruby: end - start                 # 返回秒数
来源：http://dwa.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://lgd.shangyingyoupin.top

[J07] 比较两个日期
来源：http://vhq.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://rkt.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rcy.gaohongyu789.top

JS:   d1.getTime() < d2.getTime()
来源：http://svq.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://gpo.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gmw.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dvl.cucudq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kly.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://srh.pycfn.com

[J08] 提取年月日与星期
来源：http://tcr.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eej.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://whr.ybcxt.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iif.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dxd.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kaz.quarkkingdee.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xwa.gogol.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bzy.ctjpmb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://txm.bbcook.cn

[J09] 时区处理
来源：http://alx.zhijiandao.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eyj.guowangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nef.kuanghao11.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qxi.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gen.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ekz.bbcook.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wlt.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fti.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qgj.ydjk.org.cn

[J10] 取今天 / 本月第一天
来源：http://pif.shuidangran.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hbw.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xye.jinqigfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kdo.hammf.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://huk.yuxming.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hbh.wangdashe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://scx.0kj1m.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cui.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hsx.daxiang520.top

================================================================================
来源：http://rtq.xinyue.icu

K. JSON 与序列化
来源：http://tae.fengsongda.top

================================================================================
来源：http://noo.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://kam.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fcw.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://orh.daria6918.cn

JS:   JSON.stringify(obj)
来源：http://jlc.mhx1999.top

TS:   JSON.stringify(obj)
来源：http://wem.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://npa.ydzc1.top

Go:   json.Marshal(obj)
来源：http://gun.zhaomingkeji.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://kwl.gotoacloud.top

C#:   JsonSerializer.Serialize(obj)
来源：http://quj.yfazqb.com

[K02] JSON 字符串转对象
来源：http://pyn.yj20258888.top

Py:   json.loads(s)
来源：http://qlj.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iyq.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://zgk.zdqjudy.top

TS:   JSON.parse(s)
来源：http://kuh.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bgv.chenjidiqi.icu

Go:   json.Unmarshal(data, &v)
来源：http://pbh.ydjk.org.cn

Ruby: JSON.parse(s)
来源：http://pvj.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ahl.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://yky.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rci.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qqi.9152youxi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ghu.jiagoushi.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dxi.sysykeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://atw.fzhhl.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xuu.0kj1m.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ixj.fengsongda.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://esm.uphjek.com

[K04] 读取 JSON 文件
来源：http://dls.yangfankeji.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pgw.tianlin.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ghi.xuanzx.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mgt.zhixingplan.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://imj.zdbjq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://obr.tianlin.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ktj.zdbjq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bgp.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://szz.hcnkem.com

[K05] 深拷贝对象
来源：http://auv.dashuyun.cn

Py:   copy.deepcopy(obj)
来源：http://cyx.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://syj.yfazqb.com

JS:   structuredClone(obj)
来源：http://aeh.epnwcf.com

TS:   structuredClone(obj)
来源：http://xni.zycfv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://enm.zhiwuduotai.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oxd.yangfankeji.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ayv.vqdsnc.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ecp.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://jkq.epnwcf.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pnh.hesvh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yns.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://arh.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dac.ywan-chungtsiang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://exg.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uvo.zhixingplan.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mkw.fanxiaobao.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kml.hnqzz.top

[K07] 进制转换
来源：http://iie.jyoumei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uhn.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nvy.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pva.sjlbkw.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://isv.ydjk.org.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hiv.dianchejie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mfd.ehwqpu.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://moc.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zcg.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://xpx.52xcode.cn

Py:   pickle.dumps(obj)
来源：http://wdt.jinghuilouyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xph.zhaomingkeji.xyz

JS:   v8.serialize(obj)        // Node
来源：http://tyz.xingfuxueyuan.xyz

TS:   v8.serialize(obj)        // Node
来源：http://vbf.pengpengdd.cyou

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ayo.jqgfzy.top

Go:   encoding/gob
来源：http://xwr.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://seo.hesvh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uqv.xylfe.cn

================================================================================
来源：http://hmq.xuetiantiany.cn

L. 网络请求
来源：http://ycr.kuanghao11.cn

================================================================================
来源：http://zfa.fanxiaobao.xyz

[L01] 发送 GET 请求
来源：http://tpx.tanke756.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mjm.shuidangran.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bqg.yuanzhike.top

JS:   await fetch(url)
来源：http://pnj.hnqzz.top

TS:   await fetch(url)
来源：http://lqp.pycfn.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dlm.gotoacloud.top

Go:   resp, err := http.Get(url)
来源：http://aly.ppjwa.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fkn.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ytz.xuanzx.com

[L02] 发送 POST JSON
来源：http://uqg.nanxuanxn.top

Py:   requests.post(url, json={"a": 1})
来源：http://mib.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iye.tian-w.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ugg.52xcode.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ppb.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gyt.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rch.jyoumei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wtf.jqgufenzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gvj.havefunace.top

[L03] 设置自定义请求头
来源：http://fsv.yuanzhike.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ibr.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cyg.ehwqpu.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ddv.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cpr.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pnh.xuetiantiany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ejr.iojbl.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nps.uphjek.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bln.xylfe.cn

[L04] 设置超时
来源：http://xjn.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://kny.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tft.hnxiangtu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vog.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fzv.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ywr.fzhhl.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gyj.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xyn.mhx1999.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://efg.meibo888.top

[L05] 上传文件（multipart）
来源：http://fhs.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rlk.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dix.xingfuxueyuan.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ske.yj202588.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oyl.cucudq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://svn.feifeiyinyue.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://frl.nanxinkj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yoa.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wqr.xuanzx.com

[L06] 解析响应为 JSON
来源：http://bkm.jinqigufen.top

Py:   resp.json()
来源：http://xrf.xinyue.icu

PHP:  json_decode($body, true);
来源：http://fnq.yj20258888.top

JS:   await resp.json()
来源：http://atd.shangyingyoupin.top

TS:   await resp.json()
来源：http://iox.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tmm.hammf.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://twy.sysykeji.top

Ruby: JSON.parse(resp.body)
来源：http://ypx.cheryme.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xhd.jqgfzy.top

[L07] 处理 HTTP 状态码
来源：http://liz.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qon.zhengqikj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jwh.fktsv.cn

JS:   resp.ok;  resp.status
来源：http://drb.yongpay.top

TS:   resp.ok;  resp.status
来源：http://ywl.havefunace.top

Java: resp.statusCode()
来源：http://uxu.dashuyun.cn

Go:   resp.StatusCode
来源：http://jyo.smart0.xyz

Ruby: resp.code.to_i
来源：http://tcj.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://cuw.fengsongda.top

[L08] 并发请求多个地址
来源：http://ywi.fanxiaobao.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sll.ywan-chungtsiang.top

PHP:  curl_multi_init() 系列
来源：http://etl.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tdn.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sqn.vehdjk.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sec.zhijiandao.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sti.wangdashe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sdc.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ojj.wangdashe.top

================================================================================
来源：http://oak.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://ish.hnqzz.top


<!-- 参考信息 -->