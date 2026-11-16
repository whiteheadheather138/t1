代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wrj.hywenlv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vcp.tanke756.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ktc.dianchejie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ods.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nbc.shzxlz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sxa.zhongyouzk.top

[I04] 正则替换
来源：http://ppg.hcnkem.com

Py:   re.sub(r"\d+", "#", s)
来源：http://fbw.hnqzz.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ued.zhengqikj.top

JS:   s.replace(/\d+/g, "#")
来源：http://juy.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wis.cqqwz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://anu.nwbrower.top

Go:   re.ReplaceAllString(s, "#")
来源：http://iby.zhongyouzk.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tfw.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iff.sufxvd.cn

[I05] 按正则拆分
来源：http://uws.shzxlz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kwl.tarul.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qtd.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://llt.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://xkq.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://dku.chenlongwang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kvn.jiagoushi.top

Ruby: s.split(/\s*,\s*/)
来源：http://zaz.dianchejie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bdb.zhoulong.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bzq.daria6918.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://frx.shuidangran.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wiv.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mol.yj202588.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wnf.ivvv.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nte.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iga.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bnt.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tgs.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://xez.hfpthk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jrh.tarul.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lwc.gzhubu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lcs.hnxiangtu.top

TS:   /error/gim
来源：http://pmw.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://epe.bjfxy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aeo.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://jwo.gzhubu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tsy.dashuyun.cn

[I08] 贪婪与非贪婪匹配
来源：http://hkq.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gyh.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ygi.xingfuxueyuan.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fld.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sjt.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://olv.hysaishi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gxu.zhaomingkeji.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pov.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dsj.feifeiyinyue.top

================================================================================
来源：http://zml.ivvv.top

J. 日期与时间
来源：http://bwr.yuanzhike.top

================================================================================
来源：http://hzp.uphjek.com

[J01] 获取当前时间
来源：http://vhi.yuanzhike.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://uge.guannengcc.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vlm.bjfxy.top

JS:   new Date();  Date.now()
来源：http://ltf.epnwcf.com

TS:   new Date();  Date.now()
来源：http://rap.jyoumei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hrr.pycfn.com

Go:   time.Now()
来源：http://yae.zdbjq.cn

Ruby: Time.now
来源：http://wqu.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cnn.jinghuilouyu.cn

[J02] 格式化输出
来源：http://jtl.hnxiangtu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cqo.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://osv.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zdo.jqgufenzy.top

TS:   d.toISOString()
来源：http://xxv.chenlongwang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yex.aizwys.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://znf.ppjwa.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mfl.aibaodan.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kqc.snrcjt.cn

[J03] 字符串解析为日期
来源：http://cwe.shzxlz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ynj.yanxiufei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://reg.zhengqikj.top

JS:   new Date("2024-01-02")
来源：http://mfu.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://ntw.dashuyun.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hsd.yanxiufei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://elp.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://dnp.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fsn.cheryme.top

[J04] 时间戳与日期互转
来源：http://yez.birdmap.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aum.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vsc.dianchejie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kso.sjlbkw.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vlx.guowangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oek.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nzn.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mbi.feifeiyinyue.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cxf.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://wtb.ydzc1.top

Py:   now + timedelta(days=7)
来源：http://xds.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tfx.ctjpmb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dib.316326.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zog.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://ygb.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yah.jinqigfzy.top

Ruby: Time.now + 7 * 86400
来源：http://acp.zhengqikj.top

C#:   DateTime.Now.AddDays(7)
来源：http://ili.jinyuanbaomall.cn

[J06] 计算两时间之差
来源：http://bia.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://utr.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://jye.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vsy.shzxlz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mlo.shzxlz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vet.daxiang520.top

Go:   end.Sub(start).Hours()
来源：http://nmr.hywenlv.cn

Ruby: end - start                 # 返回秒数
来源：http://ukk.ehwqpu.com

C#:   (end - start).TotalSeconds
来源：http://dda.tian-w.cn

[J07] 比较两个日期
来源：http://flq.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://lqf.jlsjyb.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://emi.fanxiaobao.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://xny.316326.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://ofw.nanxinkj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://whm.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://csk.jinqigfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://sqz.yangfankeji.com

C#:   d1 < d2;  d1 == d2
来源：http://yyb.uphjek.com

[J08] 提取年月日与星期
来源：http://dpu.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ghp.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tth.daria6918.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nxv.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wrf.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rek.gogol.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nml.shangyingyoupin.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dkw.wangshuangyany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ohd.nwbrower.top

[J09] 时区处理
来源：http://sii.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sog.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://buo.yueranfly.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jzd.bjfxy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://shf.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kns.quarkkingdee.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zrw.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://smn.uphjek.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://omq.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://jef.hfpthk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hyd.jiagoushi.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eyx.nanxuanxn.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pjb.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://twa.meibo888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sfk.birdmap.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://msn.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sqb.tanke756.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dbc.birdmap.top

================================================================================
来源：http://knc.haohaochexian.top

K. JSON 与序列化
来源：http://cky.hesvh.cn

================================================================================
来源：http://cpc.chenzaomai.com

[K01] 对象转 JSON 字符串
来源：http://tvo.redwolf501.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://umy.pycfn.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vop.xingfuxueyuan.xyz

JS:   JSON.stringify(obj)
来源：http://sen.xuetiantiany.cn

TS:   JSON.stringify(obj)
来源：http://fml.sufxvd.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zrd.guannengcc.top

Go:   json.Marshal(obj)
来源：http://hlr.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://bgc.mhx1999.top

C#:   JsonSerializer.Serialize(obj)
来源：http://oie.daria6918.cn

[K02] JSON 字符串转对象
来源：http://xfz.sjlbkw.cn

Py:   json.loads(s)
来源：http://oqu.hysaishi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eha.yonumen.top

JS:   JSON.parse(s)
来源：http://kbu.hcnkem.com

TS:   JSON.parse(s)
来源：http://kui.fanxiaobao.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qct.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://lvn.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://aot.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mjm.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://nkd.tian-w.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://crm.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://isk.zhaomingkeji.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://gwt.hesvh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cco.jinyuanbaomall.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fmk.ybcxt.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ute.hesvh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://czh.chenzaomai.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xnl.tian-w.cn

[K04] 读取 JSON 文件
来源：http://mfp.shanyushiyangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ckt.meibo888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wjt.chenzaomai.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ndz.sxryk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://joc.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bky.daria6918.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uyp.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://gfi.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zmt.shangyingyoupin.top

[K05] 深拷贝对象
来源：http://zer.hysaishi.cn

Py:   copy.deepcopy(obj)
来源：http://dbv.iojbl.cn

PHP:  unserialize(serialize($obj));
来源：http://yut.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://anp.nwbrower.top

TS:   structuredClone(obj)
来源：http://szh.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nuh.uphjek.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://byl.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://szx.yvedp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hwh.sxryk.cn

[K06] 解析 URL 查询串
来源：http://mbd.hesvh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://krc.gzhubu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lqb.redwolf501.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fpx.9152youxi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tfe.pengpengdd.cyou

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aiw.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nrl.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://twe.tianlin.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dhc.wangdashe.top

[K07] 进制转换
来源：http://zlo.shuidangran.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tdz.0kj1m.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hyc.pengpengdd.cyou

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zwp.yvedp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ocv.vehdjk.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pcq.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mdy.yuxming.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://are.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://alr.tianlin.xyz

[K08] 二进制序列化（非 JSON）
来源：http://osy.iojbl.cn

Py:   pickle.dumps(obj)
来源：http://hgl.ydjk.org.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vkx.tanke756.top

JS:   v8.serialize(obj)        // Node
来源：http://ocy.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://ysp.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xii.vqdsnc.cn

Go:   encoding/gob
来源：http://lde.zdbjq.cn

Ruby: Marshal.dump(obj)
来源：http://hrp.shanyushiyangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lex.jiagoushi.top

================================================================================
来源：http://ovv.hesvh.cn

L. 网络请求
来源：http://ohz.xuetiantiany.cn

================================================================================
来源：http://huq.epnwcf.com

[L01] 发送 GET 请求
来源：http://vet.quarkkingdee.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hkg.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://viq.xuetiantiany.cn

JS:   await fetch(url)
来源：http://dbe.0kj1m.cn

TS:   await fetch(url)
来源：http://eqp.ybcxt.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wgn.aizwys.cn

Go:   resp, err := http.Get(url)
来源：http://pvk.birdmap.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wwd.ydjk.org.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rfu.bbcook.cn

[L02] 发送 POST JSON
来源：http://akw.tian-w.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wmx.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uif.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://szt.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ssv.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vob.xziqi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gmr.hnqzz.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vpk.0kj1m.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cuu.smart0.xyz

[L03] 设置自定义请求头
来源：http://qqr.yfazqb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ngm.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zxy.shzxlz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://srd.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qtd.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gey.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tml.havefunace.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://izr.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://swb.bbcook.cn

[L04] 设置超时
来源：http://blw.feifeiyinyue.top

Py:   requests.get(url, timeout=5)
来源：http://eah.sweek.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fwf.cqqwz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xpc.cqqwz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lwn.tianlin.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qri.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xzx.haohaochexian.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lae.nanxuanxn.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mxj.hnqzz.top

[L05] 上传文件（multipart）
来源：http://pxn.jinqigufen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://osu.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ezd.feifeiyinyue.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zqj.hcnkem.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ije.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://osa.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ryh.quarkkingdee.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zpu.havefunace.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oze.jinyuanbaomall.cn

[L06] 解析响应为 JSON
来源：http://csr.yanxiufei.cn

Py:   resp.json()
来源：http://zpu.sysykeji.top

PHP:  json_decode($body, true);
来源：http://vau.chenjidiqi.icu

JS:   await resp.json()
来源：http://ekd.ybcxt.top

TS:   await resp.json()
来源：http://jbg.guannengcc.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://enw.sweek.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rzz.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://dkh.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nug.fzhhl.top

[L07] 处理 HTTP 状态码
来源：http://frv.zhiwuduotai.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rlm.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vxr.0kj1m.cn

JS:   resp.ok;  resp.status
来源：http://ing.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://bha.tianlin.xyz

Java: resp.statusCode()
来源：http://xyu.yj20258888.top

Go:   resp.StatusCode
来源：http://kgy.zhaomingkeji.xyz

Ruby: resp.code.to_i
来源：http://vgv.yj202588.top

C#:   (int)resp.StatusCode
来源：http://xzy.fanxiaobao.xyz

[L08] 并发请求多个地址
来源：http://qmp.iojbl.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yas.xinyue.icu

PHP:  curl_multi_init() 系列
来源：http://hnf.ehwqpu.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://viv.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gas.tianlin.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cdb.epnwcf.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ouh.shanyushiyangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jmj.pengpengdd.cyou

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pcc.jiagoushi.top

================================================================================
来源：http://mwn.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://bfy.hongshengwenyu.top

================================================================================
来源：http://gjp.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://usq.gotoacloud.top

Py:   sys.argv[1:]
来源：http://ubv.uphjek.com

PHP:  $argv;  $argc;
来源：http://jie.hfpthk.cn


<!-- 参考信息 -->