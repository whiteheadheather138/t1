代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xza.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sqr.pycfn.com

TS:   s.replace(/\d+/g, "#")
来源：http://vxz.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uze.gogol.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dzs.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gts.yongpay.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ccb.yuanzhike.top

[I05] 按正则拆分
来源：http://yau.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fvc.cqqwz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tjm.ctjpmb.com

JS:   s.split(/\s*,\s*/)
来源：http://fis.jiagoushi.top

TS:   s.split(/\s*,\s*/)
来源：http://dyb.svipenyu.cn

Java: s.split("\\s*,\\s*")
来源：http://hhb.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sbs.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://brv.vqdsnc.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zqo.pycfn.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://two.guowangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dbh.dianchejie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://skx.9152youxi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gwk.tanke756.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cvc.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gkf.ydzc1.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wnr.ydzc1.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fuy.yueranfly.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rrn.shzxlz.cn

[I07] 忽略大小写与多行模式
来源：http://ppt.birdmap.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wjn.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cpj.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fju.gaohongyu789.top

TS:   /error/gim
来源：http://exy.zhengqikj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zlz.shanyushiyangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rdu.quarkkingdee.top

Ruby: s.scan(/error/i)
来源：http://rls.nwbrower.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ivy.dianchejie.cn

[I08] 贪婪与非贪婪匹配
来源：http://wgd.fktsv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rmp.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ugq.yuxming.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dpm.sxryk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pfa.ybcxt.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://anc.yongpay.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xzw.hammf.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wyq.zdqjudy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ozb.quarkkingdee.top

================================================================================
来源：http://aoj.cqqwz.cn

J. 日期与时间
来源：http://ssz.uphjek.com

================================================================================
来源：http://fkf.yanxiufei.cn

[J01] 获取当前时间
来源：http://guo.pycfn.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://vbx.hammf.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jjj.yfazqb.com

JS:   new Date();  Date.now()
来源：http://bku.sufxvd.cn

TS:   new Date();  Date.now()
来源：http://zlj.feifeiyinyue.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qmc.sweek.top

Go:   time.Now()
来源：http://eob.sjlbkw.cn

Ruby: Time.now
来源：http://tsl.hnxiangtu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rni.guannengcc.top

[J02] 格式化输出
来源：http://yue.9152youxi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xvv.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kxv.daxiang520.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mnu.andypj.xyz

TS:   d.toISOString()
来源：http://xkh.quarkkingdee.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wlq.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zds.yangfankeji.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mzy.epnwcf.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ikv.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://tai.sxryk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vhj.jinqigfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uwu.haohaochexian.top

JS:   new Date("2024-01-02")
来源：http://dxq.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://gmy.pengpengdd.cyou

Java: LocalDate.parse("2024-01-02")
来源：http://slr.daria6918.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ciu.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://aau.hfpthk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wja.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://iop.xylfe.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://khw.yj20258888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qya.haohaochexian.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bbm.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://khg.shanyushiyangtech.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://exp.ctjpmb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dpj.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wxv.chenlongwang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tvr.zdqjudy.top

[J05] 时间加减（加 7 天）
来源：http://sps.aibaodan.cn

Py:   now + timedelta(days=7)
来源：http://emc.daxiang520.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mil.wangdashe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uly.sufxvd.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://brs.smart0.xyz

Java: LocalDate.now().plusDays(7)
来源：http://sww.guowangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sdz.jianghu66.top

Ruby: Time.now + 7 * 86400
来源：http://rrq.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://axy.yj20258888.top

[J06] 计算两时间之差
来源：http://bzz.vehdjk.com

Py:   (end - start).total_seconds()
来源：http://ztj.jqgfzy.top

PHP:  $end->diff($start)->days;
来源：http://dow.quarkkingdee.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aif.sjlbkw.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baz.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://mec.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://ujw.xuanzx.com

Ruby: end - start                 # 返回秒数
来源：http://ckv.9152youxi.cn

C#:   (end - start).TotalSeconds
来源：http://war.ctjpmb.com

[J07] 比较两个日期
来源：http://pmk.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://zlk.yonumen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bvy.316326.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://rli.yuxming.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pha.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jgh.yfazqb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://euy.yfazqb.com

Ruby: d1 < d2;  d1 == d2
来源：http://zqy.yuanzhike.top

C#:   d1 < d2;  d1 == d2
来源：http://vlf.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://qae.vqdsnc.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uka.zhengqikj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yde.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tvk.yj20258.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://boe.jinqigufen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pdh.ctjpmb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xdb.cqqwz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pax.zdqjudy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://smo.zdqjudy.top

[J09] 时区处理
来源：http://sgr.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vma.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gdw.zhongyouzk.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://svv.quarkkingdee.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xzp.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ovn.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dat.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zju.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kts.sysykeji.top

[J10] 取今天 / 本月第一天
来源：http://rtt.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://loi.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ohq.hesvh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tln.tian-w.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dzk.zhoulong.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sml.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://grt.zdbjq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aro.hnqzz.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gym.xinyue.icu

================================================================================
来源：http://onv.zhixingplan.top

K. JSON 与序列化
来源：http://kkk.iojbl.cn

================================================================================
来源：http://nvp.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://rgu.yuxming.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gjz.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pjx.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://uon.birdmap.top

TS:   JSON.stringify(obj)
来源：http://lsp.hnxiangtu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dwa.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://xod.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uki.meibo888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qqc.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://lhb.daxiang520.top

Py:   json.loads(s)
来源：http://mcd.shanyushiyangtech.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nzo.zhongyouzk.top

JS:   JSON.parse(s)
来源：http://qej.jiagoushi.top

TS:   JSON.parse(s)
来源：http://ovc.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lnc.ehwqpu.com

Go:   json.Unmarshal(data, &v)
来源：http://nrv.316326.xyz

Ruby: JSON.parse(s)
来源：http://vke.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eve.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://vzx.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cnt.xylfe.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ibx.mhx1999.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yfn.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://usu.sxryk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hiq.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://glx.mhx1999.top

Ruby: JSON.pretty_generate(obj)
来源：http://tvi.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hfx.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://rto.xingfuxueyuan.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fub.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cfn.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qbf.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pob.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yxs.ybcxt.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nxw.nanxinkj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lns.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vrv.chenjidiqi.icu

[K05] 深拷贝对象
来源：http://xor.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://ekh.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://zhg.yuxming.cn

JS:   structuredClone(obj)
来源：http://ugn.dashuyun.cn

TS:   structuredClone(obj)
来源：http://wqa.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hsj.zhoulong.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hdo.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ggg.fktsv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oew.wangdashe.top

[K06] 解析 URL 查询串
来源：http://vhz.xylfe.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ftn.hesvh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zbb.xuanzx.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eui.daria6918.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pie.jyoumei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iaa.xuanzx.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://grn.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rwd.snrcjt.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hhf.9152youxi.cn

[K07] 进制转换
来源：http://dsr.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zio.andypj.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mcr.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ymv.jinqigufen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zjz.jqgufenzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cwy.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ecd.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zoi.epnwcf.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xii.feifeiyinyue.top

[K08] 二进制序列化（非 JSON）
来源：http://aiu.meibo888.top

Py:   pickle.dumps(obj)
来源：http://dte.yj202588.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sjs.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://tcq.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://ynt.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://szo.epnwcf.com

Go:   encoding/gob
来源：http://kvi.ivvv.top

Ruby: Marshal.dump(obj)
来源：http://cwd.vehdjk.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sbu.tarul.cn

================================================================================
来源：http://scc.gaohongyu789.top

L. 网络请求
来源：http://wpn.fzhhl.top

================================================================================
来源：http://unn.jqgfzy.top

[L01] 发送 GET 请求
来源：http://gyz.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sjy.shangyingyoupin.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ilj.ctjpmb.com

JS:   await fetch(url)
来源：http://fnm.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://awz.zhijiandao.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hja.fengsongda.top

Go:   resp, err := http.Get(url)
来源：http://gef.tianlin.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://kyl.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://owh.meibo888.top

[L02] 发送 POST JSON
来源：http://ffj.shanyushiyangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://dms.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yml.sysykeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gwy.haohaochexian.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qkw.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wlg.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://laf.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oey.tarul.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dyy.xuetiantiany.cn

[L03] 设置自定义请求头
来源：http://elp.jyoumei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rba.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://obk.epnwcf.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rww.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pcn.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://snq.snrcjt.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lpz.9152youxi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://onk.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://trj.svipenyu.cn

[L04] 设置超时
来源：http://nzr.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://vjm.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://niz.gzhubu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hmn.0kj1m.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jkr.tianlin.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fcr.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xem.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://upa.nwbrower.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pgz.daxiang520.top

[L05] 上传文件（multipart）
来源：http://wbs.xuanzx.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://brx.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cfs.daxiang520.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pqx.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://apd.cdnleiting.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oqn.feifeiyinyue.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aqe.zhijiandao.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oxb.hywenlv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uvv.yonumen.top

[L06] 解析响应为 JSON
来源：http://ekq.smart0.xyz

Py:   resp.json()
来源：http://owb.fzhhl.top

PHP:  json_decode($body, true);
来源：http://zdj.cashguo.top

JS:   await resp.json()
来源：http://bym.zhiwuduotai.top

TS:   await resp.json()
来源：http://pup.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hpb.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vcj.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://cvg.aizwys.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yuc.cheryme.top

[L07] 处理 HTTP 状态码
来源：http://zan.jianghu66.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mya.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pwe.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://qmm.jianghu66.top

TS:   resp.ok;  resp.status
来源：http://nmy.tanke756.top

Java: resp.statusCode()
来源：http://xsp.hnqzz.top

Go:   resp.StatusCode
来源：http://pzf.guannengcc.top

Ruby: resp.code.to_i
来源：http://bxe.ehwqpu.com

C#:   (int)resp.StatusCode
来源：http://ait.ppjwa.cn

[L08] 并发请求多个地址
来源：http://zss.hesvh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zii.zhiwuduotai.top

PHP:  curl_multi_init() 系列
来源：http://byg.havefunace.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://otl.xziqi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vmm.zhixingplan.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pjz.iojbl.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cns.fktsv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ycr.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cgy.andypj.xyz

================================================================================
来源：http://hux.mhx1999.top

M. 命令行 / 进程 / 环境
来源：http://uxg.daria6918.cn

================================================================================
来源：http://zgp.zhoulong.xyz

[M01] 读取命令行参数
来源：http://yww.zycfv.cn

Py:   sys.argv[1:]
来源：http://hvg.wangdashe.top

PHP:  $argv;  $argc;
来源：http://hfs.jiagoushi.top

JS:   process.argv.slice(2)
来源：http://gdm.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://dwi.cheryme.top

Java: args 数组（main 方法参数）
来源：http://coi.zhijiandao.cn

Go:   os.Args[1:]
来源：http://bft.feifeiyinyue.top

Ruby: ARGV
来源：http://cxz.iojbl.cn

C#:   args 数组（Main 方法参数）
来源：http://nyw.cdnleiting.top

[M02] 读取环境变量
来源：http://aor.wangdashe.top

Py:   os.environ.get("HOME")
来源：http://oby.shanyushiyangtech.top


<!-- 参考信息 -->