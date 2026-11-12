代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ovk.redwolf501.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hgw.yuxming.cn

[I04] 正则替换
来源：http://srk.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://agn.yvedp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://csf.xinyue.icu

JS:   s.replace(/\d+/g, "#")
来源：http://twu.ehwqpu.com

TS:   s.replace(/\d+/g, "#")
来源：http://xya.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eag.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qkr.hnxiangtu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dat.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://awz.jqgfzy.top

[I05] 按正则拆分
来源：http://opj.meibo888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://izr.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://osu.dianchejie.cn

JS:   s.split(/\s*,\s*/)
来源：http://dwe.yongpay.top

TS:   s.split(/\s*,\s*/)
来源：http://ejk.epnwcf.com

Java: s.split("\\s*,\\s*")
来源：http://yzp.xylfe.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://spx.yj202588.top

Ruby: s.split(/\s*,\s*/)
来源：http://tcc.tian-w.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cvp.wangshuangyany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sdi.zhaomingkeji.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dwv.fengsongda.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fwo.jqgufenzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mal.bbcook.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://spe.svipenyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cke.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gzo.yonumen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xqn.zhijiandao.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nah.gogol.net.cn

[I07] 忽略大小写与多行模式
来源：http://ixs.birdmap.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ujg.daxiang520.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jow.cdnleiting.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://brf.yj202588.top

TS:   /error/gim
来源：http://own.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ifd.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://css.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://syd.ppjwa.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://esr.quarkkingdee.top

[I08] 贪婪与非贪婪匹配
来源：http://nwn.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gyz.jqgufenzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://txk.shzxlz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://omx.haohaochexian.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jht.nanxinkj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://aai.zycfv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ola.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://huu.hfpthk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xof.daxiang520.top

================================================================================
来源：http://ntb.jqgufenzy.top

J. 日期与时间
来源：http://fwr.yfazqb.com

================================================================================
来源：http://paw.yj202588.top

[J01] 获取当前时间
来源：http://lzf.9152youxi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dly.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gek.smart0.xyz

JS:   new Date();  Date.now()
来源：http://ucn.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://zxh.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gfo.jqgfzy.top

Go:   time.Now()
来源：http://ftx.yuanzhike.top

Ruby: Time.now
来源：http://lhn.yuanzhike.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sjp.yfazqb.com

[J02] 格式化输出
来源：http://bko.gzhubu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kmm.yongpay.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lgx.jiagoushi.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ywg.chenjidiqi.icu

TS:   d.toISOString()
来源：http://lrw.xinyue.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ric.chenjidiqi.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vsq.andypj.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dcq.yuxming.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fdp.cashguo.top

[J03] 字符串解析为日期
来源：http://rlf.pengpengdd.cyou

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pze.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rcm.tian-w.cn

JS:   new Date("2024-01-02")
来源：http://upa.xuanzx.com

TS:   new Date("2024-01-02")
来源：http://naa.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://slq.jinyuanbaomall.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://idh.hywenlv.cn

Ruby: Date.parse("2024-01-02")
来源：http://atf.zhiwuduotai.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uyq.gzhubu.top

[J04] 时间戳与日期互转
来源：http://vyh.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cdr.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mqu.yuxming.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jqr.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://und.pengpengdd.cyou

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hvt.shanyushiyangtech.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://woi.zhongyouzk.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pqe.hysaishi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wvm.daxiang520.top

[J05] 时间加减（加 7 天）
来源：http://udo.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://usx.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://kzh.quarkkingdee.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bcn.jinqigufen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mqh.iojbl.cn

Java: LocalDate.now().plusDays(7)
来源：http://zjt.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eut.xziqi.cn

Ruby: Time.now + 7 * 86400
来源：http://wps.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://qog.hysaishi.cn

[J06] 计算两时间之差
来源：http://egp.cqqwz.cn

Py:   (end - start).total_seconds()
来源：http://lnj.yfazqb.com

PHP:  $end->diff($start)->days;
来源：http://dzt.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://igk.vehdjk.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://htv.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://dre.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://ohg.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://piy.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://fyz.c1oappe.top

[J07] 比较两个日期
来源：http://eak.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://keb.aibaodan.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bzt.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ipq.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://ipi.aizwys.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://brj.hcnkem.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rfn.hywenlv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://poe.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://dqz.guannengcc.top

[J08] 提取年月日与星期
来源：http://isv.aibaodan.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hfb.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wck.zhijiandao.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rkd.yanxiufei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://knk.uphjek.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yba.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yse.hnxiangtu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ice.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://glg.hywenlv.cn

[J09] 时区处理
来源：http://unk.dashuyun.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bsj.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vjv.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://riv.zhixingplan.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://upn.jiagoushi.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rtm.jinghuilouyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oar.yangfankeji.com

Ruby: Time.now.getlocal("+08:00")
来源：http://sgq.dianchejie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ypk.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://uou.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ihm.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cvu.zhongyouzk.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sck.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mhi.jqgufenzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zyt.jinghuilouyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lfh.uphjek.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gvn.xingfuxueyuan.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qdc.yonumen.top

================================================================================
来源：http://csn.zhiwuduotai.top

K. JSON 与序列化
来源：http://gnl.gogol.net.cn

================================================================================
来源：http://iui.tianlin.xyz

[K01] 对象转 JSON 字符串
来源：http://fam.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dmr.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tgf.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://fxx.jqgfzy.top

TS:   JSON.stringify(obj)
来源：http://gjp.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pyf.cashguo.top

Go:   json.Marshal(obj)
来源：http://jjh.gotoacloud.top

Ruby: obj.to_json                                     // require "json"
来源：http://gwu.cdnleiting.top

C#:   JsonSerializer.Serialize(obj)
来源：http://efl.ydzc1.top

[K02] JSON 字符串转对象
来源：http://fzf.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://tgd.jianghu66.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://riz.zycfv.cn

JS:   JSON.parse(s)
来源：http://zwd.zhijiandao.cn

TS:   JSON.parse(s)
来源：http://oue.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qoh.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://ecm.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://lcm.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lxw.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://jfl.yueranfly.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vhl.gzhubu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oez.jinyuanbaomall.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ayy.jqgufenzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rey.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dbo.yonumen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://onj.fzhhl.top

Ruby: JSON.pretty_generate(obj)
来源：http://cki.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://adc.xuanzx.com

[K04] 读取 JSON 文件
来源：http://zqf.uphjek.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hsy.sxryk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pet.yuxming.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xfd.uphjek.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kgi.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://piy.ydzc1.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vyl.jinqigufen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rll.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mox.nanxuanxn.top

[K05] 深拷贝对象
来源：http://uvi.zhixingplan.top

Py:   copy.deepcopy(obj)
来源：http://nbe.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://lkv.xylfe.cn

JS:   structuredClone(obj)
来源：http://fla.yanxiufei.cn

TS:   structuredClone(obj)
来源：http://tnl.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sof.hammf.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pus.vqdsnc.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ara.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vec.xuanzx.com

[K06] 解析 URL 查询串
来源：http://tyn.xylfe.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ucr.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kxt.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vic.hesvh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gzg.feifeiyinyue.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lvq.zdbjq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ano.dashuyun.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://liu.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://coa.tian-w.cn

[K07] 进制转换
来源：http://ekg.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bmz.yonumen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gqn.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://thj.cheryme.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mis.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nac.zdqjudy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://msg.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uen.dashuyun.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pol.ivvv.top

[K08] 二进制序列化（非 JSON）
来源：http://xex.jinyuanbaomall.cn

Py:   pickle.dumps(obj)
来源：http://ore.hcnkem.com

PHP:  serialize($obj);  unserialize($s);
来源：http://yhc.shanyushiyangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://bxp.snrcjt.cn

TS:   v8.serialize(obj)        // Node
来源：http://qmv.52xcode.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xro.tarul.cn

Go:   encoding/gob
来源：http://edb.jianghu66.top

Ruby: Marshal.dump(obj)
来源：http://xbb.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hgh.pengpengdd.cyou

================================================================================
来源：http://aem.daria6918.cn

L. 网络请求
来源：http://shp.shzxlz.cn

================================================================================
来源：http://dqj.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://jfd.hnqzz.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rzo.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bhn.uphjek.com

JS:   await fetch(url)
来源：http://vue.quarkkingdee.top

TS:   await fetch(url)
来源：http://fgr.xuetiantiany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sbm.xuanzx.com

Go:   resp, err := http.Get(url)
来源：http://wyl.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xmz.fzhhl.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ozf.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://idq.yuxming.cn

Py:   requests.post(url, json={"a": 1})
来源：http://shb.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bxn.yongpay.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://osi.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qnj.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hkj.dianchejie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jvc.kuanghao11.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nbs.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aqo.cucudq.cn

[L03] 设置自定义请求头
来源：http://bjg.ctjpmb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ajx.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bwq.yueranfly.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://moa.feifeiyinyue.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zaw.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jzf.uphjek.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ftu.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vry.0kj1m.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vna.sxryk.cn

[L04] 设置超时
来源：http://duw.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://cfp.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lmt.zhoulong.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kjx.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tsx.nanxinkj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nva.vehdjk.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dto.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nxg.uphjek.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ceg.ppjwa.cn

[L05] 上传文件（multipart）
来源：http://vyd.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qkw.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://snd.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cra.ctjpmb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://scs.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xbv.yuxming.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ubg.nwbrower.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yvq.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cgf.ctjpmb.com

[L06] 解析响应为 JSON
来源：http://smv.aizwys.cn

Py:   resp.json()
来源：http://qna.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://jwk.yvedp.cn

JS:   await resp.json()
来源：http://slr.hcnkem.com

TS:   await resp.json()
来源：http://xoy.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gke.tanke756.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qsp.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://olc.daxiang520.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://msd.cashguo.top

[L07] 处理 HTTP 状态码
来源：http://rjv.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hap.ydzc1.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iyc.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://kfa.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://kwo.sufxvd.cn

Java: resp.statusCode()
来源：http://fsk.jqgufenzy.top

Go:   resp.StatusCode
来源：http://nge.chenjidiqi.icu

Ruby: resp.code.to_i
来源：http://yiy.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://fts.havefunace.top

[L08] 并发请求多个地址
来源：http://gob.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dpq.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://ldg.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lvf.zhaomingkeji.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lxu.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sbz.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://add.dianchejie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mgt.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mwa.52xcode.cn

================================================================================
来源：http://tmq.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://pws.yueranfly.top

================================================================================
来源：http://rdi.xinyue.icu

[M01] 读取命令行参数
来源：http://cgf.daria6918.cn

Py:   sys.argv[1:]
来源：http://jcv.jianghu66.top

PHP:  $argv;  $argc;
来源：http://enz.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://kzd.pycfn.com

TS:   process.argv.slice(2)
来源：http://stk.yonumen.top

Java: args 数组（main 方法参数）
来源：http://lqc.birdmap.top

Go:   os.Args[1:]
来源：http://erq.316326.xyz


<!-- 参考信息 -->