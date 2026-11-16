代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ors.jinqigfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://jqz.xylfe.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kme.nanxuanxn.top

Java: s.replaceAll("\\d+", "#")
来源：http://kzg.wangdashe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pmi.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tnc.xuetiantiany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tgr.redwolf501.top

[I05] 按正则拆分
来源：http://fvq.daxiang520.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fst.andypj.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rwh.hfpthk.cn

JS:   s.split(/\s*,\s*/)
来源：http://aus.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://qvh.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://ego.xylfe.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pot.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://owz.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tlo.sjlbkw.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://inv.yonumen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wbd.tianlin.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yvb.c1oappe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ftw.hysaishi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ixb.nanxinkj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mon.feifeiyinyue.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dus.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gba.xuanzx.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vge.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://hgx.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iyk.jqgfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ujm.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lqu.shanyushiyangkeji.top

TS:   /error/gim
来源：http://ydq.jinqigufen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kgw.aibaodan.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xxm.sxryk.cn

Ruby: s.scan(/error/i)
来源：http://kcu.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lnv.jqgfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://bon.316326.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nud.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sbu.yfazqb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uff.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://raw.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rfl.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yww.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://frr.ydjk.org.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tmx.tanke756.top

================================================================================
来源：http://kkp.vehdjk.com

J. 日期与时间
来源：http://lgw.cucudq.cn

================================================================================
来源：http://kfd.fengsongda.top

[J01] 获取当前时间
来源：http://rye.yuanzhike.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://csh.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yxn.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://uyb.uphjek.com

TS:   new Date();  Date.now()
来源：http://egw.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vqa.shanyushiyangkeji.top

Go:   time.Now()
来源：http://egd.haohaochexian.top

Ruby: Time.now
来源：http://yvn.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ceg.tanke756.top

[J02] 格式化输出
来源：http://dzt.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gzd.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kbi.xylfe.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eoq.zhoulong.xyz

TS:   d.toISOString()
来源：http://hie.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oei.yanxiufei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://suk.gzhubu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vfr.bbcook.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bwz.sysykeji.top

[J03] 字符串解析为日期
来源：http://rbb.hywenlv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bxl.ydzc1.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ach.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://dum.yfazqb.com

TS:   new Date("2024-01-02")
来源：http://ivm.yj202588.top

Java: LocalDate.parse("2024-01-02")
来源：http://qgy.zdqjudy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xjd.hywenlv.cn

Ruby: Date.parse("2024-01-02")
来源：http://voc.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lsa.smart0.xyz

[J04] 时间戳与日期互转
来源：http://ikn.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wmh.jinqigfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zxd.dashuyun.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://byh.nanxinkj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nfx.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rgl.jyoumei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://znr.jyoumei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ids.9152youxi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jkn.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://sku.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://jsu.smart0.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://mln.shanyushiyangtech.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qoe.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dwa.epnwcf.com

Java: LocalDate.now().plusDays(7)
来源：http://zcw.shangyingyoupin.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qsh.chenzaomai.com

Ruby: Time.now + 7 * 86400
来源：http://gsp.iojbl.cn

C#:   DateTime.Now.AddDays(7)
来源：http://txx.yuxming.cn

[J06] 计算两时间之差
来源：http://vwk.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://krc.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://egc.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ozr.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kzh.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://luk.yj202588.top

Go:   end.Sub(start).Hours()
来源：http://zqr.jyoumei.cn

Ruby: end - start                 # 返回秒数
来源：http://yux.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://vuw.yonumen.top

[J07] 比较两个日期
来源：http://jxc.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://aji.quarkkingdee.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ofu.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://end.daxiang520.top

TS:   d1.getTime() < d2.getTime()
来源：http://gku.jinyuanbaomall.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nkx.xylfe.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gso.jinqigufen.top

Ruby: d1 < d2;  d1 == d2
来源：http://mub.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://kvw.chenlongwang.top

[J08] 提取年月日与星期
来源：http://efr.xuanzx.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ben.dashuyun.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nwd.epnwcf.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vhb.vehdjk.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kku.snrcjt.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://log.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mqh.sjlbkw.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fcm.cheryme.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hhq.jinyuanbaomall.cn

[J09] 时区处理
来源：http://ntw.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ttm.sjlbkw.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://awg.0kj1m.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://klc.cashguo.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qvy.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xfe.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://odn.zhaomingkeji.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://uzr.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ssa.bbcook.cn

[J10] 取今天 / 本月第一天
来源：http://miz.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ddp.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zoh.gogol.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oya.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qew.zhijiandao.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xgq.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bgt.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jsj.vehdjk.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://suw.andypj.xyz

================================================================================
来源：http://vgg.jianghu66.top

K. JSON 与序列化
来源：http://pnf.guannengcc.top

================================================================================
来源：http://kyb.guannengcc.top

[K01] 对象转 JSON 字符串
来源：http://tpo.52xcode.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uya.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uyg.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://bxo.316326.xyz

TS:   JSON.stringify(obj)
来源：http://qxt.vqdsnc.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sqk.snrcjt.cn

Go:   json.Marshal(obj)
来源：http://ysy.yueranfly.top

Ruby: obj.to_json                                     // require "json"
来源：http://rjz.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fkv.havefunace.top

[K02] JSON 字符串转对象
来源：http://bbd.cdnleiting.top

Py:   json.loads(s)
来源：http://xvs.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vng.jqgfzy.top

JS:   JSON.parse(s)
来源：http://itg.yonumen.top

TS:   JSON.parse(s)
来源：http://acy.meibo888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oai.yangfankeji.com

Go:   json.Unmarshal(data, &v)
来源：http://syr.ydjk.org.cn

Ruby: JSON.parse(s)
来源：http://lhg.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pzk.wangdashe.top

[K03] JSON 美化输出（带缩进）
来源：http://cem.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vav.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zgg.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yls.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wfr.sufxvd.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oza.shangyingyoupin.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://osp.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://iqp.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dti.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://kli.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zdq.316326.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iso.chenlongwang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hdn.tianlin.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hti.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gup.andypj.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://acx.ppjwa.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dqu.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://awn.hammf.cn

[K05] 深拷贝对象
来源：http://hjx.ctjpmb.com

Py:   copy.deepcopy(obj)
来源：http://jod.haohaochexian.top

PHP:  unserialize(serialize($obj));
来源：http://azd.gzhubu.top

JS:   structuredClone(obj)
来源：http://snt.chenjidiqi.icu

TS:   structuredClone(obj)
来源：http://aaq.jinqigfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dmb.ctjpmb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pwn.fengsongda.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mbc.ivvv.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hcg.yj202588.top

[K06] 解析 URL 查询串
来源：http://tos.cucudq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mzg.tanke756.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kyi.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hor.yonumen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hxq.sysykeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pxc.zdbjq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hhn.iojbl.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uoj.yuanzhike.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://puf.0kj1m.cn

[K07] 进制转换
来源：http://ijt.tanke756.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yqc.wangshuangyany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xjz.fzhhl.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lmr.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vwt.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://egr.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://liw.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lbx.jlsjyb.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gtz.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://kki.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://ntk.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rrc.cdnleiting.top

JS:   v8.serialize(obj)        // Node
来源：http://vwj.jinyuanbaomall.cn

TS:   v8.serialize(obj)        // Node
来源：http://vdu.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qdh.yvedp.cn

Go:   encoding/gob
来源：http://uro.chenzaomai.com

Ruby: Marshal.dump(obj)
来源：http://nmb.feifeiyinyue.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oag.cqqwz.cn

================================================================================
来源：http://dmb.tian-w.cn

L. 网络请求
来源：http://tuy.fzhhl.top

================================================================================
来源：http://eyh.yongpay.top

[L01] 发送 GET 请求
来源：http://wno.cucudq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://phm.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eik.yj202588.top

JS:   await fetch(url)
来源：http://xkm.ybcxt.top

TS:   await fetch(url)
来源：http://jcu.wangshuangyany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uxp.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://ndk.shangyingyoupin.top

Ruby: Net::HTTP.get(URI(url))
来源：http://izd.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yvk.birdmap.top

[L02] 发送 POST JSON
来源：http://uyo.gaohongyu789.top

Py:   requests.post(url, json={"a": 1})
来源：http://iwx.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wvj.jyoumei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xkf.zhaomingkeji.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wqg.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zgg.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dad.shzxlz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lmp.shanyushiyangtech.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hyh.xylfe.cn

[L03] 设置自定义请求头
来源：http://aiu.tanke756.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://npt.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ygt.pengpengdd.cyou

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ebu.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zbc.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uvo.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://epz.ehwqpu.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xia.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://htf.yuxming.cn

[L04] 设置超时
来源：http://cfz.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://cin.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://awc.fengsongda.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kyq.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yxt.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kzq.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kfv.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pfy.redwolf501.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wut.hesvh.cn

[L05] 上传文件（multipart）
来源：http://mxx.meibo888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iny.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://djz.jinqigfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://glf.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vcg.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lcy.chenjidiqi.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zns.ybcxt.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lvs.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fqh.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://ckp.fktsv.cn

Py:   resp.json()
来源：http://kqh.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://wid.daria6918.cn

JS:   await resp.json()
来源：http://ghj.xylfe.cn

TS:   await resp.json()
来源：http://giz.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aoc.chenjidiqi.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vhl.guannengcc.top

Ruby: JSON.parse(resp.body)
来源：http://sgk.sweek.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vom.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://mhw.fehbvm.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dne.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lvv.andypj.xyz

JS:   resp.ok;  resp.status
来源：http://rmi.hnqzz.top

TS:   resp.ok;  resp.status
来源：http://cup.nanxinkj.top

Java: resp.statusCode()
来源：http://dmc.9152youxi.cn

Go:   resp.StatusCode
来源：http://enw.yj202588.top

Ruby: resp.code.to_i
来源：http://kde.smart0.xyz

C#:   (int)resp.StatusCode
来源：http://gjn.redwolf501.top

[L08] 并发请求多个地址
来源：http://hca.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zwz.zhijiandao.cn

PHP:  curl_multi_init() 系列
来源：http://phd.hammf.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iqv.ivvv.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pgx.pycfn.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mti.shzxlz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nes.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hfk.xylfe.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pyz.guannengcc.top

================================================================================
来源：http://emu.wangshuangyany.cn

M. 命令行 / 进程 / 环境
来源：http://cvh.yuanzhike.top

================================================================================
来源：http://gtd.yueranfly.top

[M01] 读取命令行参数
来源：http://rfs.yongpay.top

Py:   sys.argv[1:]
来源：http://sra.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://zxk.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://huj.xziqi.cn

TS:   process.argv.slice(2)
来源：http://pab.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://wiu.vqdsnc.cn

Go:   os.Args[1:]
来源：http://pjh.yanxiufei.cn

Ruby: ARGV
来源：http://kxz.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://jyo.hesvh.cn

[M02] 读取环境变量
来源：http://fii.yj20258888.top

Py:   os.environ.get("HOME")
来源：http://xdd.zhixingplan.top


<!-- 参考信息 -->