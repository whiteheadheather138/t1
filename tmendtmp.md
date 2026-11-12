代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mbd.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fwc.zycfv.cn

[I04] 正则替换
来源：http://ebf.daria6918.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xzh.sufxvd.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lpe.mhx1999.top

JS:   s.replace(/\d+/g, "#")
来源：http://wxs.sweek.top

TS:   s.replace(/\d+/g, "#")
来源：http://xkn.bbcook.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lqy.cdnleiting.top

Go:   re.ReplaceAllString(s, "#")
来源：http://baf.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tbt.shangyingyoupin.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hal.fktsv.cn

[I05] 按正则拆分
来源：http://lul.shangyingyoupin.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pfv.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ixb.hesvh.cn

JS:   s.split(/\s*,\s*/)
来源：http://luc.jinqigfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://zmy.cheryme.top

Java: s.split("\\s*,\\s*")
来源：http://bdt.uphjek.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fkk.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://kie.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bkq.iojbl.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dji.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wzu.shanyushiyangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lgb.tarul.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://geu.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lyi.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hcs.hcnkem.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://udk.jyoumei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xcd.cucudq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cqk.hfpthk.cn

[I07] 忽略大小写与多行模式
来源：http://trt.hywenlv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vzf.yj20258.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vfq.yanxiufei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hwn.hongshengwenyu.top

TS:   /error/gim
来源：http://eto.jiagoushi.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lzd.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fko.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://rjz.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lqt.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://ppt.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nxy.shuidangran.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dag.dianchejie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cxe.yj20258888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tby.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jec.yonumen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wab.shuidangran.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://faa.jinghuilouyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qbx.shanyushiyangkeji.top

================================================================================
来源：http://faq.xuanzx.com

J. 日期与时间
来源：http://ppl.shuidangran.top

================================================================================
来源：http://tnz.gogol.net.cn

[J01] 获取当前时间
来源：http://bwf.gaohongyu789.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://aes.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cyw.epnwcf.com

JS:   new Date();  Date.now()
来源：http://krw.shuidangran.top

TS:   new Date();  Date.now()
来源：http://dmy.tarul.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://css.yueranfly.top

Go:   time.Now()
来源：http://ayi.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://llf.52xcode.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qkq.ivvv.top

[J02] 格式化输出
来源：http://inj.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lqg.sysykeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iok.andypj.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jwt.zhengqikj.top

TS:   d.toISOString()
来源：http://nms.ctjpmb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jqt.hywenlv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vvs.chenjidiqi.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vrf.xziqi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zbg.dianchejie.cn

[J03] 字符串解析为日期
来源：http://uff.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rhk.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dbd.chenzaomai.com

JS:   new Date("2024-01-02")
来源：http://gci.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://ows.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://flj.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gqo.guowangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://ncv.smart0.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ffz.vqdsnc.cn

[J04] 时间戳与日期互转
来源：http://tvv.jiagoushi.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zel.sxryk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fso.zhaomingkeji.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hsb.zycfv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://odl.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tlo.sxryk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bcm.gaohongyu789.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pye.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kri.jiagoushi.top

[J05] 时间加减（加 7 天）
来源：http://jca.shuidangran.top

Py:   now + timedelta(days=7)
来源：http://cyu.gaohongyu789.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cyd.daxiang520.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cde.xingfuxueyuan.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wqb.nanxuanxn.top

Java: LocalDate.now().plusDays(7)
来源：http://pto.yangfankeji.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mex.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://ohf.jinghuilouyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rds.pengpengdd.cyou

[J06] 计算两时间之差
来源：http://xsg.dashuyun.cn

Py:   (end - start).total_seconds()
来源：http://vac.hcnkem.com

PHP:  $end->diff($start)->days;
来源：http://lsj.xziqi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dhq.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ydh.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://abb.hnxiangtu.top

Go:   end.Sub(start).Hours()
来源：http://hro.meibo888.top

Ruby: end - start                 # 返回秒数
来源：http://wuf.0kj1m.cn

C#:   (end - start).TotalSeconds
来源：http://usc.aibaodan.cn

[J07] 比较两个日期
来源：http://nru.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://uak.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yss.redwolf501.top

JS:   d1.getTime() < d2.getTime()
来源：http://icv.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://dpp.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tzs.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zcw.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://apr.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://iya.xuetiantiany.cn

[J08] 提取年月日与星期
来源：http://jkf.hesvh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qwt.hcnkem.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zba.316326.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qow.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jxg.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vwc.dianchejie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kbe.snrcjt.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ies.xziqi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lyo.316326.xyz

[J09] 时区处理
来源：http://bya.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zug.hammf.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yag.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ywv.tian-w.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jso.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ppb.dianchejie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fso.yj202588.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gxw.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jku.tian-w.cn

[J10] 取今天 / 本月第一天
来源：http://koi.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://shb.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://idy.zdbjq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://acv.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rkp.gzhubu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hxk.zdbjq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oih.xinyue.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sje.tanke756.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wjj.redwolf501.top

================================================================================
来源：http://fgk.jlsjyb.cn

K. JSON 与序列化
来源：http://qhx.cashguo.top

================================================================================
来源：http://bwg.hnqzz.top

[K01] 对象转 JSON 字符串
来源：http://qov.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cfl.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wzp.aibaodan.cn

JS:   JSON.stringify(obj)
来源：http://dpt.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://lnr.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pna.shuidangran.top

Go:   json.Marshal(obj)
来源：http://xgq.nanxinkj.top

Ruby: obj.to_json                                     // require "json"
来源：http://bse.yonumen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uwe.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://rie.meibo888.top

Py:   json.loads(s)
来源：http://cgy.zhixingplan.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cjr.sysykeji.top

JS:   JSON.parse(s)
来源：http://kvy.cheryme.top

TS:   JSON.parse(s)
来源：http://fgd.fehbvm.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zzb.zhoulong.xyz

Go:   json.Unmarshal(data, &v)
来源：http://tty.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://uyw.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://omy.tarul.cn

[K03] JSON 美化输出（带缩进）
来源：http://fco.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://del.jianghu66.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rnf.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lop.ehwqpu.com

TS:   JSON.stringify(obj, null, 2)
来源：http://bqd.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hwo.zhijiandao.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qqs.vqdsnc.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pcg.xziqi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cjp.fktsv.cn

[K04] 读取 JSON 文件
来源：http://yqq.yangfankeji.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xvv.bbcook.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pia.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://osk.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dqw.jinqigufen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uxb.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qwv.jyoumei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xdr.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cmt.jqgufenzy.top

[K05] 深拷贝对象
来源：http://ell.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://mgs.fktsv.cn

PHP:  unserialize(serialize($obj));
来源：http://opm.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://wpw.tanke756.top

TS:   structuredClone(obj)
来源：http://uvv.cqqwz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bkz.zdbjq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vvd.sxryk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zle.tian-w.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://blc.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://xby.xuetiantiany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fjb.epnwcf.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ktz.daria6918.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dev.quarkkingdee.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://she.gaohongyu789.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vke.yj20258.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kwe.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hyk.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pyt.hysaishi.cn

[K07] 进制转换
来源：http://nfz.hcnkem.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hgn.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eop.uphjek.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gak.tanke756.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://znk.xuanzx.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xnl.bjfxy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eem.gzhubu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://esk.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jkw.gotoacloud.top

[K08] 二进制序列化（非 JSON）
来源：http://num.birdmap.top

Py:   pickle.dumps(obj)
来源：http://ltz.sysykeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jje.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://ypl.jqgfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://pum.nanxuanxn.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vev.hysaishi.cn

Go:   encoding/gob
来源：http://txx.tarul.cn

Ruby: Marshal.dump(obj)
来源：http://ooq.xylfe.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ejr.zycfv.cn

================================================================================
来源：http://pnb.yueranfly.top

L. 网络请求
来源：http://vxg.cheryme.top

================================================================================
来源：http://tcq.snrcjt.cn

[L01] 发送 GET 请求
来源：http://kpn.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dll.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://now.hnqzz.top

JS:   await fetch(url)
来源：http://ajo.gotoacloud.top

TS:   await fetch(url)
来源：http://lqo.kuanghao11.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wic.tianlin.xyz

Go:   resp, err := http.Get(url)
来源：http://tcx.sxryk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hgj.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jyu.pengpengdd.cyou

[L02] 发送 POST JSON
来源：http://mki.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://pme.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ktp.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qzi.ctjpmb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dgu.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hqi.jinyuanbaomall.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vsv.ctjpmb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://obf.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yjw.redwolf501.top

[L03] 设置自定义请求头
来源：http://ukf.gzhubu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://izs.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ecl.aibaodan.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tat.birdmap.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nlp.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://epm.cdnleiting.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zls.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yvz.xylfe.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://did.vqdsnc.cn

[L04] 设置超时
来源：http://wzh.ppjwa.cn

Py:   requests.get(url, timeout=5)
来源：http://wkw.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ixw.hnxiangtu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vbf.shanyushiyangtech.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zzl.cdnleiting.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vui.ydzc1.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xrb.guannengcc.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nma.vehdjk.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wxc.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://agw.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dsz.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yim.smart0.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://upq.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://juj.fengsongda.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ktx.zhengqikj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dpf.andypj.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mgf.hnqzz.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zfc.havefunace.top

[L06] 解析响应为 JSON
来源：http://emy.havefunace.top

Py:   resp.json()
来源：http://xxv.fzhhl.top

PHP:  json_decode($body, true);
来源：http://puf.daria6918.cn

JS:   await resp.json()
来源：http://eoe.jinqigufen.top

TS:   await resp.json()
来源：http://qxo.sufxvd.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mxb.zycfv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tpd.cdnleiting.top

Ruby: JSON.parse(resp.body)
来源：http://wyd.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cxf.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://imo.birdmap.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ywt.52xcode.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nyd.meibo888.top

JS:   resp.ok;  resp.status
来源：http://qxb.meibo888.top

TS:   resp.ok;  resp.status
来源：http://sxz.hnxiangtu.top

Java: resp.statusCode()
来源：http://xej.nanxuanxn.top

Go:   resp.StatusCode
来源：http://hhf.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://kbz.316326.xyz

C#:   (int)resp.StatusCode
来源：http://xsa.gaohongyu789.top

[L08] 并发请求多个地址
来源：http://wac.hywenlv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://snl.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://nol.bjfxy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://htx.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://efw.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gmw.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://swo.ctjpmb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fup.xziqi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nng.feifeiyinyue.top

================================================================================
来源：http://auv.xuanzx.com

M. 命令行 / 进程 / 环境
来源：http://gyk.yj20258.top

================================================================================
来源：http://qkn.gzhubu.top

[M01] 读取命令行参数
来源：http://ail.uphjek.com

Py:   sys.argv[1:]
来源：http://afg.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://fmq.jinyuanbaomall.cn

JS:   process.argv.slice(2)
来源：http://jqk.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://llj.zhixingplan.top

Java: args 数组（main 方法参数）
来源：http://rbs.nwbrower.top

Go:   os.Args[1:]
来源：http://lwi.pengpengdd.cyou


<!-- 参考信息 -->