代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ram.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yhu.hcnkem.com

TS:   s.replace(/\d+/g, "#")
来源：http://vsp.xinyue.icu

Java: s.replaceAll("\\d+", "#")
来源：http://kju.hywenlv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rbc.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://haq.yvedp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://miy.xuanzx.com

[I05] 按正则拆分
来源：http://hlz.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tfq.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://thn.ybcxt.top

JS:   s.split(/\s*,\s*/)
来源：http://ten.fehbvm.com

TS:   s.split(/\s*,\s*/)
来源：http://atq.chenlongwang.top

Java: s.split("\\s*,\\s*")
来源：http://luc.sufxvd.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://own.cucudq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yde.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tyu.fktsv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://api.jlsjyb.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gky.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hzo.fehbvm.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uvp.shuidangran.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gtd.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jxz.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xog.tanke756.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ppq.bjfxy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uhz.svipenyu.cn

[I07] 忽略大小写与多行模式
来源：http://bsh.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://con.zhoulong.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gbb.sufxvd.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nvd.cheryme.top

TS:   /error/gim
来源：http://eij.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wul.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oua.smart0.xyz

Ruby: s.scan(/error/i)
来源：http://xfk.aibaodan.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vnr.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://ygq.aibaodan.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hjc.yfazqb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://smr.ywan-chungtsiang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sut.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://biv.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://bna.aibaodan.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://krg.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nbp.xuanzx.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://unf.uphjek.com

================================================================================
来源：http://tyv.gaohongyu789.top

J. 日期与时间
来源：http://dwi.daria6918.cn

================================================================================
来源：http://kdr.dianchejie.cn

[J01] 获取当前时间
来源：http://fwj.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ezr.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gow.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://vjl.zhixingplan.top

TS:   new Date();  Date.now()
来源：http://kma.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dgm.fengsongda.top

Go:   time.Now()
来源：http://crt.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://zqc.haohaochexian.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jxf.jqgfzy.top

[J02] 格式化输出
来源：http://xps.hnxiangtu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bzs.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kgg.zycfv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wbj.chenjidiqi.icu

TS:   d.toISOString()
来源：http://qif.yanxiufei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dvc.wangshuangyany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zqe.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rlt.xuanzx.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yqt.cqqwz.cn

[J03] 字符串解析为日期
来源：http://rtz.yanxiufei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://evf.c1oappe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zoa.xingfuxueyuan.xyz

JS:   new Date("2024-01-02")
来源：http://jmd.9152youxi.cn

TS:   new Date("2024-01-02")
来源：http://mav.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://nxz.redwolf501.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rmb.shuidangran.top

Ruby: Date.parse("2024-01-02")
来源：http://slr.shzxlz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lyc.yangfankeji.com

[J04] 时间戳与日期互转
来源：http://ggc.dianchejie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ndh.fktsv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uew.redwolf501.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lwn.andypj.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://rzx.316326.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://exn.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mbk.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zag.hammf.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yur.haohaochexian.top

[J05] 时间加减（加 7 天）
来源：http://bvc.0kj1m.cn

Py:   now + timedelta(days=7)
来源：http://xdz.shzxlz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qlg.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lud.uphjek.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uvo.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://huj.nanxinkj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ktm.xuanzx.com

Ruby: Time.now + 7 * 86400
来源：http://ixa.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fzn.ctjpmb.com

[J06] 计算两时间之差
来源：http://vzk.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://mcr.zhixingplan.top

PHP:  $end->diff($start)->days;
来源：http://bgh.zhaomingkeji.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ffe.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mek.tian-w.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jdp.cucudq.cn

Go:   end.Sub(start).Hours()
来源：http://fxh.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://omv.wangshuangyany.cn

C#:   (end - start).TotalSeconds
来源：http://psr.nanxuanxn.top

[J07] 比较两个日期
来源：http://qvd.chenzaomai.com

Py:   d1 < d2;  d1 == d2
来源：http://veu.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wyh.yj20258888.top

JS:   d1.getTime() < d2.getTime()
来源：http://pwl.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jsb.jinghuilouyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fpr.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pjv.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://ewh.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ixo.hcnkem.com

[J08] 提取年月日与星期
来源：http://pde.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ryx.snrcjt.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nyq.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://psj.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lym.yj20258.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://plk.shanyushiyangtech.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bem.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tmh.ybcxt.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jxx.yj202588.top

[J09] 时区处理
来源：http://kym.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mtu.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yyz.jinqigfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jci.redwolf501.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ohr.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wjl.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mrl.daria6918.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://now.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://agb.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://ekr.xuanzx.com

Py:   date.today();  date.today().replace(day=1)
来源：http://tqo.meibo888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vbd.jinqigfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ujz.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pke.jlsjyb.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ygn.yonumen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wlw.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ixe.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wgg.guowangkeji.top

================================================================================
来源：http://syz.yanxiufei.cn

K. JSON 与序列化
来源：http://iyb.chenlongwang.top

================================================================================
来源：http://uqt.havefunace.top

[K01] 对象转 JSON 字符串
来源：http://vbl.guowangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wuj.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oec.andypj.xyz

JS:   JSON.stringify(obj)
来源：http://njh.hnxiangtu.top

TS:   JSON.stringify(obj)
来源：http://aeg.birdmap.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hgj.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://get.xylfe.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qwj.cheryme.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lrp.fehbvm.com

[K02] JSON 字符串转对象
来源：http://kbl.redwolf501.top

Py:   json.loads(s)
来源：http://csq.fzhhl.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wjo.yangfankeji.com

JS:   JSON.parse(s)
来源：http://gjn.sysykeji.top

TS:   JSON.parse(s)
来源：http://zrq.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tbg.gaohongyu789.top

Go:   json.Unmarshal(data, &v)
来源：http://plc.gzhubu.top

Ruby: JSON.parse(s)
来源：http://hfz.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://deb.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://qaz.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vzn.52xcode.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bkh.xingfuxueyuan.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://ouh.jinyuanbaomall.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qeo.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pur.316326.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bbz.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sfg.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ids.guannengcc.top

[K04] 读取 JSON 文件
来源：http://bul.yvedp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kxr.havefunace.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oyc.zdqjudy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fik.cashguo.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pud.zhiwuduotai.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lxk.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vpl.yonumen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mdc.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://voy.ehwqpu.com

[K05] 深拷贝对象
来源：http://yve.hysaishi.cn

Py:   copy.deepcopy(obj)
来源：http://uyk.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://xxm.ivvv.top

JS:   structuredClone(obj)
来源：http://vmp.9152youxi.cn

TS:   structuredClone(obj)
来源：http://isz.xziqi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kxr.yj20258.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gbr.jqgfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://act.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://wzw.cheryme.top

[K06] 解析 URL 查询串
来源：http://cux.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://phi.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cob.zycfv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://afy.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rom.cashguo.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tnm.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xqv.zhoulong.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://twp.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fjt.xinyue.icu

[K07] 进制转换
来源：http://rhd.hesvh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dey.chenzaomai.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://icr.hongshengwenyu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ehm.guowangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ghw.daxiang520.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bqb.jinghuilouyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://byu.zycfv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zhs.jqgfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wki.tian-w.cn

[K08] 二进制序列化（非 JSON）
来源：http://egi.zhongyouzk.top

Py:   pickle.dumps(obj)
来源：http://qsn.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xui.xziqi.cn

JS:   v8.serialize(obj)        // Node
来源：http://fxa.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://brs.fengsongda.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://brk.jyoumei.cn

Go:   encoding/gob
来源：http://yxl.gogol.net.cn

Ruby: Marshal.dump(obj)
来源：http://yfh.cqqwz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rhu.cashguo.top

================================================================================
来源：http://jfo.zhengqikj.top

L. 网络请求
来源：http://rto.jinqigfzy.top

================================================================================
来源：http://ral.jianghu66.top

[L01] 发送 GET 请求
来源：http://zqr.gzhubu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rei.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xho.xylfe.cn

JS:   await fetch(url)
来源：http://ktk.bjfxy.top

TS:   await fetch(url)
来源：http://dqa.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://foc.yj20258.top

Go:   resp, err := http.Get(url)
来源：http://zaa.fzhhl.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uib.hongshengwenyu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kqj.c1oappe.top

[L02] 发送 POST JSON
来源：http://rau.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://vzm.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dik.shzxlz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yjd.jinyuanbaomall.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ppq.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ecy.gotoacloud.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tvg.wangshuangyany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sco.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://geq.hammf.cn

[L03] 设置自定义请求头
来源：http://vom.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bgw.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zrj.xziqi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fmv.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://azl.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ieb.316326.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zbw.52xcode.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ezz.nanxinkj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mnv.havefunace.top

[L04] 设置超时
来源：http://ihv.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://fzs.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lpj.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gdz.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ykt.nanxuanxn.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wdk.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nqs.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://quw.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gzh.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://jgi.jlsjyb.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dfa.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zyj.yvedp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vom.zhaomingkeji.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tps.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mhl.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ons.uphjek.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xsd.yvedp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://foc.c1oappe.top

[L06] 解析响应为 JSON
来源：http://xdq.zhaomingkeji.xyz

Py:   resp.json()
来源：http://bml.pengpengdd.cyou

PHP:  json_decode($body, true);
来源：http://aqi.shuidangran.top

JS:   await resp.json()
来源：http://slx.fktsv.cn

TS:   await resp.json()
来源：http://cvh.shanyushiyangtech.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pin.ivvv.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://erl.feifeiyinyue.top

Ruby: JSON.parse(resp.body)
来源：http://yld.fzhhl.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tbk.ydjk.org.cn

[L07] 处理 HTTP 状态码
来源：http://luc.yueranfly.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ztg.tanke756.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://obv.fehbvm.com

JS:   resp.ok;  resp.status
来源：http://pcw.sweek.top

TS:   resp.ok;  resp.status
来源：http://mjy.yj20258.top

Java: resp.statusCode()
来源：http://icp.meibo888.top

Go:   resp.StatusCode
来源：http://zim.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://ejw.feifeiyinyue.top

C#:   (int)resp.StatusCode
来源：http://cxc.chenzaomai.com

[L08] 并发请求多个地址
来源：http://gjm.hywenlv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aea.yfazqb.com

PHP:  curl_multi_init() 系列
来源：http://sjq.hnxiangtu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yek.xylfe.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jqg.0kj1m.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mkz.zhoulong.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://coy.bjfxy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wes.sufxvd.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hyt.fktsv.cn

================================================================================
来源：http://kfk.vehdjk.com

M. 命令行 / 进程 / 环境
来源：http://wan.hammf.cn

================================================================================
来源：http://how.yj20258888.top

[M01] 读取命令行参数
来源：http://jwu.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://iet.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://lcg.yueranfly.top

JS:   process.argv.slice(2)
来源：http://jwy.gotoacloud.top

TS:   process.argv.slice(2)
来源：http://wgp.ehwqpu.com

Java: args 数组（main 方法参数）
来源：http://gwc.hywenlv.cn

Go:   os.Args[1:]
来源：http://jeo.cqqwz.cn

Ruby: ARGV
来源：http://jkq.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://mdc.fehbvm.com

[M02] 读取环境变量
来源：http://otd.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://gkg.ivvv.top


<!-- 参考信息 -->