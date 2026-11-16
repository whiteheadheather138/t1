代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vce.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://raw.mhx1999.top

TS:   s.replace(/\d+/g, "#")
来源：http://ybi.zhixingplan.top

Java: s.replaceAll("\\d+", "#")
来源：http://fga.ywan-chungtsiang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://eme.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mln.xziqi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://edg.hywenlv.cn

[I05] 按正则拆分
来源：http://zgm.feifeiyinyue.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nvf.haohaochexian.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vyc.tian-w.cn

JS:   s.split(/\s*,\s*/)
来源：http://gfn.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://hwb.gaohongyu789.top

Java: s.split("\\s*,\\s*")
来源：http://utk.jinqigfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uhy.ybcxt.top

Ruby: s.split(/\s*,\s*/)
来源：http://lgc.hysaishi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://adh.daria6918.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kpi.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vtm.ydzc1.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://opw.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gwc.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wka.hywenlv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cmg.gzhubu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tgh.tarul.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oiy.zhaomingkeji.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kdq.redwolf501.top

[I07] 忽略大小写与多行模式
来源：http://efr.nanxuanxn.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mpl.zhijiandao.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://onj.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zjh.ppjwa.cn

TS:   /error/gim
来源：http://aiz.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lxp.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pkm.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://lcz.iojbl.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sih.ctjpmb.com

[I08] 贪婪与非贪婪匹配
来源：http://ylo.yfazqb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lpn.guowangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://trm.zhixingplan.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://koi.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ufw.kuanghao11.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nch.9152youxi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ili.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ctq.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://que.yangfankeji.com

================================================================================
来源：http://rze.zhijiandao.cn

J. 日期与时间
来源：http://opf.shzxlz.cn

================================================================================
来源：http://vtp.hcnkem.com

[J01] 获取当前时间
来源：http://vfh.xuetiantiany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dqv.cdnleiting.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dxc.tanke756.top

JS:   new Date();  Date.now()
来源：http://ksa.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://rgi.vqdsnc.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tfr.nwbrower.top

Go:   time.Now()
来源：http://xah.gzhubu.top

Ruby: Time.now
来源：http://wcq.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oan.sjlbkw.cn

[J02] 格式化输出
来源：http://plo.guannengcc.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://efr.hnqzz.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://knj.nwbrower.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://csc.xinyue.icu

TS:   d.toISOString()
来源：http://sim.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zke.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dhk.xuanzx.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pvh.jyoumei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xht.tianlin.xyz

[J03] 字符串解析为日期
来源：http://arr.guowangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://itj.ywan-chungtsiang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pxl.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://fys.hnxiangtu.top

TS:   new Date("2024-01-02")
来源：http://mgh.9152youxi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ofg.wangshuangyany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xfk.zhongyouzk.top

Ruby: Date.parse("2024-01-02")
来源：http://jop.gaohongyu789.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://chi.ctjpmb.com

[J04] 时间戳与日期互转
来源：http://dqq.ehwqpu.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yok.hfpthk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://osd.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xzn.xylfe.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nqs.zhongyouzk.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ipc.9152youxi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rhl.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pnk.hnqzz.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://obx.bjfxy.top

[J05] 时间加减（加 7 天）
来源：http://ybe.yj202588.top

Py:   now + timedelta(days=7)
来源：http://vof.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ntb.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tpl.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zbi.mhx1999.top

Java: LocalDate.now().plusDays(7)
来源：http://ilh.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qtx.sweek.top

Ruby: Time.now + 7 * 86400
来源：http://jwv.yj20258.top

C#:   DateTime.Now.AddDays(7)
来源：http://hsd.sjlbkw.cn

[J06] 计算两时间之差
来源：http://tsa.ydjk.org.cn

Py:   (end - start).total_seconds()
来源：http://xbj.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://tei.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bbp.jinqigfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://prp.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sqt.redwolf501.top

Go:   end.Sub(start).Hours()
来源：http://nga.tanke756.top

Ruby: end - start                 # 返回秒数
来源：http://fda.guannengcc.top

C#:   (end - start).TotalSeconds
来源：http://roc.cucudq.cn

[J07] 比较两个日期
来源：http://kes.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://lir.shuidangran.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pqq.daxiang520.top

JS:   d1.getTime() < d2.getTime()
来源：http://zjf.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://okq.tanke756.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ipa.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fhp.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://ygj.fanxiaobao.xyz

C#:   d1 < d2;  d1 == d2
来源：http://miv.gogol.net.cn

[J08] 提取年月日与星期
来源：http://cgi.hfpthk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mgp.jinqigfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://udb.fehbvm.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wwc.zhengqikj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bpu.ybcxt.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fpv.yanxiufei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ggp.wangdashe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://knd.chenjidiqi.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cbk.nwbrower.top

[J09] 时区处理
来源：http://tkx.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kzl.tian-w.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wjo.havefunace.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qoj.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://esr.nanxuanxn.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rcn.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pok.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://olr.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hdp.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://kpo.yfazqb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ibh.c1oappe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zlm.chenlongwang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://asn.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ayt.kuanghao11.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aby.ppjwa.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tce.jqgufenzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://goh.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mru.aibaodan.cn

================================================================================
来源：http://jhl.ctjpmb.com

K. JSON 与序列化
来源：http://kga.vqdsnc.cn

================================================================================
来源：http://pmb.guowangkeji.top

[K01] 对象转 JSON 字符串
来源：http://bee.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xzs.xuanzx.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://muu.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://nzo.smart0.xyz

TS:   JSON.stringify(obj)
来源：http://yqf.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pix.yuanzhike.top

Go:   json.Marshal(obj)
来源：http://ctg.mhx1999.top

Ruby: obj.to_json                                     // require "json"
来源：http://sne.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://top.epnwcf.com

[K02] JSON 字符串转对象
来源：http://rae.pengpengdd.cyou

Py:   json.loads(s)
来源：http://zcd.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://szc.tian-w.cn

JS:   JSON.parse(s)
来源：http://nxd.havefunace.top

TS:   JSON.parse(s)
来源：http://gcy.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vht.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://hbs.zdbjq.cn

Ruby: JSON.parse(s)
来源：http://ixp.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://giv.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://uou.yj20258.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pwi.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bwl.feifeiyinyue.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bua.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qfb.nanxuanxn.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qcx.ivvv.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mon.xylfe.cn

Ruby: JSON.pretty_generate(obj)
来源：http://afs.smart0.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://axz.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://cfl.yuxming.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jms.yongpay.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gcr.zhaomingkeji.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zwn.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yjc.pycfn.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pqb.xuanzx.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://izv.ppjwa.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gsz.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lbv.gogol.net.cn

[K05] 深拷贝对象
来源：http://thi.meibo888.top

Py:   copy.deepcopy(obj)
来源：http://rab.wangdashe.top

PHP:  unserialize(serialize($obj));
来源：http://vzn.ppjwa.cn

JS:   structuredClone(obj)
来源：http://aow.yueranfly.top

TS:   structuredClone(obj)
来源：http://ues.redwolf501.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dzp.jqgfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qrv.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wru.haohaochexian.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wkj.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://igj.zhoulong.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dtu.sysykeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://und.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pdt.pycfn.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ytz.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qff.hnxiangtu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://agr.haohaochexian.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ftk.yj202588.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kyg.316326.xyz

[K07] 进制转换
来源：http://yjs.ybcxt.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xfu.kuanghao11.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qrq.xziqi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pki.epnwcf.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mgb.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mrn.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bsf.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lrl.52xcode.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://npc.9152youxi.cn

[K08] 二进制序列化（非 JSON）
来源：http://ikg.quarkkingdee.top

Py:   pickle.dumps(obj)
来源：http://txb.zdbjq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://haq.aibaodan.cn

JS:   v8.serialize(obj)        // Node
来源：http://psj.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://sej.fehbvm.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ukl.zdbjq.cn

Go:   encoding/gob
来源：http://kqr.sysykeji.top

Ruby: Marshal.dump(obj)
来源：http://bxb.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wez.hywenlv.cn

================================================================================
来源：http://ahq.zycfv.cn

L. 网络请求
来源：http://jqi.nanxinkj.top

================================================================================
来源：http://wef.hnqzz.top

[L01] 发送 GET 请求
来源：http://nms.jinqigufen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wiy.yvedp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://crb.nwbrower.top

JS:   await fetch(url)
来源：http://sul.ehwqpu.com

TS:   await fetch(url)
来源：http://ula.xziqi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wne.shzxlz.cn

Go:   resp, err := http.Get(url)
来源：http://enf.cqqwz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qdw.shangyingyoupin.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zod.xylfe.cn

[L02] 发送 POST JSON
来源：http://pzb.tian-w.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nqg.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fzq.ybcxt.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eut.hysaishi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://igg.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://brq.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ufc.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fep.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yyd.fktsv.cn

[L03] 设置自定义请求头
来源：http://ndh.snrcjt.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uti.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xiq.kuanghao11.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qnw.zhaomingkeji.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vnw.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zak.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wik.iojbl.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vyy.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bak.ppjwa.cn

[L04] 设置超时
来源：http://six.tian-w.cn

Py:   requests.get(url, timeout=5)
来源：http://hbh.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aeo.wangshuangyany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qwz.hnqzz.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yed.fehbvm.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qex.birdmap.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wrh.guannengcc.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iya.iojbl.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vxh.zdbjq.cn

[L05] 上传文件（multipart）
来源：http://lwr.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://njo.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vbv.cheryme.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://shc.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zca.xylfe.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pig.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kgb.zdbjq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wkj.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gng.hnxiangtu.top

[L06] 解析响应为 JSON
来源：http://jya.vehdjk.com

Py:   resp.json()
来源：http://sjj.dianchejie.cn

PHP:  json_decode($body, true);
来源：http://xrk.ywan-chungtsiang.top

JS:   await resp.json()
来源：http://rny.sufxvd.cn

TS:   await resp.json()
来源：http://pwq.cashguo.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sqp.daria6918.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ncx.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://iqx.cheryme.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://adv.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://day.yueranfly.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mwy.pycfn.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yag.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://sah.316326.xyz

TS:   resp.ok;  resp.status
来源：http://bsq.yuxming.cn

Java: resp.statusCode()
来源：http://auu.epnwcf.com

Go:   resp.StatusCode
来源：http://ttt.andypj.xyz

Ruby: resp.code.to_i
来源：http://abe.xuetiantiany.cn

C#:   (int)resp.StatusCode
来源：http://jst.fzhhl.top

[L08] 并发请求多个地址
来源：http://oms.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mwo.fengsongda.top

PHP:  curl_multi_init() 系列
来源：http://ker.fengsongda.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rvu.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hta.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ljj.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ibd.ivvv.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://onf.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iop.jiagoushi.top

================================================================================
来源：http://mhw.uphjek.com

M. 命令行 / 进程 / 环境
来源：http://hnk.zdbjq.cn

================================================================================
来源：http://baa.ydjk.org.cn

[M01] 读取命令行参数
来源：http://zcd.uphjek.com

Py:   sys.argv[1:]
来源：http://xmr.ydjk.org.cn

PHP:  $argv;  $argc;
来源：http://shw.yvedp.cn

JS:   process.argv.slice(2)
来源：http://gbz.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://qtd.jyoumei.cn

Java: args 数组（main 方法参数）
来源：http://ety.c1oappe.top

Go:   os.Args[1:]
来源：http://jtu.zycfv.cn

Ruby: ARGV
来源：http://xot.nwbrower.top

C#:   args 数组（Main 方法参数）
来源：http://vld.chenzaomai.com

[M02] 读取环境变量
来源：http://xmu.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://dfj.c1oappe.top


<!-- 参考信息 -->