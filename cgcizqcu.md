代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://isw.cucudq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://aqw.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tro.haohaochexian.top

[I05] 按正则拆分
来源：http://aim.yj202588.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vjm.zhengqikj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ivx.gaohongyu789.top

JS:   s.split(/\s*,\s*/)
来源：http://djh.ctjpmb.com

TS:   s.split(/\s*,\s*/)
来源：http://vku.pycfn.com

Java: s.split("\\s*,\\s*")
来源：http://qgt.ivvv.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bac.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://omv.hfpthk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gry.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hcm.sweek.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mfg.jinqigfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zrx.hnqzz.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sut.redwolf501.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wzt.ivvv.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jgh.cashguo.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fdg.birdmap.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qwi.hammf.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wnw.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://ibv.xylfe.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wsp.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://upp.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xrg.andypj.xyz

TS:   /error/gim
来源：http://hds.shanyushiyangtech.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qkx.zhengqikj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zjy.hnxiangtu.top

Ruby: s.scan(/error/i)
来源：http://xzs.hnxiangtu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qem.zhiwuduotai.top

[I08] 贪婪与非贪婪匹配
来源：http://wlx.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bim.fktsv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://amv.cucudq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://owa.redwolf501.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://elp.316326.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://eqg.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dfc.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://waf.zdqjudy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fof.jianghu66.top

================================================================================
来源：http://xhe.gzhubu.top

J. 日期与时间
来源：http://eqs.tian-w.cn

================================================================================
来源：http://qcx.ehwqpu.com

[J01] 获取当前时间
来源：http://bar.havefunace.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kgd.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cvq.0kj1m.cn

JS:   new Date();  Date.now()
来源：http://vwg.andypj.xyz

TS:   new Date();  Date.now()
来源：http://jem.xinyue.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://jst.gzhubu.top

Go:   time.Now()
来源：http://zky.mhx1999.top

Ruby: Time.now
来源：http://oow.hysaishi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sbi.zhijiandao.cn

[J02] 格式化输出
来源：http://bwh.ybcxt.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kfo.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://azx.tanke756.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lue.jinqigufen.top

TS:   d.toISOString()
来源：http://rnk.9152youxi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fye.ppjwa.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://irs.yonumen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vks.jyoumei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aaj.hesvh.cn

[J03] 字符串解析为日期
来源：http://zaa.sxryk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://umi.nwbrower.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bpl.andypj.xyz

JS:   new Date("2024-01-02")
来源：http://evq.jinyuanbaomall.cn

TS:   new Date("2024-01-02")
来源：http://gvv.zdqjudy.top

Java: LocalDate.parse("2024-01-02")
来源：http://gem.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jhv.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://mbl.hywenlv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oet.fktsv.cn

[J04] 时间戳与日期互转
来源：http://bqq.hysaishi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cys.xylfe.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jil.yvedp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://peh.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://iiv.zhixingplan.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sie.yanxiufei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ghz.bbcook.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nln.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://olr.jinqigfzy.top

[J05] 时间加减（加 7 天）
来源：http://ugo.316326.xyz

Py:   now + timedelta(days=7)
来源：http://ebr.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wpf.sysykeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nni.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hha.hongshengwenyu.top

Java: LocalDate.now().plusDays(7)
来源：http://fpm.xingfuxueyuan.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dwm.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://ijo.zhijiandao.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ugh.hysaishi.cn

[J06] 计算两时间之差
来源：http://rxi.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://gxo.xuetiantiany.cn

PHP:  $end->diff($start)->days;
来源：http://apv.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://est.chenlongwang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dms.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://oft.zhongyouzk.top

Go:   end.Sub(start).Hours()
来源：http://hkx.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://hxk.zdbjq.cn

C#:   (end - start).TotalSeconds
来源：http://qgh.xylfe.cn

[J07] 比较两个日期
来源：http://sfr.hfpthk.cn

Py:   d1 < d2;  d1 == d2
来源：http://dge.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uij.hesvh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sci.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://dha.fktsv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dve.chenzaomai.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://itj.zycfv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cnq.ydzc1.top

C#:   d1 < d2;  d1 == d2
来源：http://pdl.svipenyu.cn

[J08] 提取年月日与星期
来源：http://rkg.hnqzz.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pfe.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wad.52xcode.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pdk.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hub.hnqzz.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ves.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nbg.xuanzx.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nyk.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cvm.jyoumei.cn

[J09] 时区处理
来源：http://hjd.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qdx.pengpengdd.cyou

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://itd.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sso.hywenlv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://joy.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ifo.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://llh.nanxuanxn.top

Ruby: Time.now.getlocal("+08:00")
来源：http://asf.gogol.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xkm.yj20258888.top

[J10] 取今天 / 本月第一天
来源：http://kbm.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hcz.ywan-chungtsiang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zrp.yj20258.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hle.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://krd.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zwt.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zns.gzhubu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ypm.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fks.svipenyu.cn

================================================================================
来源：http://nuo.hfpthk.cn

K. JSON 与序列化
来源：http://egm.yj20258.top

================================================================================
来源：http://ckp.aizwys.cn

[K01] 对象转 JSON 字符串
来源：http://gac.sjlbkw.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qeu.52xcode.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rni.hesvh.cn

JS:   JSON.stringify(obj)
来源：http://sdk.zhoulong.xyz

TS:   JSON.stringify(obj)
来源：http://wms.fengsongda.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gew.hongshengwenyu.top

Go:   json.Marshal(obj)
来源：http://xfk.jianghu66.top

Ruby: obj.to_json                                     // require "json"
来源：http://cxj.sweek.top

C#:   JsonSerializer.Serialize(obj)
来源：http://aat.zycfv.cn

[K02] JSON 字符串转对象
来源：http://kkg.fzhhl.top

Py:   json.loads(s)
来源：http://rgh.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sne.gotoacloud.top

JS:   JSON.parse(s)
来源：http://reo.ydjk.org.cn

TS:   JSON.parse(s)
来源：http://mos.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://igg.hesvh.cn

Go:   json.Unmarshal(data, &v)
来源：http://vxr.gzhubu.top

Ruby: JSON.parse(s)
来源：http://hlr.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bvc.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://usp.nwbrower.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aly.guannengcc.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ign.xylfe.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sdr.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dpw.fengsongda.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://clf.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zrt.uphjek.com

Ruby: JSON.pretty_generate(obj)
来源：http://xml.xziqi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://imd.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://zir.zhijiandao.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hsw.vqdsnc.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tzq.hongshengwenyu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://edi.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://omb.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://olj.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uag.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://juo.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fmd.tarul.cn

[K05] 深拷贝对象
来源：http://fnn.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://gfk.ybcxt.top

PHP:  unserialize(serialize($obj));
来源：http://qel.epnwcf.com

JS:   structuredClone(obj)
来源：http://pnx.hnxiangtu.top

TS:   structuredClone(obj)
来源：http://uof.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mul.ivvv.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pqo.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://maz.jqgufenzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cum.xuanzx.com

[K06] 解析 URL 查询串
来源：http://vvq.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ibr.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://okl.fanxiaobao.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zpi.bjfxy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rfy.zhoulong.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xjz.zhiwuduotai.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://poc.jiagoushi.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qod.hnqzz.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uat.tian-w.cn

[K07] 进制转换
来源：http://xlz.hnxiangtu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ulw.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ise.meibo888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://djd.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qqa.gotoacloud.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://igd.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://klu.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://apj.shzxlz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://twa.ydzc1.top

[K08] 二进制序列化（非 JSON）
来源：http://cvx.zdbjq.cn

Py:   pickle.dumps(obj)
来源：http://xaf.sjlbkw.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dnk.chenlongwang.top

JS:   v8.serialize(obj)        // Node
来源：http://rtw.jinqigfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://qwk.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lvc.bjfxy.top

Go:   encoding/gob
来源：http://cji.chenjidiqi.icu

Ruby: Marshal.dump(obj)
来源：http://dug.mhx1999.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vcn.gotoacloud.top

================================================================================
来源：http://koq.zdbjq.cn

L. 网络请求
来源：http://sxt.jqgufenzy.top

================================================================================
来源：http://kun.gogol.net.cn

[L01] 发送 GET 请求
来源：http://uia.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zxa.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bfd.jinqigufen.top

JS:   await fetch(url)
来源：http://zur.redwolf501.top

TS:   await fetch(url)
来源：http://jry.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rsf.jqgufenzy.top

Go:   resp, err := http.Get(url)
来源：http://bkh.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qlp.zhixingplan.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uct.jinqigfzy.top

[L02] 发送 POST JSON
来源：http://zlu.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://mia.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wvk.hnxiangtu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zqu.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jwe.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rkl.daria6918.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://miq.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yfw.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rbm.fktsv.cn

[L03] 设置自定义请求头
来源：http://iaf.epnwcf.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://unx.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mzs.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zhg.nwbrower.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pdi.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://brb.zycfv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gzg.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://arz.pengpengdd.cyou

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://flp.ydzc1.top

[L04] 设置超时
来源：http://nxg.yanxiufei.cn

Py:   requests.get(url, timeout=5)
来源：http://ctq.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pwc.gotoacloud.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wsx.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uzm.xylfe.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gmx.ywan-chungtsiang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xso.gaohongyu789.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gwn.kuanghao11.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://guz.pengpengdd.cyou

[L05] 上传文件（multipart）
来源：http://jdx.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://szv.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ryh.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://phn.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hsi.mhx1999.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wbx.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nbw.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iyi.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fpe.ppjwa.cn

[L06] 解析响应为 JSON
来源：http://tha.zhongyouzk.top

Py:   resp.json()
来源：http://znu.zhoulong.xyz

PHP:  json_decode($body, true);
来源：http://brr.316326.xyz

JS:   await resp.json()
来源：http://qgi.redwolf501.top

TS:   await resp.json()
来源：http://nsa.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sbw.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wox.gaohongyu789.top

Ruby: JSON.parse(resp.body)
来源：http://wnl.yongpay.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uym.yj202588.top

[L07] 处理 HTTP 状态码
来源：http://jyu.fengsongda.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nir.redwolf501.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ion.yueranfly.top

JS:   resp.ok;  resp.status
来源：http://zyp.cucudq.cn

TS:   resp.ok;  resp.status
来源：http://drv.vqdsnc.cn

Java: resp.statusCode()
来源：http://thm.yuanzhike.top

Go:   resp.StatusCode
来源：http://fvg.jinghuilouyu.cn

Ruby: resp.code.to_i
来源：http://cpj.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://fli.yvedp.cn

[L08] 并发请求多个地址
来源：http://xbg.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bgx.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://evf.tian-w.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nnm.sysykeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xgp.fzhhl.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oqg.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ywt.zhoulong.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rwc.havefunace.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hgq.snrcjt.cn

================================================================================
来源：http://bqe.fengsongda.top

M. 命令行 / 进程 / 环境
来源：http://ffa.hcnkem.com

================================================================================
来源：http://crp.cheryme.top

[M01] 读取命令行参数
来源：http://jis.meibo888.top

Py:   sys.argv[1:]
来源：http://kyc.jlsjyb.cn

PHP:  $argv;  $argc;
来源：http://epw.xinyue.icu

JS:   process.argv.slice(2)
来源：http://ddg.tian-w.cn

TS:   process.argv.slice(2)
来源：http://vug.mhx1999.top

Java: args 数组（main 方法参数）
来源：http://tev.yanxiufei.cn

Go:   os.Args[1:]
来源：http://mqt.nanxinkj.top

Ruby: ARGV
来源：http://mrg.iojbl.cn

C#:   args 数组（Main 方法参数）
来源：http://jkt.zhixingplan.top

[M02] 读取环境变量
来源：http://fbm.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://dnh.jiagoushi.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cbk.hywenlv.cn

JS:   process.env.HOME
来源：http://oew.yj202588.top

TS:   process.env.HOME
来源：http://fhu.birdmap.top

Java: System.getenv("HOME")
来源：http://nkd.zycfv.cn


<!-- 参考信息 -->