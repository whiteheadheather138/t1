代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://omy.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yzg.svipenyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://avd.jinqigufen.top

TS:   s.split(/\s*,\s*/)
来源：http://ydo.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://cbi.zhengqikj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lax.sweek.top

Ruby: s.split(/\s*,\s*/)
来源：http://pxf.jinyuanbaomall.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yjz.316326.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ctf.jinqigfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ypl.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vbt.sysykeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mtk.sufxvd.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mks.zhongyouzk.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dtm.daxiang520.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zxn.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zvx.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vlc.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://hhs.shanyushiyangtech.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://flj.jinghuilouyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zbo.epnwcf.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pml.zhiwuduotai.top

TS:   /error/gim
来源：http://vay.fanxiaobao.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hbq.chenlongwang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ppx.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://jup.vqdsnc.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://idy.hnxiangtu.top

[I08] 贪婪与非贪婪匹配
来源：http://osc.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pns.fktsv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qqk.epnwcf.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://taa.ydjk.org.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qea.chenlongwang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ooy.xingfuxueyuan.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://spi.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fer.cashguo.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yrl.0kj1m.cn

================================================================================
来源：http://how.cheryme.top

J. 日期与时间
来源：http://tvy.cdnleiting.top

================================================================================
来源：http://jxm.yanxiufei.cn

[J01] 获取当前时间
来源：http://nih.vqdsnc.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kju.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pdy.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://ffp.fengsongda.top

TS:   new Date();  Date.now()
来源：http://zmt.fanxiaobao.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://qpe.sweek.top

Go:   time.Now()
来源：http://ipa.feifeiyinyue.top

Ruby: Time.now
来源：http://kej.yonumen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hxl.shanyushiyangtech.top

[J02] 格式化输出
来源：http://rpo.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://crk.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bmv.xylfe.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aat.yangfankeji.com

TS:   d.toISOString()
来源：http://tgs.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xbq.aibaodan.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vzh.yonumen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://siu.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oqw.shanyushiyangkeji.top

[J03] 字符串解析为日期
来源：http://lrv.yueranfly.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pmb.aizwys.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ixr.shanyushiyangkeji.top

JS:   new Date("2024-01-02")
来源：http://evx.vqdsnc.cn

TS:   new Date("2024-01-02")
来源：http://frt.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://dqg.0kj1m.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ype.yuanzhike.top

Ruby: Date.parse("2024-01-02")
来源：http://cut.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yfh.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://nol.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rqv.zhaomingkeji.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qmv.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bev.tianlin.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://ldt.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gsb.epnwcf.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dzr.nanxinkj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kto.xingfuxueyuan.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qrw.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://lzh.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://whu.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ttf.zhixingplan.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ebv.sweek.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wbc.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://nzh.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://drz.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://bdc.316326.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://kkw.birdmap.top

[J06] 计算两时间之差
来源：http://oqb.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://fxh.dashuyun.cn

PHP:  $end->diff($start)->days;
来源：http://axh.cucudq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://urh.ppjwa.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nvu.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://sel.daria6918.cn

Go:   end.Sub(start).Hours()
来源：http://zum.hfpthk.cn

Ruby: end - start                 # 返回秒数
来源：http://hzk.daxiang520.top

C#:   (end - start).TotalSeconds
来源：http://dbd.xinyue.icu

[J07] 比较两个日期
来源：http://wma.zhijiandao.cn

Py:   d1 < d2;  d1 == d2
来源：http://okz.0kj1m.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ajh.quarkkingdee.top

JS:   d1.getTime() < d2.getTime()
来源：http://bfj.cucudq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://djx.jyoumei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vyq.jinghuilouyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ggj.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://utu.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://oue.svipenyu.cn

[J08] 提取年月日与星期
来源：http://kpw.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xmz.ivvv.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ejs.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ifd.hysaishi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xsa.fehbvm.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rzs.shangyingyoupin.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wmr.yuxming.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xre.nanxuanxn.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qws.cheryme.top

[J09] 时区处理
来源：http://fqr.yj20258.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iob.daxiang520.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iqj.hammf.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ayn.zhongyouzk.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gar.zhiwuduotai.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rko.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ays.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kkh.xylfe.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mbj.ywan-chungtsiang.top

[J10] 取今天 / 本月第一天
来源：http://jaf.dianchejie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://luw.xingfuxueyuan.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hch.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tpv.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cwy.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hwc.zycfv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qqo.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dia.chenlongwang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://drw.tianlin.xyz

================================================================================
来源：http://drq.ydjk.org.cn

K. JSON 与序列化
来源：http://ari.shanyushiyangkeji.top

================================================================================
来源：http://fsz.meibo888.top

[K01] 对象转 JSON 字符串
来源：http://idf.jinyuanbaomall.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wyf.iojbl.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://njk.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://kta.jinqigufen.top

TS:   JSON.stringify(obj)
来源：http://ryu.ydjk.org.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zdr.wangshuangyany.cn

Go:   json.Marshal(obj)
来源：http://mfg.nanxinkj.top

Ruby: obj.to_json                                     // require "json"
来源：http://evh.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://msu.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://yhq.yangfankeji.com

Py:   json.loads(s)
来源：http://tkk.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hpr.meibo888.top

JS:   JSON.parse(s)
来源：http://mjg.zhixingplan.top

TS:   JSON.parse(s)
来源：http://olp.jqgfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://woz.wangshuangyany.cn

Go:   json.Unmarshal(data, &v)
来源：http://gfz.mhx1999.top

Ruby: JSON.parse(s)
来源：http://olv.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uuk.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://bcf.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zsw.zhiwuduotai.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tct.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lxp.hcnkem.com

TS:   JSON.stringify(obj, null, 2)
来源：http://efb.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jfl.jinghuilouyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lrx.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://ngy.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qmk.zdbjq.cn

[K04] 读取 JSON 文件
来源：http://ytc.yueranfly.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vat.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://twg.shanyushiyangtech.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zmq.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hen.tian-w.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cjm.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://phr.wangshuangyany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xrc.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cbj.hesvh.cn

[K05] 深拷贝对象
来源：http://bcn.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://egr.dianchejie.cn

PHP:  unserialize(serialize($obj));
来源：http://ewk.hcnkem.com

JS:   structuredClone(obj)
来源：http://kre.ehwqpu.com

TS:   structuredClone(obj)
来源：http://vth.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nub.jinyuanbaomall.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jyl.wangdashe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bed.yueranfly.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rxu.sxryk.cn

[K06] 解析 URL 查询串
来源：http://cjv.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dey.gzhubu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qyw.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cck.jinyuanbaomall.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tkn.jqgufenzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://emy.hcnkem.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://jrr.jiagoushi.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xwa.dashuyun.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nps.redwolf501.top

[K07] 进制转换
来源：http://leu.daria6918.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yvt.sxryk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wzp.hcnkem.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dfi.cheryme.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dzk.jianghu66.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fok.yonumen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://llg.aizwys.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lnl.nanxuanxn.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xgq.guowangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://xzx.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://bbc.sjlbkw.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dkq.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://zkb.bjfxy.top

TS:   v8.serialize(obj)        // Node
来源：http://kuy.jqgufenzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oao.yuanzhike.top

Go:   encoding/gob
来源：http://wmu.52xcode.cn

Ruby: Marshal.dump(obj)
来源：http://qmw.kuanghao11.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yzn.zycfv.cn

================================================================================
来源：http://bgr.aizwys.cn

L. 网络请求
来源：http://csc.wangshuangyany.cn

================================================================================
来源：http://txk.dashuyun.cn

[L01] 发送 GET 请求
来源：http://fxe.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rdf.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://scp.shangyingyoupin.top

JS:   await fetch(url)
来源：http://wmz.pycfn.com

TS:   await fetch(url)
来源：http://nzi.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pwu.chenlongwang.top

Go:   resp, err := http.Get(url)
来源：http://ikb.dashuyun.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dhp.fzhhl.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vei.9152youxi.cn

[L02] 发送 POST JSON
来源：http://uru.cheryme.top

Py:   requests.post(url, json={"a": 1})
来源：http://ome.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lnq.shzxlz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dyf.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://exw.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lhf.xziqi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zbr.dianchejie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eam.jlsjyb.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lem.ehwqpu.com

[L03] 设置自定义请求头
来源：http://wuz.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rhg.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://txe.jinqigfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wbe.316326.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mxx.pycfn.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vlg.jinqigfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nwu.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jtr.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qhv.hongshengwenyu.top

[L04] 设置超时
来源：http://iuc.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://xcc.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wpz.snrcjt.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iuk.zhaomingkeji.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://esd.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://noz.jianghu66.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eno.yvedp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hxr.fehbvm.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ool.smart0.xyz

[L05] 上传文件（multipart）
来源：http://mcl.ybcxt.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dny.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kmt.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eqc.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://btj.mhx1999.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://epm.epnwcf.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qrw.cucudq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ngm.uphjek.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mzd.cucudq.cn

[L06] 解析响应为 JSON
来源：http://npn.zdbjq.cn

Py:   resp.json()
来源：http://nly.zhongyouzk.top

PHP:  json_decode($body, true);
来源：http://qho.0kj1m.cn

JS:   await resp.json()
来源：http://seq.daxiang520.top

TS:   await resp.json()
来源：http://zvo.ydzc1.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zfu.hesvh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xoy.hcnkem.com

Ruby: JSON.parse(resp.body)
来源：http://pdr.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lwp.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://tpw.yanxiufei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kgf.pengpengdd.cyou

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sxu.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://uuu.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://enw.zhengqikj.top

Java: resp.statusCode()
来源：http://fxm.sysykeji.top

Go:   resp.StatusCode
来源：http://xiu.xingfuxueyuan.xyz

Ruby: resp.code.to_i
来源：http://ckm.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://hho.cashguo.top

[L08] 并发请求多个地址
来源：http://kvp.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ccv.sufxvd.cn

PHP:  curl_multi_init() 系列
来源：http://bxp.52xcode.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ujv.jqgufenzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wns.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tlk.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wnh.guowangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hjo.ppjwa.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ssb.feifeiyinyue.top

================================================================================
来源：http://gjd.jqgufenzy.top

M. 命令行 / 进程 / 环境
来源：http://olt.yuanzhike.top

================================================================================
来源：http://uyy.ydzc1.top

[M01] 读取命令行参数
来源：http://tky.0kj1m.cn

Py:   sys.argv[1:]
来源：http://dtn.nanxinkj.top

PHP:  $argv;  $argc;
来源：http://vuc.yueranfly.top

JS:   process.argv.slice(2)
来源：http://egt.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://hfm.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://jln.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://aot.dianchejie.cn

Ruby: ARGV
来源：http://mar.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://nye.haohaochexian.top

[M02] 读取环境变量
来源：http://skk.zdbjq.cn

Py:   os.environ.get("HOME")
来源：http://non.chenzaomai.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://csu.tianlin.xyz

JS:   process.env.HOME
来源：http://isr.jinqigfzy.top

TS:   process.env.HOME
来源：http://msp.hammf.cn

Java: System.getenv("HOME")
来源：http://fib.dashuyun.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lzz.xinyue.icu

Ruby: ENV["HOME"]
来源：http://dov.hammf.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mhv.gzhubu.top

[M03] 执行外部命令
来源：http://sxi.fengsongda.top


<!-- 参考信息 -->