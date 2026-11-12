代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fgx.kuanghao11.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wou.jinqigufen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qnx.cheryme.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kbj.ctjpmb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ovh.jqgfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://frg.yueranfly.top

[I04] 正则替换
来源：http://dgm.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://utu.jinqigfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rko.pengpengdd.cyou

JS:   s.replace(/\d+/g, "#")
来源：http://vsz.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://bqi.ehwqpu.com

Java: s.replaceAll("\\d+", "#")
来源：http://aro.chenzaomai.com

Go:   re.ReplaceAllString(s, "#")
来源：http://fgf.wangshuangyany.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lyg.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ztg.bbcook.cn

[I05] 按正则拆分
来源：http://cqp.birdmap.top

Py:   re.split(r"\s*,\s*", s)
来源：http://apz.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nxd.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://blf.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://pxr.jlsjyb.cn

Java: s.split("\\s*,\\s*")
来源：http://dgm.jinqigufen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aaj.chenlongwang.top

Ruby: s.split(/\s*,\s*/)
来源：http://zgn.yj20258888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tqi.fanxiaobao.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vvh.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fvp.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fyx.c1oappe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hsl.yangfankeji.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jux.dianchejie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ssj.yfazqb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dua.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lht.316326.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uar.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://doh.jqgufenzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xwb.yuxming.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hhd.shzxlz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fmg.yangfankeji.com

TS:   /error/gim
来源：http://xzu.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xvx.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://myn.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://djb.ydjk.org.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bxx.xylfe.cn

[I08] 贪婪与非贪婪匹配
来源：http://xkh.smart0.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dap.bbcook.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mkv.9152youxi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lgr.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kba.gaohongyu789.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fme.fktsv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ozs.yangfankeji.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nqe.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ami.haohaochexian.top

================================================================================
来源：http://gkn.iojbl.cn

J. 日期与时间
来源：http://uzj.snrcjt.cn

================================================================================
来源：http://gwh.gotoacloud.top

[J01] 获取当前时间
来源：http://nuf.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tez.yueranfly.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bbs.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://kfl.yuanzhike.top

TS:   new Date();  Date.now()
来源：http://vzy.nanxinkj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tur.sweek.top

Go:   time.Now()
来源：http://qtk.cqqwz.cn

Ruby: Time.now
来源：http://czw.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mti.svipenyu.cn

[J02] 格式化输出
来源：http://sto.quarkkingdee.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bif.yuxming.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yad.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ibg.redwolf501.top

TS:   d.toISOString()
来源：http://jih.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ljk.ydzc1.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qie.xinyue.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://plu.hesvh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lpy.pycfn.com

[J03] 字符串解析为日期
来源：http://bea.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://feo.sweek.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lae.hnqzz.top

JS:   new Date("2024-01-02")
来源：http://bfg.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://jek.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://svn.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://shn.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://wpy.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://coo.pengpengdd.cyou

[J04] 时间戳与日期互转
来源：http://ptj.jqgfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://izt.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yob.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ujd.tian-w.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ozu.aibaodan.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ktq.shzxlz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jwr.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xbh.guowangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://spy.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://ogx.andypj.xyz

Py:   now + timedelta(days=7)
来源：http://esw.tianlin.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://keo.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ysl.zhongyouzk.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://men.snrcjt.cn

Java: LocalDate.now().plusDays(7)
来源：http://awc.hongshengwenyu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rck.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://igr.0kj1m.cn

C#:   DateTime.Now.AddDays(7)
来源：http://joo.haohaochexian.top

[J06] 计算两时间之差
来源：http://ser.52xcode.cn

Py:   (end - start).total_seconds()
来源：http://lmx.tanke756.top

PHP:  $end->diff($start)->days;
来源：http://gny.birdmap.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cqr.hfpthk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lbc.9152youxi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lmo.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://uiy.fehbvm.com

Ruby: end - start                 # 返回秒数
来源：http://cbp.jinghuilouyu.cn

C#:   (end - start).TotalSeconds
来源：http://bdk.chenlongwang.top

[J07] 比较两个日期
来源：http://ohd.9152youxi.cn

Py:   d1 < d2;  d1 == d2
来源：http://lwj.guowangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kfs.haohaochexian.top

JS:   d1.getTime() < d2.getTime()
来源：http://plu.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://deo.zhengqikj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fmv.yuxming.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://scq.52xcode.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hql.xinyue.icu

C#:   d1 < d2;  d1 == d2
来源：http://din.xziqi.cn

[J08] 提取年月日与星期
来源：http://ihu.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mih.cheryme.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cxr.cdnleiting.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iyd.pengpengdd.cyou

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mpl.gogol.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iyu.feifeiyinyue.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://shl.wangdashe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://coj.tian-w.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eum.jinqigufen.top

[J09] 时区处理
来源：http://wnd.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jaw.jqgufenzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hxy.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ycc.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nrk.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qqu.shuidangran.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lcl.gogol.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://aco.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eua.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://dah.ppjwa.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://llm.sxryk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dtu.zhijiandao.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bxu.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sef.yj20258888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://itx.hywenlv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xtw.9152youxi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://duc.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zvo.havefunace.top

================================================================================
来源：http://con.xziqi.cn

K. JSON 与序列化
来源：http://yal.smart0.xyz

================================================================================
来源：http://hgz.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://oun.cdnleiting.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://snk.smart0.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qst.gaohongyu789.top

JS:   JSON.stringify(obj)
来源：http://hlg.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://jzm.aibaodan.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qqu.316326.xyz

Go:   json.Marshal(obj)
来源：http://pno.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wdr.yfazqb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://gid.epnwcf.com

[K02] JSON 字符串转对象
来源：http://cye.kuanghao11.cn

Py:   json.loads(s)
来源：http://ovp.jinghuilouyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mtl.jianghu66.top

JS:   JSON.parse(s)
来源：http://qcu.zycfv.cn

TS:   JSON.parse(s)
来源：http://jan.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ptf.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://col.wangdashe.top

Ruby: JSON.parse(s)
来源：http://fto.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hdo.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://mtt.ctjpmb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://psd.dianchejie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://njt.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ldk.bjfxy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://uaj.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kft.nanxinkj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hxb.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vwf.yj202588.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dus.meibo888.top

[K04] 读取 JSON 文件
来源：http://oeq.svipenyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hew.tarul.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nmz.vqdsnc.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://frs.hnxiangtu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://atr.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://seu.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iyn.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://aat.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jqa.52xcode.cn

[K05] 深拷贝对象
来源：http://ljd.cqqwz.cn

Py:   copy.deepcopy(obj)
来源：http://pqm.ivvv.top

PHP:  unserialize(serialize($obj));
来源：http://fcj.aizwys.cn

JS:   structuredClone(obj)
来源：http://duk.snrcjt.cn

TS:   structuredClone(obj)
来源：http://mby.fengsongda.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uld.cucudq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eyg.hnxiangtu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cud.fzhhl.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mun.nwbrower.top

[K06] 解析 URL 查询串
来源：http://oql.jinyuanbaomall.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dud.xziqi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kgu.birdmap.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://diw.jyoumei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dws.yj20258888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://szy.nwbrower.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zjm.chenjidiqi.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jpj.ydjk.org.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rcx.ydjk.org.cn

[K07] 进制转换
来源：http://wci.nanxuanxn.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fan.birdmap.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oif.yvedp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jxh.tian-w.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dao.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hwt.shuidangran.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://voa.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xcc.hesvh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://psl.jqgufenzy.top

[K08] 二进制序列化（非 JSON）
来源：http://umf.yj202588.top

Py:   pickle.dumps(obj)
来源：http://dxa.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vmf.dianchejie.cn

JS:   v8.serialize(obj)        // Node
来源：http://mdh.wangshuangyany.cn

TS:   v8.serialize(obj)        // Node
来源：http://yjm.gotoacloud.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pla.sweek.top

Go:   encoding/gob
来源：http://fcc.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://yui.sjlbkw.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fux.jlsjyb.cn

================================================================================
来源：http://tqb.havefunace.top

L. 网络请求
来源：http://lfh.vqdsnc.cn

================================================================================
来源：http://xqn.ctjpmb.com

[L01] 发送 GET 请求
来源：http://tqx.ivvv.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fto.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ynr.kuanghao11.cn

JS:   await fetch(url)
来源：http://gas.zhijiandao.cn

TS:   await fetch(url)
来源：http://lyw.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://idu.sysykeji.top

Go:   resp, err := http.Get(url)
来源：http://pmv.yongpay.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wny.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yuh.nanxinkj.top

[L02] 发送 POST JSON
来源：http://zof.xuanzx.com

Py:   requests.post(url, json={"a": 1})
来源：http://zll.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bas.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zaz.meibo888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wui.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zvw.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://knj.dashuyun.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hyj.ppjwa.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yae.smart0.xyz

[L03] 设置自定义请求头
来源：http://daj.hnqzz.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ysg.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qog.yvedp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fet.hcnkem.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yfj.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lni.cqqwz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ehp.ehwqpu.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qyw.yj20258888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dtf.sysykeji.top

[L04] 设置超时
来源：http://zod.zhixingplan.top

Py:   requests.get(url, timeout=5)
来源：http://yqm.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ngp.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mkw.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nto.ybcxt.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://til.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://evq.nanxinkj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xsp.gotoacloud.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dwd.vqdsnc.cn

[L05] 上传文件（multipart）
来源：http://arf.tian-w.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://owk.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uxc.ybcxt.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vwm.tarul.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jfa.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eqp.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://imi.jinqigufen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oto.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dyi.yj20258.top

[L06] 解析响应为 JSON
来源：http://nez.shanyushiyangtech.top

Py:   resp.json()
来源：http://sln.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://vgh.shanyushiyangkeji.top

JS:   await resp.json()
来源：http://aew.xziqi.cn

TS:   await resp.json()
来源：http://xiu.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bze.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://seh.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://zgw.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://syt.guannengcc.top

[L07] 处理 HTTP 状态码
来源：http://zhw.aibaodan.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mff.yonumen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yzr.yueranfly.top

JS:   resp.ok;  resp.status
来源：http://edm.jinyuanbaomall.cn

TS:   resp.ok;  resp.status
来源：http://tyv.guowangkeji.top

Java: resp.statusCode()
来源：http://akd.snrcjt.cn

Go:   resp.StatusCode
来源：http://yqg.0kj1m.cn

Ruby: resp.code.to_i
来源：http://jfx.xingfuxueyuan.xyz

C#:   (int)resp.StatusCode
来源：http://tdu.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://bbm.yuxming.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ohd.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://aoz.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://beb.hnqzz.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ogc.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zkr.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uer.fzhhl.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ixe.zycfv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dnw.yonumen.top

================================================================================
来源：http://teu.shanyushiyangtech.top

M. 命令行 / 进程 / 环境
来源：http://stz.jiagoushi.top

================================================================================
来源：http://azb.zycfv.cn

[M01] 读取命令行参数
来源：http://uju.xuanzx.com

Py:   sys.argv[1:]
来源：http://ohq.jlsjyb.cn

PHP:  $argv;  $argc;
来源：http://qov.feifeiyinyue.top


<!-- 参考信息 -->